+++
author = "Shawn Graham"
title = "Computational Notebooks Resources"
date = "2020-10-10"
description = "A collection of notebooks and other useful materials"

+++

A list of interesting / useful notebooks and other things

## Basic Skills

We are going to use Jupyter Notebooks in this class. For a global overview of how Jupyter notebooks work and are used in humanities research, see Quinn Dombrowski's lesson in [_The Programming Historian_](https://programminghistorian.org/en/lessons/jupyter-notebooks). The links below go to either live notebooks that you can work through, or guide you through some of the same steps that Dombrowski discusses, but with more detail.

+ Working with the Command Line
  - A walkthrough, by Chantal Brousseau
  - [For Windows](building/command-line-win/)
  - [For MacOS](/building/command-line-mac/)


+ [Introduction to Jupyter Notebooks](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/getting-started-with-jupyter.ipynb); if that link breaks, launch [this](https://mybinder.org/v2/gh/shawngraham/tdm-notebooks/master) and then select the notebook from the list.
    - Courtesy Nathan Kelber and Ted Lawless for JSTOR Labs, CC-BY
    - This notebook introduces Jupyter notebooks and Python for absolute beginners.
    - Going further: Kelber and Lawless have a number of notebooks for working with JSTOR's 'Data for Research' dataset creation service; [find out more here](https://tdm-pilot.org/)

+ [Intro to R & RStudio](building/intro-r-rstudio/)
  - A short walkthrough, by Chantal Brousseau
  - How to use R on your own machine!

+ [Running Jupyter Notebooks on Your Own Machine](https://www.youtube.com/watch?v=10FPoTCcv4I)
  - A walkthrough, by Chantal Brousseau

+ [How to install R in Jupyter Notebooks](https://irkernel.github.io/installation/#binary-panel)
  - Run these commands in the R console (you should be able to find it by searching "R" in your applications)
  - In reference to step 2, you want to install this **system-wide**

+ [Using Git on the Command Line to Keep your Notebook Under Version Control](#)
  - A walkthrough, by Dr. Graham and Chantal Brousseau

+ [How to launch your Notebook in a computational binder online with mybinder.org](#)
  - A walkthrough, by Chantal Brousseau

+ [Introduction to Python](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/python-basics-1.ipynb)

## Retrieve and Visualize Data

### Retrieving data

If the data is already made available on the open web, and it's in a reasonable format (json or csv) then it's not too difficult a task.

+ Loading simple data that you've found online into a Notebook
  - a [walkthrough](#)

+ [Working with Pandas to Manipulate Data](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/pandas-1.ipynb)

+ Using OpenRefine to Obtain Data
  - This tutorial adapts the Programming Historian lesson by Evan Peter Williamson ["Fetching and Parsing Data from the Web with OpenRefine", especially its example 2](https://programminghistorian.org/en/lessons/fetch-and-parse-data-with-openrefine#example-2-url-queries-and-parsing-json).
  - Tutorial link [here](#).

+ Extract Illustrated Pages from the Hathi Trust & Internet Archive
  - This tutorial & associated notebooks are developed from Stephen Krewson's piece for the Programming Historian, ["Extracting Illustrated Pages from Digital Libraries with Python"](https://programminghistorian.org/en/lessons/extracting-illustrated-pages)
  - Try searching for images related to "Ottawa".
  - [Hathi Notebook](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/hathitrust.ipynb);
  - [Internet Archive Notebook](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/internetarchive.ipynb)
  - the json file for the notebooks is in the 'data' folder

+ Retrieve data from a 'datasette'-created API [launch binder here](http://mybinder.org/v2/gh/o-date/open-context-jupyter/master?urlpath=notebooks/retrieving%20data%20from%20a%20datasette%20api.ipynb)
  - note that the 'api_search_url' variable might need to be changed to point to the survey markers datasette or the CARF excavation datasette re Fort Frontenac (see below for url)

+ Scraper. [This notebook](https://dhmuse.netlify.app/notebooks/simple-scraper) adapts [this tutorial on beautiful soup](https://programminghistorian.org/en/lessons/intro-to-beautiful-soup) to work with data from the Museum of History.

+ Working with web archives, a series of notebooks by Sherratt et al [https://glam-workbench.github.io/web-archives/](https://glam-workbench.github.io/web-archives/) (including the Internet Archive, so potentially you might find Ottawa things there.)

+ GLAM Notebooks from [BVMC.Labs 'Inspiring computationally-driven research with the British Library's digital collections'](http://data.cervantesvirtual.com/blog/notebooks/) working with a wide variety of European datasets and archival sources.

+ National Library of Scotland, Data Foundry: [A Medical History of British India](https://data.nls.uk/tools/jupyter-notebooks/exploring-a-medical-history-of-british-india/)

+ National Library of Scotland, Data Foundry: [Edinburgh Ladies' Debating Society](https://data.nls.uk/tools/jupyter-notebooks/exploring-edinburgh-ladies-debating-society/)

### Visualize

+ Visualizing Data with Bokeh & Python
    - This notebook is the one that accompanies the tutorial by Charlie Harper in [_The Programming Historian_](https://programminghistorian.org/en/lessons/visualizing-with-bokeh)
    - You can launch the notebook [here](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/viz-w-bokeh.ipynb); this will let you skip setting up the virtual environment (a way of keeping all of your lego pieces for each task separate so they don't cause conflicts).

+ [Topic Modelling and Creating Interactive Visuals in R](https://mybinder.org/v2/gh/ChantalMB/tm-visualisation/master)

+ There might be useful things in [Hands-On Data Visualization](https://handsondataviz.org); not explicitly about jupyter notebooks, but give it a look.

## Documentation

+ Building an [API with Datasette](/building/datasette-guidance)

+ Building a documentation website with Mkdocs
  - MKDocs is a python module that will turn a folder with markdown documents into a functioning website

## Creativity

For when you're ready/inclined to push things further.

+ [Sonification](https://mybinder.org/v2/gh/o-date/sonification/master?urlpath=notebooks/Intro%20to%20Sonification.ipynb)
  - An overview of how and why you might sonify data

+ [Image Glitching](https://mybinder.org/v2/gh/o-date/creativity/master?urlpath=notebooks/Glitching%20an%20image%20with%20prism%20sorting.ipynb)
  - An overview of why glitching an image might be one way of letting people play with collections

+ [An introduction to 'Processing', a language for quick sketches, visualizations, and artwork](https://mybinder.org/v2/gh/o-date/processing/master?urlpath=notebooks/python%20with%20processing.ipynb)
  - A simple introduction to a language that enables creative expression (Brian Foo, the 'Data Driven DJ' uses processing to make visualizations to accompany his sonifications. See for instance his work, [Lee and Jackson](https://datadrivendj.com/tracks/painters/).)

## Ottawa Datasets

### Galleries
- National scale
  - [Inuit Artists' Print Database](https://www.gallery.ca/inuit_artists/home.jsp?Lang=EN)
  - [Art in Canada to 1930](https://www.gallery.ca/indexartcanada/home.jsp?Lang=EN)
  - [Canadian Souvenir View Albums](https://www.gallery.ca/sva/intro_e.htm)
  - [NGC Database](http://archives.gallery.ca/?lang=en)
  - [Artists in Canada](https://app.pch.gc.ca/application/aac-aic/?lang=en)


### Libraries & Archives
- LAC
  - [Notebook](https://nbviewer.jupyter.org/github/GLAM-Workbench/library-archives-canada/blob/master/lac-naturalisation-1915-1945-harvest-by-country.ipynb) that creates datasets from [LAC Naturalization Records, 1915-1946](https://www.bac-lac.gc.ca/eng/discover/immigration/citizenship-naturalization-records/naturalized-records-1915-1951/Pages/introduction.aspx) --> could likely be repurposed to extract later records as well
  - [Black Loyalist Refugees, 1782-1807- Port Roseway Associates](https://www.bac-lac.gc.ca/eng/discover/military-heritage/loyalists/loyalist-port-roseway/Pages/port-roseway-associates-loyalists.aspx)
  - [Canadian Illustrated News, 1869-1883](https://www.bac-lac.gc.ca/eng/discover/canadian-illustrated-news-1869-1883/Pages/canadian-illustrated-news.aspx)
  - [Canadian Patents, 1869-1919](https://www.bac-lac.gc.ca/eng/discover/patents-1869-1919/Pages/canadian-patents-1869-1919.aspx)
  - [Carleton Papers – Book of Negroes, 1783](https://www.bac-lac.gc.ca/eng/discover/military-heritage/loyalists/book-of-negroes/Pages/introduction.aspx)
  - [Carleton Papers – Loyalists and British Soldiers, 1772-1784](https://www.bac-lac.gc.ca/eng/discover/military-heritage/loyalists/loyalists-british-soldiers-1722-1784/Pages/introduction.aspx)
  - [Immigrants Before 1865](https://www.bac-lac.gc.ca/eng/discover/immigration/immigration-records/immigrants-before-1865/Pages/introduction.aspx)
  - [Immigrants from the Russian Empire, 1898-1922](https://www.bac-lac.gc.ca/eng/discover/immigration/immigration-records/immigrants-russian-empire/Pages/introduction.aspx)
  - [Ukrainian Immigrants, 1891-1930](https://www.bac-lac.gc.ca/eng/discover/immigration/immigration-records/immigrants-ukraine-1891-1930/Pages/introduction.aspx)
  - [Marriage Bonds, 1779-1858 - Upper & Lower Canada](https://www.bac-lac.gc.ca/eng/discover/vital-statistics-births-marriages-deaths/marriage-bonds/Pages/marriage-bonds-upper-lower.aspx)
  - [Open Data](https://search.open.canada.ca/en/od/?sort=score%20desc&page=1&search_text=&od-search-subjects=History%20and%20Archaeology&od-search-format=CSV)

- [City of Ottawa Archives](http://ottawa.minisisinc.com/ottawa/scripts/mwimain.dll?logon&application=UNION_SEARCH&language=144&file=[ottawa_web]NewOPAC\index.html)
  - Offers collections of artworks and items from Ottawa historical museums --> cannot find exportable data, would have to be scraped

- [Canadiana.ca](https://www.canadiana.ca/)

### Museums

- [Canadian Museum of History](https://www.historymuseum.ca/collections/)

- Ingenium Museum Network
  - [Open data](https://ingeniumcanada.org/collection-research/artifact-open-data-set-mash-up)
    - All artifacts in the collection of the Canada Agriculture and Food Museum, Canada Aviation and Space Museum and the Canada Science and Technology Museum
    - Available in XML or CSV

## Misc

+ [Computational Analysis of Catalogue Data with AntConc](https://cataloguelegacies.github.io/antconc.github.io/)

+ Student created datasettes:

   + Survey markers from the CSTM (compiled by Sherwin et al) [https://cstm-demo2.herokuapp.com/cstm-markers/](https://cstm-demo2.herokuapp.com/cstm-markers/)

   + This API makes available some 400 record cards from the CARF excavations of Fort Frontenac in Kingston. http://fort-frontenac-excavation.herokuapp.com/.
