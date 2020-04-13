# mybinder-template
A template for future mybinder projects, with all necessary configuration files.
This is set up to run on myBinder in a jupyterlab interface.
The `beakerx` jupyterlab extension enables multiple language kernels e.g. Scala, Kotlin, Python.

Check the badge below to see how it looks: <br>
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanielTemesgen/mybinder-template/master?urlpath=lab)

## Getting Started
Use the template by clicking the green "Use this template" button at the top of the page.

The binder badge above takes you to the following link: <br>
https://mybinder.org/v2/gh/DanielTemesgen/mybinder-template/master?urlpath=lab

Replace it with the following: <br>
https://mybinder.org/v2/gh/YOUR_USER_NAME/YOUR_REPO_NAME/master?urlpath=lab

## File Description
* binder
  * `environment.yml` - conda environment, this includes `beakerx` which enables JVM kernels.
  * `postBuild` - a script which runs after the jupyterlab session has been created. We can then install jupyterlab extensions such as table of contents.
* .jupyter/lab/user-settings/@jupyterlab/apputils-extension/
  * `themes.jupyterlab-settings` - enables dark theme.


## More Information
* [myBinder Docs](https://mybinder.readthedocs.io/en/latest/)
* [beakerx](http://beakerx.com/) is an easy to use jupyterlab extension which among other things, enables JVM kernels to be used.
* A [template](https://github.com/ian-r-rose/binder-workspace-demo) which includes details on how to use a jupyterlab workspace. Will be of interest if you want your jupyterlab session to start with a certain file layout. It involves saving a `workspace.json` file in the binder directory and adding a command to postBuild.
