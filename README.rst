========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis| |appveyor|
        | |codecov|
    * - package
      - | |version| |wheel| |supported-versions| |supported-implementations|
        | |commits-since|
.. |docs| image:: https://readthedocs.org/projects/katatest/badge/?style=flat
    :target: https://readthedocs.org/projects/katatest
    :alt: Documentation Status

.. |travis| image:: https://api.travis-ci.org/dellielo/katatest.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/dellielo/katatest

.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/dellielo/katatest?branch=master&svg=true
    :alt: AppVeyor Build Status
    :target: https://ci.appveyor.com/project/dellielo/katatest

.. |codecov| image:: https://codecov.io/github/dellielo/katatest/coverage.svg?branch=master
    :alt: Coverage Status
    :target: https://codecov.io/github/dellielo/katatest

.. |version| image:: https://img.shields.io/pypi/v/katatest.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/katatest

.. |wheel| image:: https://img.shields.io/pypi/wheel/katatest.svg
    :alt: PyPI Wheel
    :target: https://pypi.org/project/katatest

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/katatest.svg
    :alt: Supported versions
    :target: https://pypi.org/project/katatest

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/katatest.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/katatest

.. |commits-since| image:: https://img.shields.io/github/commits-since/dellielo/katatest/v0.0.0.svg
    :alt: Commits since latest release
    :target: https://github.com/dellielo/katatest/compare/v0.0.0...master



.. end-badges

Mise pratique de tests sur un projet Kata

* Free software: MIT license

Installation
============

::

    pip install katatest

You can also install the in-development version with::

    pip install https://github.com/dellielo/katatest/archive/master.zip


Documentation
=============


https://katatest.readthedocs.io/


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
