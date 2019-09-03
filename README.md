# ML Workshops — Set-Up Instructions

All Rights Reserved © <a href="http://www.louisdorard.com" style="color: #6D00FF;">Louis Dorard</a>

<img src="http://s3.louisdorard.com.s3.amazonaws.com/ML_icon.png">

Our Machine and Deep Learning workshops include “lab” sessions, with exercises to do on your laptop. This document contains the required set-up instructions to prepare the environment you’ll use for these exercises.

The environment is based on a service called Floyd. We explain its benefits below, and we provide information to get started. (More instructions will be provided at the end of the workshop, so you can set up a similar environment on your own machine.)

Finally, some optional instructions are given.

***

## Main instructions

Please follow these instructions from the machine you’ll be using during the workshop:

* [ ] Sign up for a Floyd account via [floydhub.com](https://www.floydhub.com/). Floyd is a cloud platform to set up Python and [Jupyter](https://jupyter.org/) environments, provisioned with all the software we'll need.
* [ ] Join our Slack messaging group via [this link](https://louisdorard.com/slack). Slack is the preferred way to communicate with your instructor during and prior to the workshop.
* [ ] Send your Floyd username to your instructor via Slack (@louis or @christophe), so he can add you to our Floyd team.
* [ ] Make sure you have a recent version of [Chrome](http://google.com/chrome). You could try using a different browser, but we have noticed issues with the web interfaces we use for these workshops (whereas everything was tested with Chrome and works well).

## Why Floyd

There are 3 main reasons:

* It’s common practice to use powerful (GPU-equipped) machines in the cloud for Machine and Deep Learning experiments. They make it faster to run experiments, and they can continue running while your laptop is closed.
* Floyd makes it much faster to set up cloud machines than other services, and much more convenient to persist work done on these machines.
* You won’t have to download heavy datasets (several GB for the DL workshop): they’re already on Floyd!

## Getting started with the Floyd / Jupyter / Python environment

The main environment we'll be using is that of Jupyter notebooks. Among other features, Jupyter allows editing and executing Python code from a web interface (have a look at the video below for an introduction). Floyd enables to easily set up "workspaces", which provide access to Jupyter environments, hosted on cloud machines, provisioned with all the necessary ML software, and with access to the datasets we'll need.

[Video] [Introduction to Jupyter Notebooks for ML](https://www.youtube.com/watch?v=pwr-pR0tu5Y&&feature=youtu.be)

**Make sure you've shared your username with your instructor and that you've been added to our Floyd [team](https://www.floydhub.com/teams/humancoders/settings).** This will allow you to run Floyd workspaces and to have access to paid features, without having to enter your credit card information. It will also give you access to our datasets and to the access keys to the workshop content.

* [ ] **[Create a new project](https://www.floydhub.com/projects/create)**
  * [ ] Choose "humancoders" as owner (otherwise you won't be able to use our CPU credits)
  * [ ] Include your name in the “Project name”
* [ ] **Create and run a new workspace in this project**
  * [ ] Click on “Create workspace” (blue button)
  * [ ] Click on “Create workspace” (green button)
  * [ ] Choose “Import from GitHub”
  * [ ] Enter the following repository URL: `http://github.com/louisdorard/ml-workshops-setup`
    * [ ] Follow on-screen instructions to run the workspace
* [ ] **Go through the [Intro-Jupyter notebook](Intro-Jupyter.ipynb)**
  * [ ] Make one obvious change to the notebook and save the change
  * [ ] Click on the Shutdown button
  * [ ] Start the workspace again and make sure you can see the change you made to the notebook
* [ ] **Stop the workspace when you're done**

We will show more in class. In the meantime, here are some important remarks:

* ⚠️ Billing starts as soon as you run a workspace (or a job) and ends when you shut it down. **Don’t forget to stop/shutdown your Floyd workspaces/jobs!**
* If you can’t access Floyd, you may have to deactivate proxies on your machine — get in touch with your IT department and with your instructor.
* From the Floyd team: “Spinning up the whole environments from scratch in a public cloud usually takes 10s of minutes. We put in a lot of efforts to reduce it to seconds.”

<!--
In case you cannot use Floyd, you will need to download the workshop datasets and to install all the required ML software on your own machine, which will be time consuming.
-->

### Optional

* Sign up for an [Indico](http://www.indico.io/) account. Indico is a cloud API which exposes pre-built, proprietary Machine Learning and Deep Learning models. Usage is free for non-commercial purposes.
* Sign up for a [Kaggle](http://kaggle.com) account. Kaggle hosts many Machine Learning datasets, challenges, and interesting discussions around them.

## Downloading workshop's code

Your instructor will share with you the URL of the workshop's git repository in class.

### Step 1. Configure ssh keys to access the git repo

Execute the following command in a terminal (you can open a terminal from the Floyd workspace by clicking _File, New, Terminal_):

```bash
mkdir ~/.ssh
echo -e "Host gitlab.com\nIdentityFile /floyd/input/ssh/ml" >> ~/.ssh/config
```

### Step 2. Clone the repo

```bash
cd /floyd/home
git clone URL
```

## Copyright

[Louis Dorard](http://louisdorard.com) © All Rights Reserved

Follow me on Twitter [@louisdorard](https://twitter.com/louisdorard)
