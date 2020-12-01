---
author: Will Becker
bg_image: images/featue-bg.jpg
categories:
- Modelling
date: "2020-12-12"
description: And its many applications.
draft: true
image: images/blog/razor.png
tags:
- Modelling
- Statistics
title: Occam's Razor
type: post
---

So far in my few posts in this blog I've been writing about indicators. Actually I only started working in indicators around 2015. I found that the topic suits me because it is a blend of statistics/data analysis and qualitative work (writing, conceptualising and so on), and I like things that are not too narrowly focused.

Before that (and still now) I was/am a researcher in sensitivity and uncertainty analysis. Uncertainty analysis is understanding how uncertainties in model inputs affect the results, and sensitivity analysis is a more detailed breakdown of which particular model inputs/assumptions are causing the most uncertainty, and by how much.

These topics, combined with some years of experience working in the European Commission, also led me to be generally interested in modelling. I had direct experience building [engineering](https://www.sciencedirect.com/science/article/abs/pii/S0888327012000866) and [biomechanical](https://www.sciencedirect.com/science/article/abs/pii/S0021929011002570) models in my PhD, and came across many different types of models in the Commission, often used for policy impact assessments.

## What is a model?

First of all, what is a model? Well, as usual there are many ways to divide and classify things, but one distinction is:

* **Principle/process-driven models**: these are models that are built based on understanding the physics or processes behind the system. A simple example is [Hooke's Law](https://en.wikipedia.org/wiki/Hooke%27s_law) which describes how a spring extends under a given load. More complex examples are hydrological models and climate models. In all cases, the model is built based on some encoding of the physics or processes driving the system.

* **Data-driven models**: in these models, the system is treated much like a black box. Instead, we use a set of measured system inputs and outputs, and try to build a statistical mapping between the two. A linear regression is a simple example, but more complex examples are Gaussian processes, neural networks, deep learning and so on. What they have in common is that the modelling simply tries to replicate the input/output relationship, rather than trying to model any particular physical process.

No doubt many people would dispute the nuances of those definitions, but I think that the core concept is solid. However, the two categories are not distinct, and in fact will overlap to some extent. At the end of the day, both categories are a system of equations, and both usually have to be calibrated or fitted in some way. This discussion could go on for a while so let's leave it at that for now.

## Elementary, my dear Occam

Occam's Razor is one of those heuristics that seems to apply everywhere. According to Wikipedia, it can be defined as:

> the problem-solving principle that "entities should not be multiplied without necessity", or more simply, the simplest explanation is usually the right one.

What has this got to do with modelling? Well, everything points to the fact that the simplest model that explains the data/process is the best.

But can I back up that claim? Well let's see. You might have heard of the "bias-variance trade off": this is the idea in statistical modelling (i.e. category 2 of the taxonomy above), there is a balance to be struck between underfitting and overfitting a set of data. Underfitting means that the model is too simple to explain the data/process, whereas overfitting means the opposite: 


Image by <a href="https://pixabay.com/users/clker-free-vector-images-3736/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=33226">Clker-Free-Vector-Images</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=33226">Pixabay</a>