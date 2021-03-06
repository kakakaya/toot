Release instructions
====================

* Update the version number in `setup.py`
* Update the `CHANGELOG.md` with the release notes & date
* Tag a release
* Push master & tag to GitHub

Publishing to PyPI
------------------

* `make dist` to create source and wheel distributions
* `make publish` to push them to PyPI

Publishing to Debian repo
-------------------------

Publishing deb packages is done via [ihabunek/packages](https://github.com/ihabunek/packages)

* `make deb` to create the debian package
* copy deb file to packages project directory
* in packages project directory:
    * `make` to build the repo files
    * `make publish` to send them to the server
