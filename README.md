gitolite-tools
==============

Description
-----------

Collection of tools to work with [gitolite][] repositories.

So far implemented:

* git gl-desc - Display or edit description of
  [gitolite wildcard repositories][wildrepos].
* git gl-perms - Display or edit permissions of
  [gitolite wildcard repositories][wildrepos].
* git gl-info - Display [gitolite][] server information

Installation
------------

By default, the programs will be installed to "`git --exec-path`".
Just call:

	make && sudo make install

If git is installed to your home directory, `sudo` is not needed.

Installation directory can also be specified by setting `gitexecdir`, e.g.:

	make && make gitexecdir=$HOME/gitexec install

This can be useful if you can't or don't want to mess with the git
installation. gitolite-tools can then be used by setting `GIT_EXEC_PATH`.
For example:

	GIT_EXEC_PATH="$HOME/gitexec:$(git --exec-path)"

Copyright
---------

Copyright (c) 2010 Teemu Matilainen <teemu.matilainen@iki.fi>

License: [Apache 2](http://www.apache.org/licenses/LICENSE-2.0)

[gitolite]: http://github.com/sitaramc/gitolite
[wildrepos]: http://github.com/sitaramc/gitolite/tree/wildrepos
