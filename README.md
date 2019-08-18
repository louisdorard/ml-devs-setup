# LOCAL Set-Up Instructions

You can set up a temporary environment in the cloud via Binder:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/louisdorard/ml-devs-setup/local-setup?filepath=Intro-Jupyter.ipynb)

You can also generate a Docker image via [repo2docker](https://repo2docker.readthedocs.io/en/latest/). Otherwise, follow the instructions below to set up your own local environment with conda.

## conda (Python distro)

On Mac I used Homebrew's Cask: `brew cask install miniconda`. You can initialize it for your shell with `conda init YOUR_SHELL_NAME`.

Windows or Linux: download from https://www.anaconda.com/distribution/

Update it via `conda update —all -y`.

### `ml-devs` conda environment

#### Create environment

From this repo's directory:

```bash
conda env create -f environment.yml
conda activate ml-devs
```

TODO test this on Windows

#### Update environment

`conda env update -f environment.yml`

### Install Jupyter in base environment

Install a few packages so you can then start Jupyter from your base conda environment:

```bash
conda activate base
conda install jupyterlab rise jupyter_contrib_nbextensions nb_conda_kernels
```

TODO test this on Windows

* rise: to turn notebooks into slideshows
* jupyter_contrib_nbextensions: to make it easier to customize rise
* nb_conda_kernels: to allow usage of any environment as Jupyter kernel

Once it's installed, fire up Jupyter Lab

```bash
jupyter-lab
```

This should automatically open your browser at localhost:8888/

### IDE (Optional)

I use VS Code...

* One advantage is that it has built-in Git
* Recommended extensions: Python, Docker, Rainbow CSV, Excel Viewer, Markdown All in One
* Go through [Getting Started with Python in VS Code](https://code.visualstudio.com/docs/python/python-tutorial)

TODO On Mac it can be installed from Homebrew

On Linux it can be installed from the [Snap Store](snapcraft.io/store)

If you're (interested in) using a cloud machine for development, coder.com allows to run VS Code on a server.

### Scripts

Using papermill.

Can be run from a Terminal application (I use iTerm2 on Mac) or from VS Code or from Jupyter Lab.

If you are on Windows, you might want to try the [Ubuntu app](https://www.microsoft.com/p/ubuntu/9nblggh4msv6?activetab=pivot:overviewtab), or to install Ubuntu alongside Windows, to make it easier to use the command line.

## Copyright

[Louis Dorard](http://louisdorard.com) © All Rights Reserved

Follow me on Twitter [@louisdorard](https://twitter.com/louisdorard) 