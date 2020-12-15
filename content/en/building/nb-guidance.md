+++
author = "Dr. Graham"
title = "Guidance on Building your own Notebook"
date = "2020-08-02"
description = "Expectations for content and format"
+++

![](images/paper-notebook.png)

## Goal

The goal of your notebook is to produce a computational document that engages with GLAM data from Ottawa. It would be helpful - but not required - to coordinate with your peers so that we have a wide variety of final notebooks. But even if two people created notebooks working with the same data, you would in all likelihood go about it in different ways, and so a user/reader would still learn from your example.

The notebook should do something _meaningful_ with the data, with two examples of 'something meaningful' within a single notebook, from the same data source:
+ What constitutes a 'thing'? It could be a visualization of a certain subset of information. It could show how to map the material. It might make the material more easily available. It might do some sort of creative remixing. Other things are possible. See the [examples in the wild](/building/technotes-toc).
+ What constitutes 'meaningful'? Well, that's an argument you would make in full in your [Notebook Reflection](/building/cs-guidance). But you'd also include a briefer indication within your notebook as well, summarizing what the notebook will do, what data it will work with, and where a user/reader might like to expand or change things or push further.


## Requirements

1. The notebook will have the following subheadings
  - `Introduction` ~ This section will introduce your goals for the notebook, and briefly situate what your notebook does and why it matters.
  - `Data` ~ This section will discuss the source of your data, is strengths / limitations, and will include the necessary code to load the data up. The discussion here may be brief; you will want to address the same questions in more depth in your Notebook Reflection.
    - It may well be that you are loading data from some other website; it could be that you've already downloaded, subsetted, and cleaned data from somewhere; in this case, you'd be loading the data from your own github repository.
  - The body of your notebook will have subheadings as appropriate to the tasks you are doing. Each subheading should also include a text block that explains the overall task being done in the section.
  - Code should be commented thoroughly.
  - `Conclusion` ~ This section will summarize what the reader/user has just accomplished, pointing out those points/places where they might wish to expand or modify to work with their own data.
  - `References` ~ Citations & links to anything you used to build the notebook.
  - `Further Readings` ~ links to three resources that will help your reader take your example further or think about it more deeply.

2. Text blocks should be written using Markdown conventions. Here's a [cheatsheet](https://www.markdownguide.org/cheat-sheet/).

3. A copy of your notebook should be kept in a Github repo. This repo may be public or private. If it is private, share it with user `shawn.graham`.

## Other Considerations

1. You should probably be writing the notebook on your own machine, having already installed python and jupyter notebooks locally. You would then lodge copies of your notebook in a repo on Github you've created for the task, as you go. These copies can then be launched using [Binder](https://mybinder.org) for live engagement.

+ Alternatively, you can launch this [demo from Binder](http://mybinder.org/v2/gh/binder-examples/r_with_python/master) which is preloaded with Python and R. It might take a few minutes to launch. You can create a new notebook by hitting 'new' then 'notebook':

![](images/new-notebook.png)

{{< alert theme="info" >}}
Download your work **TO YOUR OWN MACHINE** if you are using an online binder; these can time-out after a certain amount of inactivity. If you just hit 'save', it's only saving on the temporary image at Binder and will be deleted. Hit save, then download from the file menu.
{{< /alert >}}

+ Another alternative: if you have a google account, you can use [the Google colab service](colab.research.google.com/) to create your notebooks. These can be saved directly to your own gdrive or to your github account, as well as locally. Again, this service will time-out so it is important to save your work frequently to your own machine or gdrive. **An advantage** of using Colab is that it will give you access to a GPU, which is handy if you are doing anything computationally heavy, like image recognition.

2. You may wish to collaborate with one of your peers.
+ This collaboration could take the form of co-authoring the notebook and the notebook reflection; in this case, you will also be required to discuss the nature of your collaboration, who did what and why and was this equitable, how you managed conflict, how you organized your time, and what lessons your collaboration might imply for GLAM organizations.
+ Alternatively, you could coordinate your notebooks to work with the same data source to highlight different but complementary aspects. You would then work out an ideal sequence for how the user/reader might engage with the materials. What perspective emerges on the data by using your notebooks?
+ I'm open to other ideas; talk to me.

3. Even if you're not formally collaborating with anyone, **talk about what's working, what isn't, and what troubles you've run into** in our Discord space. Help each other out. Brainstorm. Share. Kvetch. You are under no obligation to do this work in splendid isolation.
