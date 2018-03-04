This section covers installation of AppleCommander. As of 1.4.0, this should be a bit simpler as SWT is now packaged for each platform.

### Install Java

If you do not already have Java 8 (or later) installed, you will be required to install one.

Fortunately, Oracle maintains a site dedicated to Java at [Java.com](https://java.com/).

The directions to check which version of Java you have installed is [here](https://java.com/en/download/help/version_manual.xml).

### Download AppleCommander

Visit the [AppleCommander release page](https://github.com/AppleCommander/AppleCommander/releases) and download the JAR file for your system.  It will look something like this:

![GitHub release page for AppleCommander](images/github-release-page.png)

#### Graphical Interface

The GUI component comes pre-packaged with all needed dependencies. You do not need to find and install the SWT toolkit any more!

* For Windows use the file with `AppleCommander-win64-VERSION.jar`,
* For Macintosh use `AppleCommander-macosx-VERSION.jar`, and
* For Linux use `AppleCommander-linux64-gtk-VERSION.jar`.

Once the JAR is downloaded, just double-click on the file!

For Linux, you may need to set the file to be executable by allowing the JAR file to be executed as a program.

![Setting execute permission in Ubuntu Linux](images/linux-ubuntu-properties.png)

#### Command-line

The distribution file `AppleCommander-ac.jar` provides a command-line interface to AppleCommander. It is ready to use immediately, but it may be convenient to rename it (e.g. ac.jar) or invoke it from a script, e.g.

GNU bash script (`ac.sh`):
```bash
#!/bin/sh
java -jar ~/bin/ac.jar "${@}"
```

MS DOS batch file (`ac.bat`):
```batch
@echo off
java -jar AppleCommander-1.3.5-ac.jar %*
```

There is a Mac OS X [Apple II homebrew repository](https://github.com/lifepillar/homebrew-appleii) which allows an install of:
```
$ brew install applecommander
```
Visit the GitHub page for information on how to install the tap.

Unix-like environments have the ability to `alias` a command, to give an `ac` command:
```bash
alias ac='java -jar build/libs/AppleCommander-ac-1.4.0-BETA.jar'
```