director-buckminster-b3-install
===============================

Ant script for installing director, Buckminster headless and b3 headless.

This script will install the director, Buckminster headless (all versions) and the latest b3 headless.

It will install use these properties

    base.dir.install     where all tools will be installed, each
							one with their own directory, e.g.,
							${base.dir.install}/director,
							${base.dir.install}/buckminster-4.3, etc.
							It defaults to ${user.home}

    eclipse.download	The base URL Eclipse main download site
							Default: http://download.eclipse.org

You can run the script simply by

    ant -f director-buckminster-b3-install.ant <target>

The main targets are

    install-all
    install-buckminster-3.6
    install-buckminster-3.7
    install-buckminster-4.2
    install-buckminster-4.3
    install.b3
    install.p2.director

The **install-all** will install all the tools.

You can have the tools installed in a directory different from the default one with

    ant -f director-buckminster-b3-install.ant <target> -Dbase.dir.install=<absolute path>
