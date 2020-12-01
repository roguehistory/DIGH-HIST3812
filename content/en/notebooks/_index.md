---
title: "Notebooks"
description: "Some Demo Jupyter Notebooks"
date: 2020-01-11T14:09:21+09:00
draft: false
---

#### A memo to self- how I import to the website

I turn them into markdown for display here by running the following jupyter command:

```
jupyter nbconvert --to html <NOTEBOOK_NAME>.ipynb
```
and then put the html in the same folder as the page, with the following html

```html
<iframe
      src="./<CONVERTED_NOTEBOOK_FILENAME>"
      width="90%"
      height="1000px"
      style="border:none;">
</iframe>
```

## Demo Notebooks
