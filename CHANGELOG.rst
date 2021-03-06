Changelog
---------

0.2.5
~~~~~

Improvements:

* Added `python3.6` and `Django==1.11`
* Fixed `tests/settings` structure with `basic/` folder
* Added documentation, which is built with `Sphinx`
* Updated `README.rst` with new logo
* Updated `README.rst` with `docs` badge
* Updated `CONTRIBUTING.rst` with new information

Bugs:

* Updated `README.rst` to be compatible with `PyPI`

0.2.4
~~~~~

* Changed the default Django version in the requirements from `>= 1.5.1` to `>= 1.5`
* Added `setup.cfg` to support `python setup.py test` command
* Refactored how the tests work
* Added `tests/conftest.py` file with the fixtures, used fixtures widely
* Changed all test to be functions instead of classes
* Added new classifiers
* Added `pytest-env` to read env variables from `setup.cfg`
* Removed `run_coveralls.py`, added `after_success` section in `.travis.yml`
* Changed the `README.rst` to be shorter

0.2.3
~~~~~

* Added `django@1.10` support
* Now `include` function finds parent `globals()` scope automatically if not provided
* Added protection against infinite recursion
* Added tests for stackable settings definition. See `tests/settings/stacked/`
* Added tests for the new functionality
* Added tests for `django@1.10` in `tox` and `travis`
* Removed `3.2` and `3.3` from `setup.py` since these versions were not tested anyway

0.2.2
~~~~~

* Now supporting `unicode` filenames, fixes https://github.com/sobolevn/django-split-settings/issues/9
* Tests structure is changed
* Removed example
* Changed how `MANIFEST.in` is defined

0.2.1
~~~~~

* Changed ``optional`` to be a function.
* Added ``test_tools.py``, achieved 100% in coverage.
* Removed ``setuptools-git`` from ``setup.py``, now ``Manifest`` is only way to provide ``dist`` sources.
* Added ``run_coveralls.py`` to work on both ``CI`` and local tests.
* Style fixes.

0.2.0
~~~~~

* Now ``tox`` is used for testing.
* Added ``coverage`` information and badge.
* Removed ``pep8`` utility, now using ``pylint``.

0.1.3
~~~~~

* Python 3.5 support, Django 1.9 test-support, documentation updates.

0.1.2
~~~~~

* Fixed Python 3 compatibility. Fixed `issue #7`_.

0.1.1
~~~~~

* Fixed `issue #1`_: now works with Gunicorn, too

0.1.0
~~~~~

* Initial version

.. _`issue #1`: https://github.com/sobolevn/django-split-settings/issues/1
.. _`issue #7`: https://github.com/sobolevn/django-split-settings/issues/7
