---
layout: post
title: "TIL: Finding Meetings with Attachments in Outlook 2011 for Mac"
description: ""
category: 'TIL' 
tags: ['outlook', 'calendar', 'search', 'mac']
---
{% include JB/setup %}

I am currently have an ongoing project to go through my MASSIVE Outlook inbox and separate out the wheat from the mountains of chaff. One thing I recently realized is that in addition to emails, there might be useful documents hiding quietly in my old meetings. 

As with a lot of things in Outlook 2011 for Mac, there's no readily apparent way to do this. After poking at every menu option and view button I could think of, I turned to Google. After several failed attempts, I finally came across [this post](http://answers.microsoft.com/en-us/mac/forum/macoffice2011-macoutlook/are-attachments-actually-stored-in-meeting-invites/d3357fee-9b1c-427c-9c3a-ed81252420d0?auth=1) on Microsoft's forums. 

User "sturtus" has our answer:

> 1. Highlight the search field to enable the Search tab in the ribbon.
> 2. choose Advanced
> 3. Filter for "Item Contains"
> 4. Filter for items containing the text "cid:" (no quotes)
> 5. This will find any calendar items containing attached documents

Obvious!

Thank you sturtus, whoever you are. You are one the internet's unsung heroes.
