# Creating webapps with Binder that have Seaborn, VPython, and other useful dependencies

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/fomightez/appmode/master?urlpath=apps%2Findex.ipynb)

This repository demonstrates how to create webapps with Binder. This is similar to how Shiny apps work in R.
Using the `appmode` Jupyter plugin, a notebook's code will be run, and then only the markdown cells and
code outputs will be shown.
----

## POST-FORKING DIFFERENCES
- I added seaborn and other useful dependencies after forking this from [here](https://github.com/binder-examples/appmode). (To determine which ones I could place in `environment.yml` to have conda handle install, I opened a Binder from appmode Binder-example and then launched terminal then searched, such as `conda search seaborn` to see if available in conda-forge, based on [here](https://conda.io/docs/user-guide/tasks/manage-pkgs.html#searching-for-packages). Nothing returned for those like `vpython` not available.)
- Updated `launch binder` button to point out my fork.
- Placed dependencies conda cannot handle in `postBuild`.
----

You can check out the `appmode` repository here: https://github.com/oschuett/appmode
