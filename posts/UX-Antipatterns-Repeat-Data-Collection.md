---
title: 'UX Antipatterns: Repeat Data Collection'
description: 'UX Antipatterns: Repeat Data Collection'
date: 2012-12-12
author: Michael Boeke
tags:
  - design
  - antipatterns
layout: layouts/post.njk
icon: redo-alt
---

This is an antipattern I’ve come across many times while working on financial software. It often occurs when a website is trying to present one form that will map to multiple systems, or will be used to replicate a physical form (e.g. a credit application). Few things are more frustrating to a user than having to fill out the same data multiple times. It adds no value, increases the likelihood of error, and causes people to tear their hair out.

For example, let’s take a look at the Active.com signup for the Shamrock Shuffle (a great springtime running race in Chicago). It starts off with just a few questions about my age. Thankfully, it calculates my age for me, based on my birthdate, but it won’t infer that I’m older than 16.

![Asking for birthdate multiple times](/img/repeat_data_collection1.gif)

Repeat data collection
As I get to this next section, they’re asking for my birthdate again. They ask my age again too…except this time they don’t calculate it for me.

![Asking for birthdate again](/img/repeat_data_collection2.gif)

Repeat data collection
Finally, when I get to step three, they ask me one more time if I’m 16 years or older, even though I’ve answered this very question already, and have given them my age and birthdate…twice. Yep, I’m still over 16!

![Asking for birthdate yet again](/img/repeat_data_collection3.gif)

Repeat data collection
This redundancy is particularly frustrating for those of us who make software. We know it’s possible for the software to map one answer into multiple fields. When you have to collect a lot of data from a user, it’s easy to get focused on where the data is eventually going to live (e.g. in a form or another system) but if you want people to complete your form, you have to focus on the user instead.