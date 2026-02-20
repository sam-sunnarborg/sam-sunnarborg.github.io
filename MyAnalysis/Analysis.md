---
title: My Analysis
layout: default
---

# My Analysis
A search for a dark matter candidate at the CMS Experiment

We know the Standard Model has a few missing pieces. One of the most interesting of which is dark matter. We don't yet know what dark matter is, but we do know a few things about it.
1. It has mass and thus experiences gravity
2. It is not electrically charged and does not interact with light
3. It is stable and long-lived
From these clues theorists can make guesses as to what dark matter might be. We experimentalists then can go searching through our collision data to try and find the theoretical particle.
Below I describe what this elusive search looks like at the CMS Experiment.


## Step 0:
### The Theorists Tell Us Their Guess
One idea for dark matter is the existence of a "dark sector". This means that the Standard Model particles we know and love would have dark 

## Step 1:
### What Would The Particle Look Like?
In order to look for the particle, we need to model what it would look like inside of the CMS Detector. To do this we create computer simulations to model the particle inside our detector. We call this the "signal". This is what we will go searching for. Everything else we call "background". 

What something "looks like" in particle physics is described by its physical characteristics. These include things like its mass, its energy/momentum, its path, etc. The important part of the analysis is finding characteristics that look very particular to the signal we are looking for, and thus can distinguish it from the background. 
In order to "look" at the signal and the background we make histograms of each characteristic. It is the distributions we are interested in and what will help us describe and find the signal we are looking for.
Sometimes the distributions are very different, and sometimes they are very similar. If there are a few characteristics that are very distinguishing we can simply grab all events in a particular region, as we are confident most of them will be the signal we want. In this analysis, there are no characteristics that are so clear. So instead we use a tool called a Neural Network. This tool takes in as many characteristics as we want, and instead of making simple cuts on characteristics it will instead learn from all of the characteristics at once! It will then output a score on a range from background-like (0) to signal-like (1). Then we can instead grab the region of this score where we are confident there is a lot of signal.

![Neural Networks](../images/GNN_handdrawn-9.jpg)

Here are a few examples of what these histograms of characteristics might look for signal and for background. Notice some distributions look very different between signal and background, and some look very similar. Then notice how different they look after the Neural Network has scored them! Thanks Neural Network!



