.. image:: https://img.shields.io/badge/rtn--035-lsst.io-brightgreen.svg
   :target: https://rtn-035.lsst.io
.. image:: https://github.com/lsst/rtn-035/workflows/CI/badge.svg
   :target: https://github.com/lsst/rtn-035/actions/
..
  Uncomment this section and modify the DOI strings to include a Zenodo DOI badge in the README
  .. image:: https://zenodo.org/badge/doi/10.5281/zenodo.#####.svg
     :target: http://dx.doi.org/10.5281/zenodo.#####

###################################
The Rubin Operations Center at SLAC
###################################

RTN-035
=======

As one of the operating partners for Rubin Operations, SLAC is responsible for the stewardship of the LSST Camera: SLAC staff will provide scientific and technical support for LSST Cam operations at the Summit Facility in Chile, and SLAC Observing Specialists will perform night-time operations both on-site and remotely. To fulfill these obligations, SLAC will need (and has budgeted for) a remote observing room (providing a direct video link and mirrored views of the observatory controls at the Rubin Summit Facility), and associated collaboration space. In this design document we derive the specifications of this remote observing room as the central component of a more general, multi-purpose Rubin Operations Center, situated in the 1st floor of the Kavli Building at SLAC. This Center will support collaboration by others in the Rubin Operations team (including the staff processing the LSST image data at the Rubin US Data Facility), and with members of the LSST Dark Enerrgy Science Collaboration. It will also act as a hub for the wider KIPAC community as it does science with the LSST data, and be a major destination for visitors on lab tours and other public outreach events. 

**Links:**

- Publication URL: https://rtn-035.lsst.io
- Alternative editions: https://rtn-035.lsst.io/v
- GitHub repository: https://github.com/lsst/rtn-035
- Build system: https://github.com/lsst/rtn-035/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally with `Sphinx`_:

.. code-block:: bash

   git clone https://github.com/lsst/rtn-035
   cd rtn-035
   pip install -r requirements.txt
   make html

.. note::

   In a Conda_ environment, ``pip install -r requirements.txt`` doesn't work as expected.
   Instead, ``pip`` install the packages listed in ``requirements.txt`` individually.

The built technote is located at ``_build/html/index.html``.

Editing this technical note
===========================

You can edit the ``index.rst`` file, which is a reStructuredText document.
The `DM reStructuredText Style Guide`_ is a good resource for how we write reStructuredText.

Remember that images and other types of assets should be stored in the ``_static/`` directory of this repository.
See ``_static/README.rst`` for more information.

The published technote at https://rtn-035.lsst.io will be automatically rebuilt whenever you push your changes to the ``main`` branch on `GitHub <https://github.com/lsst/rtn-035>`_.

Updating metadata
=================

This technote's metadata is maintained in ``metadata.yaml``.
In this metadata you can edit the technote's title, authors, publication date, etc..
``metadata.yaml`` is self-documenting with inline comments.

Using the bibliographies
========================

The bibliography files in ``lsstbib/`` are copies from `lsst-texmf`_.
You can update them to the current `lsst-texmf`_ versions with::

   make refresh-bib

Add new bibliography items to the ``local.bib`` file in the root directory (and later add them to `lsst-texmf`_).

.. _Sphinx: http://sphinx-doc.org
.. _DM reStructuredText Style Guide: https://developer.lsst.io/restructuredtext/style.html
.. _this repo: ./index.rst
.. _Conda: http://conda.pydata.org/docs/
.. _lsst-texmf: https://lsst-texmf.lsst.io
