---
title: 'Eleventy and Netflify are my new jam'
description: 'My experience rebuilding my website with Eleventy and Netflify'
date: 2019-10-02
author: Michael Boeke
tags:
 - Code
layout: layouts/post.njk
icon: boombox
---

I recently found myself in the job market for the first time in a while, and it was just the kick I needed to embark on a long-overdue overhaul of my website and blog (the very one you are reading).

I'm not new to the JAMstack - I previously used Middleman as my static site generator and hosted it on Github pages. Middleman is great but one of the reasons my site went stale is that Ruby is such a time-suck. I've burned entire evenings wrestling with Ruby versioning without getting to a working environment. So, when I started seeing lots of good things about Eleventy paired with Netflify in my corner of Twitter, I decided to give it a try.

## Getting Started with Eleventy
I still had to sort out Node versions, but it only took a few minutes even though I'm relatively new to the Node-iverse.

![Eleventy screenshot](/img/eleventy_screenshot.png)

Eleventy has a bunch of example projects, which is helpful, but it can be hard to tell what's going to be most relevant. I started with Hylia because it looked the most mature but it was way more complicated than I wanted. So, I started over with Eleventy blog base and that was much closer to what I needed. I understood the organization and live updating on the server worked well. It's still a version 0.x project, so there are some rough edges. For one thing, documentation could be better, and some of the helpful utilities included in Middleman aren't present. But overall, it hits the sweet spot for someone with my modest level of technical skill. And by modest, I mean a website creator who's comfortable with HTML, CSS and template languages, but doesn't write much javascript. Better yet, Netlify can also help avoid the hassles of network and server configuration, as the base blog project works with Netflify right out of the box. That's handy because...

## Netlify is amazing

I didn't know what to expect from Netlify but I followed the prompt from the Eleventy Base Blog project and it led me to the wonderfully intuitive Netlify onboarding experience. You log in to Netlify with your Github credentials, select a repo, and it publishes your Eleventy site to the web.

That trick of automatic deploys is central to the Netlify experience. Anytime you commit to master in your Github repo,  Netlify deploys the site. Even better, Netlify automatically creates a preview version of your site when you create a PR on a branch. That's super convenient when you want someone to read a blog post before you publish it.

![Netflify screenshot](/img/netlify_screenshot.png)

Snippet Injection: I don't have a lot of third-party scripts on my site, but this feature is great for analytics. It adds scripts to the <head> element when the page is served, which enables you to keep analytics scripts in your dev environment from inflating your visitor counts.

Custom domains are easy to set up, too. I just had to update the DNS name server settings at my domain registrar and Netflify took care of the rest. The same was true for SSL; no need to mess with certs, Netlify just added it automatically. This process did have one snag - it took a full day for DNS changes to propagate and during that time it was unclear to me whether there was an error with my DNS an SSL or if I just needed to wait. It all worked out in the end, but it was the notable exception in an otherwise fantastic experience.

Oh, and did I mention this is all available for free? Not to sound like an infomercial, but this is a fantastic deal and I'm excited about it.

Conclusion
If you're making a blog site with a static site generator, Eleventy is pretty great. If you are hosting and deploying websites of any kind, Netlify is amazing. Both of these will be my go-to technologies for the foreseeable future.