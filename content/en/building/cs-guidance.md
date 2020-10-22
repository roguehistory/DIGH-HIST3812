+++
author = "Dr. Graham"
title = "Guidance for your Case Study"
date = "2020-02-02"

+++

## Your Case Study Is Due Before the End of Week 12

You will have submitted the link to your Jupyter Notebook at the end of week 9. If all goes according to plan, I will have bundled these altogether into a supporting website, the Ottawa GLAM Workbench ([fyi, repo here](https://github.com/XLabCU/GLAM-Ottawa)) and used the [My Binder](https://mybinder.org) service to make these live online, by the end of week 10. This gives you 2 weeks to create a 'case study' document that can then be integrated into the workbench.

## Goal

The goal here is to create a kind of guide to a selected notebook that shows what the notebook can do. **It walks the user through the notebook, how to use it, perhaps visualize results or ways to extend it, in order to suggest questions a user might want to pose, and why it might matter.** That last point is the most 'case study'-ish bit. By providing guidance on the 'so what' question, you will engage with the literature or issues and provide context for non-dh-minded folk should take this work seriously.

### Parameters

1. A single markdown page with footnotes.* You should have a proper text editor like [Sublime Text](https://www.sublimetext.com/) or [Atom](https://atom.io/) installed; compose your document using the text editor.

Footnotes can be formatted in markdown like so:

`Footnotes[^1] are added in-text like so ...`

and then at the end of the document, like this:

```
[^1]:
Graham, S. 2006. _Ex Figlinis_. BAR International Series: Oxford.
```

{{< alert theme="info" >}}
*It is possible to make an online slideshow out of a markdown document. You might wish to format your document that way. If you do, use this [template on the HackMD platform](https://hackmd.io/tPo_MRQmRjSRBD6O7yKNfw?edit=&template=0f4505d1-db3c-4abf-94ad-471a14425f26#). You can log in with your Github username. Copy it into your text editor; make your edits in your text editor and save locally. When you're ready to test, paste it all into a new note on HackMd, then 'view in slideshow mode' under the sharing button. You can then submit the URL to the slideshow mode version.

The two slide shows on the [Glam Workbench main page](https://glam-workbench.github.io/) are generated this way.
{{< /alert >}}

---

2. Use clear headings and header levels to signal a clear, logical, flow.

---

3. Be succinct.

---

4. Illustrate. Create screenshots & illustrate these with arrows, circles, etc to make it clear what's going on. On a Mac, you can use cmd+4 to take a screenshot, and then the preview app to annotate it. On a PC, the snip-it tool can be used the same way. Change the names of the files to `your-surname-fig-1.png` (or .jpg, as appropriate) and so on, so that I don't lose track of things. Insert images into your document with markdown: `![alt-descriptive-text](your-surname-fig-1.png)`.

---

5. Video walkthroughs can be helpful too. I use the free version of https://screencast-o-matic.com/ . The resulting file can be saved on your computer and then placed in your repository; it can also be uploaded to your userspace on screencast-o-matic and then can be embedded from there. If you load it to your own repo, just use `~insert video 1 here~` and I'll do the rest when I compile everything. Otherwise, use the embed code from screencast-o-matic. Mac users can also make quick videos using cmd+5; Windows 10 users can use the x-box app screenrecorder (press Windows+G) ([more info](https://www.theverge.com/2020/4/21/21222533/record-screen-pc-windows-laptop-xbox-game-bar-how-to)).

---

6. Provide a link to launch the binder in a live environment.

---

7. Full and accurate citations in a 'References' list at the end. Chicago style is fine.

---

8. Remember to address the goals for this exercise. The most important of these: the 'so what?', also known as the 'what's in it for me?'.
