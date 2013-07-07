---
layout: post
title: "up to eleven"
date: 2013-07-07 17:31
comments: true
categories: 
---

I did a number of things for my most recent client, around automation and the build pipeline. I introduced them to the notion of using [Puppet](http://puppetlabs.org) to help them provision boxes, and I formulated an idea for a more complete build pipeline. All in all, their build pipeline isn't half bad. They use Jenkins to run unit tests, build artifacts and push those artifacts to a Nexus repo, or to Spacewalk/RHN Satellite. But I, and one of their engineers, thought it could be better.

What if, we thought, we could not only run our standard tests automatically, but also bring up the actual software deployment in a virtual machine, and run an automated acceptance suite? What if, once this had happened, the software was packaged up nicely and pushed to other channels in Spacewalk, for deployment to UAT? What if we could deploy some stuff straight to production? We had ideas.

Then I remembered my previous client, a startup, who hired me to kickstart the development of one of their products. I went in and there was literally nothing there, just some designs, and BitBucket and Rackspace accounts. I hand-whittled servers together, the build processes, the single-click deployment scripts and such-like, all the while wishing I could get it done faster. 

So with this in mind, I've decided to prepare myself for the next time someone hires me to get their greenfield project off the ground. I've started building the 'Up to Eleven' stack, which aims to give me exactly what I wish I'd had before. Everything I need to check out code, build it, test it, deploy it to live, with the minimum of fuss. I look forward to keeping this blog up to date with progress on it.