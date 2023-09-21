+++
title = "Publishing Data to the Web with Heroku and Datasette"
date = "2020-02-02"
description = "Step by step instructions for publishing data to the web"
+++

## Prerequisites

You need to have the following installed on your machine:

1. Python. I recommend using Anaconda to manage all of your python related work. [Get Anaconda here](https://www.anaconda.com/distribution/#download-section) and get the 3.7 version.
2. In the instructions below, you will also be installing [Homebrew](https://brew.sh/) if you are on a Mac. Both PC and Windows people will need to install the command line interface (CLI) for [Heroku](https://devcenter.heroku.com/articles/heroku-cli). I recommend Mac people install Homebrew so that they can download the CLI from their terminal (also, lots of useful software is distributed using Homebrew). Windows people don't need Homebrew; they can install the CLI installer for Windows from the Heroku page.

## What is Heroku?

[Heroku](https://www.heroku.com/) is a platform for delivering web apps. For our purposes, it's free. The 0.50$ tour -  a simple server just delivers basic static webpages to the web. If you want some kind of interactivity, or you're doing complex database driven queries and functions, you need a server with a lot more power. Heroku does that. In [my guidance on using Datasette with Glitch](/datasette-with-glitch/) you learned that Glitch can host very small datasets using Glitch's collaborative coding environment. This is great for when you want to quickly test something out, or share very small data, but it's not a good solution if you want to put larger materials online. We'll use Heroku for that.

## Here we go!

### 1. Create a python environment for your work

Open a new terminal (Mac) or start up Conda and start a new terminal window (Windows). (Windows users, look for 'command prompt for powershell anaconda' and start that.) I make a version of python - an 'environment' - just for working with this course by using the command `$ conda create`, like so:

`$ conda create --name dhmuse`

and pressing `y` for 'yes, i do want to create a pythion environment called 'dhmuse''. There are many different packages or bundles of python-legos out there that can be combined to do lots of different things. You create environments to manage all of these pieces so that you don't create conflicts. I create an environment for analytical work, or for creative work, or for database work, or for a unique project, so that my different pieces of code have *just* the right pieces they need. Then, I can remind myself what conda environments I have by entering:

`$ conda env list`

and can then select the one I want by typing it in after the 'activate' command:

`$ conda activate dhmuse`

When I'm finished, I can type

`$ conda deactivate`

and I'm done. Remember! The convention when writing about code is to provide the command prompt `$` or `>` but _you do not enter that prompt yourself!_

---

### 2. Install datasette and csvs-to-sqlite

At the `$` prompt in your new environment which has been activated (you'll see the name of your environment now appearing in your command line), you'll install a utility that converts csvs to sqlite format; that is, from a plain table to a table formatted for use with sql powered databases:

`$ pip install csvs-to-sqlite`

Then

`$ pip install datasette`

_because we are installing inside the environment we just created_ these particular commands (packages; boxes of code legos) will not be available after you type `conda deactivate`. They live inside this environment only.

+ More info about CSVS-toSQLITE [https://github.com/simonw/csvs-to-sqlite](https://github.com/simonw/csvs-to-sqlite)
+ More info about Datasette [https://datasette.readthedocs.io](https://datasette.readthedocs.io)

---

### 3. Convert your table of data to a database

Now we convert your csv table of data to a sql database:

`$ csvs-to-sqlite your-data-table.csv your-database.db`

When it finishes running, check it out via datasette:

`$ datasette your-datasette.db`

Ta da! Your data is running probably at [http://127.0.0.1:8001](http://127.0.0.1:8001). Check it out! Hit ctrl+c in your terminal to stop it.

---

### 4. Publish to the web; install Heroku command line tools

Now we're going to publish to the web, putting it on space at heroku

**If you're on a Mac, get homebrew to install heroku by running these command:**

`$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

`$ brew tap heroku/brew && brew install heroku`

If you're on **Windows**, [download](https://devcenter.heroku.com/articles/heroku-cli) and run the installer.

### 5. Get an account at Heroku

Now, go to [Heroku.com](http://heroku.com) and make an account. Keep note of your username and your password, you'll need them.

### 6. Login to Heroku at the command line

Back in the terminal/command line, now that Heroku is installed, tell it you want to login to your account:

`$ heroku login -i`

It'll ask you for your username and password; enter them.

**Drumroll please!**

### 7. Publish to the web

Now we publish your database file to the web:

`$ datasette publish heroku --name cstm-demo cstm.db`

where the `--name` flag is the subdomain you want your data to be available at. In my case, my choice of 'cstm-demo' becomes available at [http://cstm-demo.herokuapp.com](http://cstm-demo.herokuapp.com)


### Reference
The publish-to-heroku command has many options:

`$ datasette publish heroku --help`

```
Usage: datasette publish heroku [OPTIONS] [FILES]...

Options:
  -m, --metadata FILENAME         Path to JSON file containing metadata to publish
  --extra-options TEXT            Extra options to pass to datasette serve
  --branch TEXT                   Install datasette from a GitHub branch e.g. master
  --template-dir DIRECTORY        Path to directory containing custom templates
  --plugins-dir DIRECTORY         Path to directory containing custom plugins
  --static MOUNT:DIRECTORY        Serve static files from this directory at /MOUNT/...
  --install TEXT                  Additional packages (e.g. plugins) to install
  --plugin-secret <TEXT TEXT TEXT>...
                                  Secrets to pass to plugins, e.g. --plugin-secret
                                  datasette-auth-github client_id xxx
  --version-note TEXT             Additional note to show on /-/versions
  --title TEXT                    Title for metadata
  --license TEXT                  License label for metadata
  --license_url TEXT              License URL for metadata
  --source TEXT                   Source label for metadata
  --source_url TEXT               Source URL for metadata
  --about TEXT                    About label for metadata
  --about_url TEXT                About URL for metadata
  -n, --name TEXT                 Application name to use when deploying
  --help                          Show this message and exit.
```
