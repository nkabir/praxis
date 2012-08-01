## Installation

Note that we use _separate_ installations of Eclipse for various languages:

* Java
* C/C++
* Scripting: Javascript, Bash and Python

Download [Eclipse Juno JEE](http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/junor).

If you are setting up a Python tool chain, unzip the folder into

    $HOME/local/eclipse-juno/eclipse-python

Create a bash script to launch this e.g. `eclipse-python.sh`. Create your new work space with a folder structure as follows:

    /home/asmith/workspaces/juno/python

## General Plugins

### Mercurial Plugin

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

## Scripting Languages

Note that you should create a separate installation specifically for scripting languages.

### Python

Python support has been integrated into the Aptana Studio Plugin. It's open source and available at [http://www.aptana.com](http://www.aptana.com).

## Java

Unzip Juno into `$HOME/local/eclipse-juno/eclipse-java/` followed by the Mercurial plugin as outlined above.

### Maven

You'll need the `m2eclipse` plugin to support Maven projects. Add the following repository to Eclipse:

    http://download.eclipse.org/technology/m2e/releases

Once it's installed, go to `Window->Preferences->Maven->Installations` and change the default to a `maven2` installation (`maven3` has compatibility issues with many plugins). Also, change `User Interface` to default to the XML editor for `pom.xml` files---the structured editor is sluggish.

### Color Themes

Aptana provides theming for Python. For Java, you'll need the Eclipse Color Theme plugin available at [http://eclipsecolorthemes.org/](http://eclipsecolorthemes.org/). I currently use [vibrant ink](http://eclipsecolorthemes.org/?view=theme&id=3).

### Checkstyle

The Checkstyle plugin allows the user to define a uniform set of coding conventions that are analyzed by Eclipse. The plugin is available via the [Eclipse marketplace](http://marketplace.eclipse.org/content/checkstyle-plug).
