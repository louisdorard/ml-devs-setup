# LOCAL Set-Up Instructions

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/louisdorard/ml-devs-setup/local-setup?filepath=Intro-Jupyter.ipynb)

## Install

### miniconda

On Mac I used Homebrew's Cask: `brew cask install miniconda`. You can initialize it for your shell with `conda init YOUR_SHELL_NAME`.

Update it via `conda update —all -y`.

### `ml-devs` environment

Create

```bash
conda env create -f environment.yml
conda activate ml-devs
```

Update

`conda env update -f environment.yml`

### Jupyter

Install a few packages so you can then start Jupyter from your base conda environment:

```bash
conda activate base
conda install jupyterlab rise jupyter_contrib_nbextensions nb_conda_kernels
```

* rise: to turn notebooks into slideshows
* jupyter_contrib_nbextensions: to make it easier to customize rise
* nb_conda_kernels: to allow usage of any environment as Jupyter kernel

## Copyright

[Louis Dorard](http://louisdorard.com) © All Rights Reserved

Follow me on Twitter [@louisdorard](https://twitter.com/louisdorard) 