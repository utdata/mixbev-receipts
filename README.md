Mixed Beverage Receipts Lesson
=============================


## Rework

THIS DATA SET IS BEING REWORKED BASED ON NEW DATA BY THE COMPTROLLER ON DATA.TEXAS.GOV

The comptroller now stores 10 years worth of [Mixed Beverage Gross Receipts](https://data.texas.gov/Government-and-Taxes/Mixed-Beverage-Gross-Receipts/naix-2893) data on the [Texas' Socrata portal](https://data.texas.gov).

- I'll first rework this on the new data layout using downloaded data.
- I'll then try to use the Socrata API to pull the data we need.

## From before

This repository is a lesson in a repeatable, transparent data pipeline using Jupyter Notebooks and the Python package called [agate](http://agate.readthedocs.io/).

It uses a `conda` virtual environment.

(Note: If you are using a different virtual environment, you can use mixbev-pip.txt as a requirements file.)

## Setup

This should only have to be done once on your machine. Assumes you are on Mac, but this should work with Windows.

### Install conda

- install [conda](https://conda.io/docs/download.html) or [miniconda](https://conda.io/miniconda.html) for Python 3.6
- run `conda update conda` to make sure it is up-to-date

### Create and configure the environment

- run `conda create -n mixbev --file mixbev-env.txt` to create the mixbev environment that has the pyton packages you need
- run `source activate mixbev` to load the environment so we can add the `agate` package that is not in conda.
- run `pip install agate` to install the [agate](http://agate.readthedocs.io/) package, which is not included in the conda system.

## Updating monthly numbers

- `cd` into the `mixbev-receipts`
- run `source activate mixbev` to enter the virtual environment
- run `jupyter notebook` to start the notebook
- Your browser will open [jupyter](http://localhost:8888/tree)
- Go inside the `notebooks` directory and choose `Mixed-beverages-agate.ipynb` 

The rest of the directions are in the **Mixed beverages agate** notebook.
