---
title: 'How to get designers to make your open source project awesome'
description: 'How to get designers to make your open source project awesome'
date: 2012-09-16
author: Michael Boeke
tags:
  - design
  - open source
layout: layouts/post.njk
icon: hand-sparkles
---

Like many designers, I use open source software, believe in the open source ethos, and would love to help make open source software look better and be easier to use. A lot of open-source projects are focused on the back-end, and don’t require a ton of UI/UX design, but it seems that there are more web apps popping up these days.

I had the good fortune to get involved with the Brainiac project recently, and wanted to share some of the hurdles I faced as a designer getting involved in the project. If you can address these things on your open source project, you stand a much better chance of getting designers and front-end developers to contribute.

### Make it easy to install
A lot of designers can hack CSS and HTML, and even work with layouts in various frameworks like Rails. However, to start working with those parts of your app, they have to get the entire thing to boot up locally. Make it easy, and offer step-by-step instructions. When I started working on Brainiac, I asked a developer “How do I get this running?”, to which he replied “oh, it’s a Leiningen app”. That didn’t mean anything to me, and left me feeling embarrassed about asking further questions. What I really needed was for him to lay out the handful of steps necessary to get the server running locally. I did get these for Brainiac, and then I added them to the project’s readme.

### Be a Pal
If a designer takes an interest in your project, be a friend. Help them with technical issues. Figure out which dev tasks are blocking them. Great product companies have designers working side-by-side with developers to collaborate. When the designer or front-end dev gets stuck on something technical, they can call on a more-technical developer to help them get unstuck. I can see how this is tricky for highly distributed development projects, which brings me to the next point.

### Keep Discussions Accessible
Use GitHub Issues for project discussions. This will keep discussions accessible to everyone, which is important, because designers need a channel for requesting features and posting comps. IRC WTF? That was my reaction after downloading the very cool Brackets project, and attempting to contribute. Their thorough installation instructions made it a breeze to install, but their project readme directed me to Freenode’s home page for Q&A. From there, I had no idea how to get onto the #brackets channel. Even though I’m aware that IRC is for chat, I wasn’t sure if I needed a client program or if it should work in my browser, and lost interest before I spent the time to figure it out. More explicit instructions for how to get going on the #brackets IRC channel would have helped here.

### Make sure your views don’t require a CS degree to edit

Designers are getting more technical all the time, but you still need build your app in a way that takes designers into account. HTML, CSS, and (to a lesser extant) Javascript are the lingua franca of UI design. There’s certainly nothing wrong with working some SCSS into the mix, but when you start using using a lot of the backend programming language (i.e. Ruby/Java/Clojure) in your views, you’re turning a markup exercise into a programming excercise. You’ll lose a huge chunk of potential contributors, right out of the gates. Even the ones who soldier on and try to learn the language will find themselves stuck often. If they don’t have a pal (see above) they are likely to give up.

### Wrapping up

My first foray into open source software development has been tremendously gratifying. Despite a hitting a few roadblocks, I’ve learned a ton, and have helped a great new product enter the world. I’m looking forward to continuing my involvement with Brainiac, as well as finding new projects to work on.

I’m interested in hearing from anyone who knows of projects that have done a good job engaging with designers, and I would love to hear from other designers who have waded into the open source world. Please comment below, or find me at michael@michaelboeke.com or @mvboeke.