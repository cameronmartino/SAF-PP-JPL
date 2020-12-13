16S analysis for "Assessment of the NASA Standard Spore Assay in Predicting Bacterial Populations of a Mars Mission Assembly Facility".

### Repository Structure

* code

This directory contains the code (as notebooks) for each step in a numerically organized format. More descriptions can be found within the README file for that directory.

* data

This directory contains the input data, along with some output from computationally expensive tools. 

Source tracking done with the entirety of the Earth Microbiome and American Gut projects is not included in this repository due to size (analysis in `code/2.1.0-time-source-variation.ipynb`). However, the data tables for that sourcetracking step can be re-generated through `redbiom` with code within  `code/2.1.0-time-source-variation.ipynb`.

* results

The main and extended figures and tables from the paper which can be reproduced by running the notebooks within the `code` directory.

### Setup

There are two options for setup to run the notebooks.

The first option is a QIIME 2019.10 environment amended with any additional plugins. This option is preferable for `OSX` users. The conda yml file is provided in `environment/jpl-environment.yml`. Installation of the environment can be done through `conda env create -n saf-pp-jpl --file environment/jpl-environment.yml`.

With the environment installed and activated each notebook can be run and populate the `results` directory with all of the extended tables and figures used in the paper.