---
title: My Analysis
layout: default
---

# My Analysis
## A Search for a Dark Matter Candidate with the CMS Experiment at the LHC

**under development**

### A Note from Sam:
Hello friend. This section is of course going to get pretty technical. If you are interested in the details feel free to dive right in and absorb as much as possible. If you are more interested in the pretty pictures that is perfect too! 
The goal of this page is so when I show the real plots at my Preliminary Exam, Thesis Defense, or on a future paper (fingers crossed) you will recognize them! Per usual, please send me your questions and happy reading!



We know the Standard Model has a few missing pieces. One of the most interesting of which is **dark matter**. We don't yet know what dark matter is, but we do know a few things about it.
1. It has mass and thus experiences gravity
2. It is not electrically charged and does not interact with light
3. It is stable and long-lived

From these clues theorists can make guesses as to what dark matter might be. We experimentalists then can go searching through our collision data to try and find the theoretical particle.
Below I describe what this elusive search looks like at the CMS Experiment.



## Step 0:
### The Theorists Tell Us Their Guess
One idea for dark matter is the existence of a "dark sector". This means that the Standard Model particles we know and love would have dark 

![Dark Sector](../images/darksector_handdrawn.jpg)



## Step 1:
### What Would The Particle Look Like?
In order to look for the particle, we need to model what it would look like inside of the CMS Detector. To do this we create computer simulations to model the particle inside our detector. We call this the <span style="color: blue; font-weight: bold;">signal</span>. This is what we will go searching for. Everything else we call <span style="color: grey; font-weight: bold;">background</span>. 

What something "looks like" in particle physics is described by its physical characteristics. These include things like its mass, its energy, its speed, its path, etc. The important part of the analysis is finding characteristics that look very particular to the <span style="color: blue; font-weight: bold;">signal</span> we are looking for, and thus can distinguish it from the <span style="color: grey; font-weight: bold;">background</span>. 

In order to "look" at the signal and the background we make histograms of each characteristic. It is the distributions we are interested in and what will help us describe and find the signal we are looking for.

Sometimes the distributions are very different, and sometimes they are very similar. If there are a few characteristics that are very distinguishing we can simply grab all events in a particular region, as we are confident most of them will be the signal we want. 
For example, maybe your signal has a mass that is only ever 125 while your background comes in a range of masses. Then you might make a plot of the mass of everything you see and the result would be something like this:

![Higgs Bump Hunt](../images/Higgs_BumpHunt_Plot.png)

This is how the Higgs Boson (mass of 125GeV) was discovered at the LHC in 2012. 


In this analysis, there are no characteristics that are so clear. So instead we use a tool called a **Neural Network**. This tool takes in as many characteristics as we want, and instead of making simple cuts on characteristics it will instead learn from all of the characteristics at once! It will then output a score on a range from background-like (0) to signal-like (1). Then we can instead grab the region of this score where we are confident there is a lot of signal.

![Neural Networks](../images/GNN_handdrawn-9.jpg)


Here are a few examples of what these histograms of characteristics might look for <span style="color: blue; font-weight: bold;">signal</span> and for <span style="color: grey; font-weight: bold;">background</span>. Notice some distributions look very different between <span style="color: blue; font-weight: bold;">signal</span> and <span style="color: grey; font-weight: bold;">background</span>, and some look very similar. Then notice how different they look after the Neural Network has scored them! Thanks Neural Network!



