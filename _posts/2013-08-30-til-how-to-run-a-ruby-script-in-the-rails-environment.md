---
layout: post
title: "TIL: How to run a Ruby script in the Rails environment"
description: ""
category: 'TIL'
tags: ['ruby', 'rails', 'command line']
---
{% include JB/setup %}

And now we get to the main reason I set up this blog: To document things that took me quite a bit of time to figure out (*with* Google) in the hopes that my sacrifice saves someone else time down the line.

Today, I was trying to run a Ruby script in my Rails 3 environment from the command line. This proved tricky. Apparently, the main way to do this is 

    > rails runner script_name.rb

That, for Lord Only Knows what reason, isn't working on my Rails install. It worked for my coworker on his box, but not on mine. I'm beginning to see why Rails developers are big fans of Puppet and Chef.

Anyway, the alternative I fell upon was to run the script from the Rails console. Not a 100% solution if you're trying to integrate the script into a bash script or something, but it was enough for me. And here's how you do that:

    > rails c
    Loading development environment (Rails 3.2.13)
    1.9.3p362 :001 > load 'script_name.rb'

At some point, I'll figure out why runner isn't working and I'll post a followup if it's interesting.





