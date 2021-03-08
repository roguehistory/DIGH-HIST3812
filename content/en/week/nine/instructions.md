---
title: "Building"
description: "in which perhaps the rubber meets the road"
date: 2020-01-28T00:10:37+09:00
draft: false
weight: -10
---

> in which we begin to put into practice what we have heard and read and discussed

Let's make some magic!

### Goals for this week

1. Discover the landscape of GLAM data in Ottawa
2. Build your first notebook

### Listen

<div align="center"><iframe src="https://anchor.fm/dr-graham/embed/episodes/Episode-5--the-one-where-we-start-building-things-es13ab" height="102px" width="400px" frameborder="0" scrolling="no"></iframe></div>

Given the data we're working with this week, make sure to listen to this interview with Kristy von Moos of Ingenium.ca!


### Do

1. Launch [this notebook](https://mybinder.org/v2/gh/shawngraham/dhmuse-notebooks/master?urlpath=notebooks/viz-w-bokeh.ipynb) and use it to follow along the Programming Historian Tutorial on visualizing data [located here](https://programminghistorian.org/en/lessons/visualizing-with-bokeh) using the data provided. You can skip to the 'Bsics of Bokeh' section.
2. Once you've finished that, save a copy of the notebook with a new name, and then modify the notebook with new data. Ingenium, the corporation that runs the Canadian Science and Technology Museum, the Aviation Museum, and the Agriculture Museum, makes a large variety of data available in a csv file. If you are running Jupyter on your own machine, you can download the CSV FILE from [our website](https://dhmuse.netlify.app/data/cstmc-CSV-en.csv)), and save that in a new folder.
  + Using the notebook from step (1), change the `df.read_csv("")` command to read the data into a 'dataframe'. If you're working on your own machine, you'll put the file path to the data between the quotation marks. If you're working **online** you can load the data directly from the mirror'd copy I put on the course website with `df = df.read_csv("https://dhmuse.netlify.app/data/cstmc-CSV-en.csv"`. **If you're running the notebook online and loading the data from the course site, it will take a few moments for it to load into memory.**
  + **protip** once you've loaded up data and passed it to the variable `df` you don't have to load it up again - so in subsequent cells of the notebook, use the `#` to comment out anywhere the cell says `df = pd.read_csv` etc, as you've already done that.
  + There's a lot of data in this dataframe ([here are some examples on how to filter rows](https://www.geeksforgeeks.org/ways-to-filter-pandas-dataframe-by-column-values/) by the way). Add a new code block after the the one with `df.columns.tolist()` by making sure it's the highlighted block (click on it) and then hit the `+` button. (This code block by the way shows us all of the possible columns we might want to subset our data by). In that new code block, let's filter the records to just show us items that were manufactured in Ottawa and Kingston. We'll create a list of the things we're looking for (Ottawa and Kingston), and then we'll create a new dataframe called `ottking_df` by checking the original `df` for anytime our search options are in the column `ManuCity`:

  ```
  # let's now filter the dataframe to items created in Ottawa and Kingston
    options = ['Ottawa', 'Kingston']  

    # selecting rows based on condition  
    ottking_df = df[df['ManuCity'].isin(options)]

    print('\nResult dataframe :\n',
      ottking_df)
  ```

  + Then try to visualize some dimensions (columns) of the data (which dimensions do you think?); change the labels appropriately too. Hint: you won't run your visualization on the original `df` dataframe. Save copies of your outputs. Anytime you see 'df' in the original code, make sure you've changed that to the data you're actually working with. (Hint: in the block called 'The Bokeh ColumnDataSource, change the `sample = df.sample(50)` to `sample = ottking_df.sample(500)`'. The `.sample` means to grab a certain number of rows of your total data.)
  + Try to modify some of the other visualization code blocks. Share your code in the course discord space, especially when you run into trouble.
  + Can you spot anything interesting about the collections data as a result of your visualizations?

3. Using what you know (draw on other notebooks you've seen), can you build some other visualizations of either the demo data for the Programming Historian tutorial, or the CSTM materials, or other GLAM materials in Ottawa (see [Ottawa Datasets](https://dhmuse.netlify.app/building/technotes-toc/#ottawa-datasets))?

Save your notebooks to your own computer, and then lodge a copy of them in your github repository for safekeeping.

{{< notice success "Important" >}} With tech work, if it doesn't come together in about 30 minutes, it won't come in an hour. So take a break. Close the laptop. Call somebody up for help. Find another pair of eyes to look at the problem. I don't want to hear that you labored heroically for 2 hours to do something. Jump into our social space and ask for advice.
{{< /notice >}}

### Log your work

For your digital work, it is critical that you keep notes on what works, what doesn't, what error messages you received, what help you received from others, what websites you went to, and so on.

Create a repository on Github; you can make it private.

Make a text file and call it `journal.md`. Put the date in it, write brief notes so that when you come back to all of this, you'll know what you were doing.

Drag and drop this file, and any other supporting materials you wish, onto your repository; once they've uploaded, hit the 'commit' button.

Share your repo in our Discord space if you want me or someone else to have a look if there are problems - or victories!

**While this isn't graded, per se**, you _will_ need this material when it comes to writing the documentation for your eventual GLAM notebook you create. Get in the habit of keeping careful _process_ notes.
