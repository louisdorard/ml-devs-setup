# LOCAL Set-Up Instructions

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/louisdorard/ml-devs-setup/local-setup?filepath=Intro-Jupyter.ipynb)

## Install

* Install miniconda (on Mac I used Homebrew's Cask: `brew cask install miniconda`)
* Install jupyter in your base conda environment: `conda install jupyter nb_conda_kernels`
* Create new conda environment

```bash
conda env create -f environment.yml
conda activate ml-devs
```

## Update

`conda env update -f environment.yml`

## Copyright

[Louis Dorard](http://louisdorard.com) © All Rights Reserved

Follow me on Twitter [@louisdorard](https://twitter.com/louisdorard) 