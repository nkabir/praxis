# Eclipse for Python Development

Note that we use _separate_ installations of Eclipse for various languages:

* Java
* C/C++
* Scripting: Javascript, Bash and Python

Download [Eclipse Juno JEE](http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/junor).

Unzip the folder into

    $HOME/local/eclipse-juno/eclipse-python

Create a bash script to launch this e.g. `eclipse-python.sh`. Create your new work space with a folder structure as follows:

    /home/asmith/workspaces/juno/python

# Plugins

## Mercurial Plugin

Install the Mercurial plugin from here:

    http://marketplace.eclipse.org/content/mercurialeclipse-was-hgeclipse

The update site is

    http://cbes.javaforge.com/update

Add this update site. Go to `Help->Install New Software...`

<img src="https://dl.dropbox.com/u/59707331/praxis/eclipse-juno/1-main.png" width="100%" />

Next, add the Mercurial plugin site.

<img src="https://dl.dropbox.com/u/59707331/praxis/eclipse-juno/2-add-site.png" width="100%" />

<img src="https://dl.dropbox.com/u/59707331/praxis/eclipse-juno/3-add-repository.png" width="100%" />

Be sure to install _only_ the `MercurialEclipse` plugin. Do **NOT** install the Windows Binaries.

<img src="https://dl.dropbox.com/u/59707331/praxis/eclipse-juno/4-install.png" width="100%" />

Follow the remaining instructions and you'll have Mercurial support in Eclipse.

## Python Plugin

Python support has been integrated into the Aptana Studio Plugin. It's open source and available at [http://www.aptana.com](http://www.aptana.com).



