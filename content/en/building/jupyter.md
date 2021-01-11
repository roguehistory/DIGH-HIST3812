+++
author = "Dr. Graham"
title = "Installing Jupyter"
date = "2020-02-01"
description = "How to install Jupyter"

+++


## Step 1

You need to make yourself familiar with _the command line_. There are many such tutorials out there; I encourage you to follow [this one from Melanie Walsh's Intro to Cultural Analytics class](https://melaniewalsh.github.io/Intro-Cultural-Analytics/Command-Line/The-Command-Line.html)

## Step 2

Anaconda is a package of different programming languages and utilities for 'scientific computing'. Go to the [installation page](https://docs.anaconda.com/anaconda/install/) and find the version that is appropriate for your machine. Download and then run the installer.

Accept all the defaults _until_ you get to this screen:

![Add to path screen](https://docs.anaconda.com/_images/win-install-options.png)

The 'PATH' variable is like a bin where your computer stores the locations of different programs that you want to access from anywhere on your computer (otherwise, you can only access programs when you're in the right place). Tick the 'Add Anaconda3 to my PATH environment variable' check box. Now you'll be able to run Juypter notebooks from the command line in any folder.

Make sure to [verify that everything installed correctly](https://docs.anaconda.com/anaconda/install/verify-install/)

## And GO!

On your computer, search for something called 'Anaconda Navigator'. Launch that, then if you click on 'Jupyter Notebooks' or 'Jupyter Lab' - you are now all set up and ready to go!

![navigator](https://docs.anaconda.com/_images/nav-defaults.png)

An alternative way to launch jupyter notebooks or jupyter labs is to open the command line in a given folder, then type `$ jupyter notebook` or `$ jupyter lab`. Note that you _don't type_ the `$` symbol; this is a convention to indicate that what follows is meant to be typed on the command line.

At this point, if you come across a file with `.ipynb` as its extension, you can open it and run it in a Jupyter notebook or lab. Try it now - right-click on [this link](https://github.com/shawngraham/dhmuse-notebooks/raw/master/python-basics-1.ipynb) and save-as to your computer. Then, open a command line in the folder where you saved the file. Start up `$ jupyter notebook` - which opens a new tab in your browser - and then click on the file you downloaded. Now you can run and save your work locally!

## A Video Walkthrough on Installing and Working with Jupyter Notebook Locally

<iframe width="560" height="315" src="https://www.youtube.com/embed/10FPoTCcv4I" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Included in this tutorial:
- Installing [Miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/#regular-installation)
- Installing Jupyter Notebook using `conda`
- Exploring the [GLAM Workbench](https://glam-workbench.github.io/)
- Running a downloaded notebook locally
- Adding your notebook to a git repository and publishing it with [myBinder](https://mybinder.org/)
