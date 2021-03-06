Introduction
============

SCM Backup is a tool which makes offline backups of your cloud hosted source code repositories, by cloning them.

It's free and open source!

It supports backing up from multiple source code hosters and backing up multiple users/teams per source code hoster.

At the moment, the following hosters are supported:

- `Bitbucket <https://bitbucket.org/>`_
- `GitHub <https://github.com/>`_
- `GitLab <https://gitlab.com/>`_


How does it work?
-----------------

SCM Backup uses the respective hoster's API to get a list of all your repositories hosted there.

Then, it uses the respective SCM (e.g. `Git <https://git-scm.com/>`_ and/or `Mercurial <https://www.mercurial-scm.org/>`_, which need to be installed on your machine if you have at least one repository of the given type) to clone every repository into your local backup folder - or just pull the newest changes, if it already **is** in your local backup folder.

Many hosters support wikis per repository, which are separate repositories and will be backed up as well.
