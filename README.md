[![Anaconda Cloud](https://anaconda.org/conda-forge/cmip6_preprocessing/badges/version.svg)](https://anaconda.org/conda-forge/cmip6_preprocessing)
[![conda-forge](https://img.shields.io/conda/dn/conda-forge/cmip6_preprocessing?label=conda-forge)](https://anaconda.org/conda-forge/cmip6_preprocessing)
[![Pypi](https://img.shields.io/pypi/v/cmip6_preprocessing.svg)](https://pypi.org/project/cmip6_preprocessing)
[![Build Status](https://img.shields.io/github/workflow/status/jbusecke/cmip6_preprocessing/CI?logo=github)](https://github.com/jbusecke/cmip6_preprocessing/actions)
[![codecov](https://codecov.io/gh/jbusecke/cmip6_preprocessing/branch/master/graph/badge.svg)](https://codecov.io/gh/jbusecke/cmip6_preprocessing)
[![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/215606850.svg)](https://zenodo.org/badge/latestdoi/215606850)

![BLM](BLM.png)

Science is not immune to racism. Academia is an elitist system with numerous gatekeepers that has mostly allowed a very limited spectrum of people to pursue a career. I believe we need to change that. 

Open source development and reproducible science are a great way to democratize the means for scientific analysis. **But you can't git clone software if you are being murdered by the police for being Black!**

Free access to software and hollow diversity statements are hardly enough to crush the systemic and institutionalized racism in our society and academia.

If you are using this package, I ask you to go beyond just speaking out and donate [here](https://secure.actblue.com/donate/cmip6_preprocessing) to [Data for Black Lives](http://d4bl.org/) and [Black Lives Matter Action](https://blacklivesmatter.com/global-actions/).

I explicitly welcome suggestions regarding the wording of this statement and for additional organizations to support. Please raise an [issue](https://github.com/jbusecke/cmip6_preprocessing/issues) for suggestions.

# cmip6_preprocessing

Frustrated with how 'dirty' CMIP6 data still is? Do you just want to run a simple (or complicated) analysis on various models and end up having to write logic for each seperate case? Then this package is for you.

Developed during the [cmip6-hackathon](https://cmip6hack.github.io/#/) this package provides utility functions that play nicely with [intake-esm](https://github.com/NCAR/intake-esm).

We currently support the following functions

1. Preprocessing CMIP6 data (Please check out the [tutorial](doc/tutorial.ipynb) for some examples using the [pangeo cloud](ocean.pangeo.io)). The preprocessig includes:
    a. Fix inconsistent naming of dimensions and coordinates
    b. Fix inconsistent values,shape and dataset location of coordinates
    c. Homogenize longitude conventions
    d. Fix inconsistent units
2. [Creating large scale ocean basin masks for arbitrary model output](doc/regionmask.ipynb)

The following issues are under development:
1. Reconstruct/find grid metrics
2. Arrange different variables on their respective staggered grid, so they can work seamlessly with [xgcm](https://xgcm.readthedocs.io/en/latest/)

Check out this recent Earthcube [notebook](https://github.com/earthcube2020/ec20_busecke_etal) (cite via doi: [10.1002/essoar.10504241.1](https://www.essoar.org/doi/10.1002/essoar.10504241.1)) for a high level demo of `cmip6_preprocessing` and [xgcm](https://github.com/xgcm/xgcm).


## Installation

Install `cmip6_preprocessing` via pip:

`pip install cmip6_preprocessing`

or conda:

`conda install -c conda-forge cmip6_preprocessing`

To install the newest master from github you can use pip aswell:

`pip install git+pip install git+https://github.com/jbusecke/cmip6_preprocessing.git`

