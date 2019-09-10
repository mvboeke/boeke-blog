---
title: Self-hosting Google web fonts
description: Self-hosting Google web fonts
date: 2013-10-09
tags:
  - code
  - web fonts
layout: layouts/post.njk
image: /img/woff-comparison.png
icon: font-case
---
When using web fonts from Google Fonts, it generally makes sense to take advantage of the files hosted on Google’s CDN. However, there are legitimate reasons to host fonts yourself sometimes. If you need to keep your tinfoil hat on at all times, because your site attracts bad guys, you may not want to take the risk of running code from a third party, even one as respected and august as The Google. That is indeed the case at Braintree, where we decided to host fonts on our own servers.

So we downloaded the TTF files from Google Fonts, and ran them through Font Squirrel’s web font generator to get a bulletproof font stack. Everything looked brilliant on the the Mac, but the font rendering was corrupted on both Chrome and Firefox on Windows.

## All WOFFs are not created equal
![Comparing Google Fonts WOFF files on Windows Chrome](/img/woff-comparison.png)

After much experimentation I tried using the Google-hosted version and it looked correct on Windows. I was puzzled because on both operating systems, Chrome was using the same WOFF file from our server. But with a bit of digging, I found that the Google Fonts API serves a different WOFF file to Chrome/Windows than it does to Chrome/OSX. So I downloaded the WOFF file that Google serves up to Chrome/Windows and added that to our site’s assets. It renders well across all major browsers and operating systems.

The lesson learned here: download the Chrome/Windows WOFF from Google Fonts if you want to host it yourself.

I’m still not clear on why Google Fonts serves up different WOFF files for Windows and OSX. Does anyone out there know the reason for this?

