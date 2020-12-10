---
title: "4916a W21 Episode 1"
description: ""
date: 2020-12-08T00:10:51+09:00
draft: false
weight: -4
author: "Shawn Graham"
---

Transcript of this week's podcast episode.

### Part One

When I was a kid, I lived in the hinterland of Ottawa. One year, when I was in elementary school, I got selected to go to Ottawa to hear Marc Garneau speak at the Science and Technology Museum - he had just returned from his first mission on the space shuttle. It was very exciting. After the talk, I got separated from the rest of the group. I was completely lost, completely overwhelmed, and utterly bewildered. So much stuff! They found me, apparently, in the gallery devoted to computers.

Seems like I've been a nerd for a very, very long time.

\[ music \]

Welcome to DHMuse! This course is my attempt to understand the landscape of cultural heritage informatics, especially here in Ottawa. I'm glad you've decided to join me in this attempt. How do museums and other organizations in the ‘GLAM’ sector (galleries, libraries, archives, museums) keep track of their collections? To what purpose? What might happen if we release these collections into the wild (via the internet)? If we mash these collections together what might we see, and why might it matter? Where are the dangers - and to whom could it be dangerous?

Now, my background is not in museums. You might say, it's museum-adjacent. I'm an archaeologist by training and there is of course a natural connection there between archaeologists and museum curators.

\[ clip of Indiana Jones; \] It belongs in a museum!

But I'm also the official digital humanities guy, the official digital historian, the digital archaeologist, in the department. So I've been trying to learn how all of these different fields intersect, especially with material culture, the _things_ of history. That is, I think I'm working maybe in 'cultural heritage informatics'. I hadn't even heard the term until oh around six or seven years ago when I saw Ethan Watrall, an archaeologist at Michigan State University, using it to describe a training programme he'd developed for his grad students.

Cultural Heritage Informatics. I *like* it. It seems to me that the intersection of digital history, material cutlure, museums, galleries, libraries and archives might be found within the broader field of ‘cultural heritage informatics’. Cultural heritage materials require careful description and organization to permit effective curation, preservation, management, and research. You may have heard the term ‘bioinformatics’ before; that field defines itself as

> ‘the interdisciplinary field that studies and pursues the effective uses of biomedical data, information, and knowledge for scientific inquiry, problem solving and decision making, motivated by efforts to improve human health.’ (Kulikowski et al 2012)

…in which case, we could define CHI similarly as an interdisciplinary field studying and pursuing the effective use of cultural heritage data, information, and knowledge for humanistic or scientific inquiry, problem solving, and decision making, motivated by efforts to **improve human welfare**. I added the emphasis there to make an important point. The decisions we make about **information** are necessarily **ethical** decisions. Computers operate by replicating the decisions we make, at enormous speed and scale. The consequences can be unintended and unforeseen, and so we have to begin from an ethical perspective that considers from the outset: who will this harm?

\[ music \]

By now, you've had a chance to look over this course website. The entire course is designed to be asynchronous; I don't know about you, but I could live happily without ever being in another zoom meeting. But just because this is asynchronous, it doesn't mean that we don't have a time table to keep, a schedule to observe.

Each week, there are things that need to get done, in order for us to achieve our goals. By the end of this course, I want you to have built a digital computational notebook that engages with information from one of the galleries, libraries, archives, or museums in Ottawa. It might do an analysis; it might be a creative re-imagining; it might be something else entirely.

We're taking inspiration from the work of Australian digital historian Tim Sherratt, who has built what he calls the GLAM Workbench. We're going to put together a version of this from these notebooks that you will make. Thanks to the Students as Partners Programme, I've also been supported in building this course by Chantal Brousseau, who is doing her history degree with a computer science minor. She is also your classmate and another resource person who can help troubleshoot the tech side of things.

I want to make it clear that you do not **need** to be techy to be successful in this course. I know that everyone comes with different comfort levels. My concern - and how I grade - is that you are open and honest about what has worked and what hasn't, and that you think through the *why* of that. I can't emphasize enough: in tech work, we learn far more from when things break than from things that work the first time. I want you to break things.

It'll be awesome. Trust me.

The first third of this course then will consist of a tune-up of your digital skills. You will also select some materials to explore in more detail, plotting your own adventure through the CHI literature. You'll then prepare detailed annotations of this material to share with everyone else.

Then, in the second third of the course, we will look at those materials, and respond to your annotations: basically, we will have a distributed conversation around this literature.

This will then set us up for the final third of the course where, using our digital skills and grounding the work in the literature we've just explored, you will create the computational notebook. You will also write documentation that situates that notebook, so that someone might understand the value, utility, and possibilities that the notebook allows.

All of these I will bundle up at the end of the course and turn into a website, the Ottawa GLAM Workbench.

Cool, eh?

After you've finished listening to this podcast, read through the syllabus - it's critically important that you do this, since this class is probably very unlike any others you've taken - join the class discord, say hello. Read and start following the instructions for week 1. Sort out a github account (which can be pseudonymous, as long as you let me know what your pseudonym is!). Get the hypothesis account, annotate anything you don't understand or are nervous about in the syllabus and the instructions. You're gonna do great. When life intervenes - and it will - just let me know that something's going on. I don't need to know the details; I trust you. Let me know, and we'll come up with alternatives for you to be successful. There's nothing we can't roll with, if you're willing to trust me.

One last thing - from time to time there will be a course podcast for you to listen to. I have invited a number of professionals to reflect on their work and share that with us, so that you gain perspective from those in the field.

Today, we'll finish off by hearing from Erica Vanden Bosch , Manager of Information Management Services for Ingenium, the Crown Corporation that runs the Science and Technology Museum, the Aviation Museum, and the Food and Agriculture Museum.

### Part Two: Erica Vanden Bosch

Hello, my name is Erica Vanden Bosch and I work for Ingenium, Canada's museums of science and innovation. We're located right here in Ottawa Ontario and we run three national museums: we have Canada Agriculture and Food museum; Canada Aviation and Space Museum; and Canada Science and Technology museum.

What do I do? I'm the manager of Information Management Services and if you don't know what information management means don't worry.  I will do my best to tell you what I do and I'll try and keep it short and sweet. Basically, I'm responsible for the overall management of information and corporate memory at Ingenium. That covers a huge volume and variety of information. There's documentation related to the collection like acquisition proposals, exhibition development plans and programming materials and there's also documentation generated by our internal services such as finance and human resources.

So it's a really broad portfolio. But of course, I don't personally handle each piece of information. We have 200 plus employees from curators to conservation, exhibition to programming, facilities to security. Each of these groups creates, receives, and uses information to carry out their work. My job is to try to impose controls over how the corporation manages its information.

And these controls need to respect any and all requirements that we are subject to. These could be identified in legislation, regulations, policies and countless other sources. So we take into account rules like copyright, information privacy, information security, information disposition, and that's just the name a few areas but the list goes on and on.

So that's me and that's what I do. The next prompt I'm going to address is to describe a moment where the digital aspect changed how I do my job. Well, I actually graduated from Carleton University with my undergrad bachelor of arts in English. I graduated in 2015, so some of you may be able to relate to this if you're a little bit younger- basically when I entered the workforce digital had already made its grand entrance.

So I certainly haven't experienced a digital transformation in the same way some of my colleagues have and it's not that they're haven't been changes. I mean technologies are constantly evolving and we're often undertaking projects that involve changes to our tech. But I would say I learned digital-first.

And as I work, I often find myself looking back at legacy paper versions of a process. Sometimes handling the legacy paper documents that were generated. So I do bounce between worlds but I'm definitely more of a digital-first. And what's clear to me is that digital has so much potential.

It's really inspiring. We can reach so many more people; we can share so much more information and we can give so much more control to our users and we can let them decide how they want to interact and use the materials that we have. I guess I don't want to suggest that digital is an easy solution- there's certainly lots of work to do and there are certainly challenges but we can certainly use digital tools to make cultural heritage more accessible and more inclusive. I think that's kind of my big takeaway - even though it's normal to feel comfortable with the more traditional ways of working, sometimes it's good to push ourselves out of our comfort zones when we know it's for a good cause.

Speaking of digital I'll move to the next point: what's the greatest challenge that I'm currently facing with the digital aspect of my work? I think I struggle to pinpoint one single challenge; to be honest, there are endless challenges, overlapping challenges, and even contradictory challenges where solving one issue seems to somehow aggravate another one.

So I'll just highlight one challenge, and it's the level of tech skills that varies from person to person. And that's both in the workforce with people I work with and it's also with the public that we serve- you know, there are people who are incredibly tech savvy, but there are also people who willingly admit that they're not tech friendly in this slightest even and those groups of people often want completely different things from their tech, you know, tech savvy people want a lot of sophisticated functionality.

And the less tech savvy people just want it to be super simple and of course, you know, that's a binary and it's it's not as simple as that there's a lot of people in between. Either way it's really challenging to have our products, our services, and our solutions accommodate the varying levels of technical skills across these people. So that's I think the single greatest challenge I'd say right now and my advice for that because I don't want to just leave a challenge up in the air would be:

That from your own perspective the best thing you can do is to just to ensure that you yourself have the highest tech skills you can, so that you can understand the tech.

It's really to your advantage to have that technical know-how and the more advanced your tech skills are, it's gonna help you when you're trying to resolve problems with the tech; it's also gonna help you understand what options are feasible when you're developing new solutions, when your working under resource restraints.  I think it'll even help when you're trying to develop new ideas. So that's the challenge and how I would suggest trying to work with it.

Next up: where do I see cultural heritage informatics in the future? To be honest before I can jump ahead to the future there's still so much groundwork left to do a lot of GLAMs still need to do work to make their information accessible and in machine readable formats even just internally and to make sure it's comprehensive and consistent and clean. You know, a lot of us have pockets of content that are available and ready to go but there's a lot of content waiting on the sidelines to be processed and to be prepared. So that would give us a great foundation if we could get that to kind of catch up with us.

And then after that, I hope in the future cultural heritage informatics is more open. And I mean, I understand it can only be 'open' when it's possible and when it's appropriate to release that content, so you know, not not complete openness, but 'conscious openness', deliberate openness and then I also hope that GLAMs continue to collaborate widely. I hope we continue to engage specific groups and communities, especially those that have been underrepresented and I hope we continue to provide opportunities for greater public engagement. I mean, personally, I love seeing crowdsourcing initiatives where the public can explore and contribute to collections. I love 'colab' which is a Library and Archives Canada feature on their website, so if you haven't already, check that out.

So that's where I at least hope that we're going in the future. And last but not least: 'what advice might I give to a student who is interested in the intersection of museums and cultural heritage informatics?'

I'll give three pieces of advice. Number one: just look for opportunities to gain experience and be really open about what those may be, whether that means applying to a volunteer organization, whether that's applying to join an advisory council, whether that's applying for a part-time job, it's an opportunity to gain knowledge skills and networks that can serve you and your professional development.

Advice number two would be to reflect on other skills that you may bring to the table and then think creatively about ways that you can kind of market them. So maybe you have graphic design skills or creative writing skills, maybe you're proficient in another language, my example is I'm a pretty good typer which is a really boring skill! But it's actually given me opportunities that I wouldn't have had otherwise, where I've been asked to take notes at conferences or meetings and I wouldn't have been asked to attend them, except people deliberately asked me because they thought 'oh, you could take notes that would be great' and I got exposure to these meetings really early in my career I guess because of this skill set that I had! So be creative about what skills you bring to the table and how they can help move you along.

And last but not least is just to be flexible and adaptable. Again kind of underscoring this whole idea of just be really open to opportunities, you know, you don't have to have to have your first job in a museum to start working on skills that will serve you in the GLAM arena. Don't discount any opportunities and just make the most of everything that comes your way. So, thank you so much for listening today. Have a great day.
