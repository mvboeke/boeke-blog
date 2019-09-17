---
title: 'UX Antipatterns: Splitting Numbers'
description: 'UX Antipatterns: Splitting Numbers'
date: 2012-11-12
author: Michael Boeke
tags:
  - antipatterns
  - design
layout: layouts/post.njk
icon: phone
---
When collecting a US phone number on a web form, it has become convention to collect it with three separate fields. This is meant to help the user successfully input the number in the format the server will accept. Since the user may think of the phone number as one piece of data, rather than three distinct items, many sites employ a feature that jumps the cursor to the next field as soon as it is filled with the expected numbers of characters.

Split phone number
This will totally screw up a user like me, who is used to powering through web forms by hammering the tab key as soon as I complete a field. Which leads to the unfortunate situation illustrated below.

The good folks at Southwest Airlines have tried to help me by moving my cursor to the second field in the phone number, but I’ve already hit the tab key. So I’ve skipped the second field entirely and gone straight to the third. Doh. Hence, an antipattern.

Luckily, we are living in a grand age of Javascript wizardry. We can now format phone numbers on the fly with plugins like jQuery Format Phone or Masked Input Plugin. We can just let the user enter the number into the field naturally, including or not including special characters as they wish, and format the number for them as they type. The end result might look something like this.

Auto-formatted phone number
This particular antipattern shows up in more situations than just phone number fields. Social Security Numbers and other places where sites collect numbers that include dashes or other formatting are prone to fall into the same trap.

A single field is more natural for a user, and utilizing Javascript to format the field as the user types will ensure that it is formatted as expected for both the user and the server.