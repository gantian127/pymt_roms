=========
pymt_roms
=========

.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.15021596.svg
        :target: https://doi.org/10.5281/zenodo.15021596

.. image:: https://img.shields.io/badge/CSDMS-Basic%20Model%20Interface-green.svg
        :target: https://bmi.readthedocs.io/
        :alt: Basic Model Interface

.. .. image:: https://img.shields.io/badge/recipe-pymt_roms-green.svg
        :target: https://anaconda.org/conda-forge/pymt_roms

.. image:: https://readthedocs.org/projects/pymt-roms/badge/?version=latest
        :target: https://pymt-roms.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status

.. image:: https://img.shields.io/badge/License-MIT-blue.svg
        :target: hhttps://github.com/gantian127/pymt_roms/blob/master/LICENSE

.. .. image:: https://github.com/gantian127/pymt_roms/actions/workflows/test.yml/badge.svg
        :target: https://github.com/gantian127/pymt_roms/actions/workflows/test.yml

.. .. image:: https://github.com/gantian127/pymt_roms/actions/workflows/flake8.yml/badge.svg
        :target: https://github.com/gantian127/pymt_roms/actions/workflows/flake8.yml

.. .. image:: https://github.com/gantian127/pymt_roms/actions/workflows/black.yml/badge.svg
        :target: https://github.com/gantian127/pymt_roms/actions/workflows/black.yml


pymt_roms is a package that converts `bmi_roms <https://github.com/gantian127/bmi_roms>`_ package into a reusable,
plug-and-play data component for `PyMT <https://pymt.readthedocs.io/en/latest/?badge=latest>`_ modeling framework
developed by Community Surface Dynamics Modeling System (`CSDMS <https://csdms.colorado.edu/wiki/Main_Page>`_).
This allows `ROMS model <https://www.myroms.org/>`_ datasets
to be easily coupled with other datasets or models that expose a `Basic Model Interface <https://bmi.readthedocs.io/en/latest/>`_.

The current implementation supports 2D, 3D and 4D ROMS output datasets defined with geospatial and/or time dimensions (e.g.,
dataset defined with dimensions as [time, s_rho, eta_rho, xi_rho])

========= ===================================
Component PyMT
========= ===================================
Roms      `from pymt.models import Roms`
========= ===================================

---------------
Installing pymt
---------------

Installing `pymt` from the `conda-forge` channel can be achieved by adding
`conda-forge` to your channels with:

.. code::

  conda config --add channels conda-forge

*Note*: Before installing `pymt`, you may want to create a separate environment
into which to install it. This can be done with,

.. code::

  conda create -n pymt python=3
  conda activate pymt

Once the `conda-forge` channel has been enabled, `pymt` can be installed with:

.. code::

   conda install pymt

It is possible to list all of the versions of `pymt` available on your platform with:

.. code::

    conda search pymt --channel conda-forge

**Please note that pymt_roms requires pymt version 1.3.2 or higher**

--------------------
Installing pymt_roms
--------------------

To install `pymt_roms`, use pip

.. code::

  pip install pymt_roms

or conda

.. code::

  conda install -c conda-forge pymt_roms

--------------------
Citation
--------------------
Please include the following references when citing this software package:

Gan, T., Tucker, G.E., Hutton, E.W.H., Piper, M.D., Overeem, I., Kettner, A.J.,
Campforts, B., Moriarty, J.M., Undzis, B., Pierce, E., McCready, L., 2024:
CSDMS Data Components: data–model integration tools for Earth surface processes
modeling. Geosci. Model Dev., 17, 2165–2185. https://doi.org/10.5194/gmd-17-2165-2024

Gan, T. (2025). PyMT plugin for CSDMS ROMS Data Component. Zenodo. https://doi.org/10.5281/zenodo.15021596

--------------------
Coding Example
--------------------

You can learn more details about the coding example from the
`tutorial notebook <https://github.com/gantian127/pymt_roms/blob/master/notebooks/pymt_roms.ipynb>`_.