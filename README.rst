========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis| |appveyor| |requires|
        | |coveralls| |codecov|
    * - package
      - | |version| |downloads| |wheel| |supported-versions| |supported-implementations|
        | |commits-since|

.. |docs| image:: https://readthedocs.org/projects/lambda-test-helper/badge/?style=flat
    :target: https://readthedocs.org/projects/lambda-test-helper
    :alt: Documentation Status

.. |travis| image:: https://travis-ci.org/hwine/lambda-test-helper.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/hwine/lambda-test-helper

.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/hwine/lambda-test-helper?branch=master&svg=true
    :alt: AppVeyor Build Status
    :target: https://ci.appveyor.com/project/hwine/lambda-test-helper

.. |requires| image:: https://requires.io/github/hwine/lambda-test-helper/requirements.svg?branch=master
    :alt: Requirements Status
    :target: https://requires.io/github/hwine/lambda-test-helper/requirements/?branch=master

.. |coveralls| image:: https://coveralls.io/repos/hwine/lambda-test-helper/badge.svg?branch=master&service=github
    :alt: Coverage Status
    :target: https://coveralls.io/r/hwine/lambda-test-helper

.. |codecov| image:: https://codecov.io/github/hwine/lambda-test-helper/coverage.svg?branch=master
    :alt: Coverage Status
    :target: https://codecov.io/github/hwine/lambda-test-helper

.. |version| image:: https://img.shields.io/pypi/v/lambda-test-helper.svg
    :alt: PyPI Package latest release
    :target: https://pypi.python.org/pypi/lambda-test-helper

.. |commits-since| image:: https://img.shields.io/github/commits-since/hwine/lambda-test-helper/v0.1.0.svg
    :alt: Commits since latest release
    :target: https://github.com/hwine/lambda-test-helper/compare/v0.1.0...master

.. |downloads| image:: https://img.shields.io/pypi/dm/lambda-test-helper.svg
    :alt: PyPI Package monthly downloads
    :target: https://pypi.python.org/pypi/lambda-test-helper

.. |wheel| image:: https://img.shields.io/pypi/wheel/lambda-test-helper.svg
    :alt: PyPI Wheel
    :target: https://pypi.python.org/pypi/lambda-test-helper

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/lambda-test-helper.svg
    :alt: Supported versions
    :target: https://pypi.python.org/pypi/lambda-test-helper

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/lambda-test-helper.svg
    :alt: Supported implementations
    :target: https://pypi.python.org/pypi/lambda-test-helper


.. end-badges

Support testing installed AWS lambda functions.

Installation
============

::

    pip install lambda-test-helper

Documentation
=============

https://lambda-test-helper.readthedocs.io/

Development
===========

To run the all tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOPTS=--cov-append
            tox

    - - Other
      - ::

            PYTEST_ADDOPTS=--cov-append tox
