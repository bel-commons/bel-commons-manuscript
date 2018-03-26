BEL Commons Manuscript
======================
This repository contains code, resources, and tutorials described in "BEL Commons: an environment for exploration 
and analysis of networks encoded in Biological Expression Language."

Structure of Repository
-----------------------
- data: several folders containing instructions how to automatically download and process differential gene expression experiments
- screenshots: the screenshots for the tutorial (see below)

Reproducing the UCMPA Analysis
------------------------------
This tutorial shows how to reproduce the analysis shown in Figure 5 of the manuscript.

Step 1
~~~~~~
From the main page on `BEL Commons <https://pybel.scai.fraunhofer.de>`_, find the query builder.

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_1.png
        :alt: Step 1: How to Find the Query Builder
        :width: 100%
        :align: center

Step 2
~~~~~~
Use the search box to find the example NeuroMMSig AD subgraphs. Click their radio boxes to include in the query

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_2.png
        :alt: Step 2: Select networks
        :width: 100%
        :align: center

Step 3
~~~~~~
This query does not need any seeding, so scroll down to "Filters and Mutations." As a pre-processing step, use the "Filters and Mutations" box to add functions to remove MGI nodes, RGD nodes, collapse on central dogma, and rewire variants.

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_3.png
        :alt: Step 3: Add filters and mutations
        :width: 100%
        :align: center

Step 4
~~~~~~
Submit the query

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_4.png
        :alt: Step 4: Submit the query
        :width: 100%
        :align: center
