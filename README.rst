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
        :alt: Step 1: How to find the query builder
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

Step 5
~~~~~~
Click the "analyze" button to go to the data upload page

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_5.png
        :alt: Step 5: Go to analysis page
        :width: 100%
        :align: center

Step 6
~~~~~~
Upload a differential gene expression file. Several examples are included in this repository. In the manuscript, we present an analysis on the three results from GSE28146. Select the number of permutations (more are better since it's a randomized algorithm, but it's much slower. A good number is 500.). Finally, add a description so it's easier to identify the data later and press the submit button.

If the data is malformed, you'll get a warning.

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_6.png
        :alt: Step 6: Upload data
        :width: 100%
        :align: center

Step 7
~~~~~~
After submitting, you'll be redirected to the same page where another experiment can be run on the same query. 
This is useful for making differential analysis on the same network with different data sets, as presented in 
the manuscript. Submit several other experiments, and wait for them to complete.

Step 8
~~~~~~
Navigate to "My Activity" from the top of the browser

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_8.png
        :alt: Step 8: Navigate to "My Activity"
        :width: 100%
        :align: center

Step 9
~~~~~~
Scroll to "My Experiments" and click "View Comparison"

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_9.png
        :alt: Step 9: Navigate to "My Activity"
        :width: 100%
        :align: center


Step 10
~~~~~~~
Interpret the experiments (k-means clustering can be added by appending ``?clusters=5`` to the end of the URL)

.. image:: https://raw.githubusercontent.com/cthoyt/bel-commons-manuscript/master/screenshots/ucmpa_step_10.png
        :alt: Step 10: Interpretation
        :width: 100%
        :align: center
