---
title: Running SDXL in Python
date: 2024-03-13
categories: [AI, Stable Diffusion, Python]
tags: [AI, Stable Diffusion, Python, How-To, Setup]
---
- [Introduction](#introduction)
  - [Ways to Use Diffusion](#ways-to-use-diffusion)
  - [Why Code?](#why-code)
    - [Flexibility](#flexibility)
    - [Learning](#learning)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [DiffusionPipeline or StableDiffusionPipeline](#diffusionpipeline-or-stablediffusionpipeline)
- [Code](#code)

# Introduction
## Ways to Use Diffusion
We're lucky to have quite a few options for running [diffusion models](https://arxiv.org/abs/2006.11239) to create images. From beginner level abstractions, to graphical interfaces, to writing code, we have many options for how we choose to interface with a latent diffusion model.

Beginner users trend towards services like [DALL-E](https://openai.com/dall-e-3) or [Midjourney](https://midjourney.co/), which offer online interfaces to abstract away any complications with the model. While this makes them as easy as to use as typing what you want to see into a chatbox, it takes away the users ability to tweak the parameters that the model has exposed.

Because of that, users looking for a little more control will tend to make the step to using user interface tools like [AUTOMATIC1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) or [ComfyUI](https://github.com/comfyanonymous/ComfyUI) which operate as graphical wrappers around [stable diffusion](https://arxiv.org/abs/2112.10752) models. These provide all kinds of configuration options for users to play around with to generate exactly the image they were hoping for. They also give access to all kinds of powerful plugins for things like [inpainting](https://arxiv.org/abs/2201.09865). 

Finally, users can use python or other programming languages to run diffusion models.

## Why Code?
This brings us to the question, why would you use code to run diffusion models when you're able to get nearly the same level of configuration from a graphical user interface (GUI) tool? The answer isn't a straightforward one, and the reality is that for most basic (and even some advanced) cases you'll probably have an easier time using a GUI. But there are some strengths to code that cannot be replicated elsewhere.

### Flexibility
As is generally the case between code and GUI's, code provides a level of freedom that a GUI simply cannot give. There are just too many different ways these tools can be used, the GUIs can only provide the most common paths. But what if you want to generate an image 10 times, each with a slight tweak to the input text, using a different sampling method. With a graphical tool this would either be impossible, or require alot of configuration to accomplish. Using code though, it's as simple as a for loop.

### Learning
It is one thing to play around with different configuration and see what they do, it's a whole other thing to do it in code. HuggingFace's implementation specific pipelines provide documentation that directly reference the papers that created the underlying models (Such as their [StableDiffusionXLPipeline](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/stable_diffusion_xl)). There is no better way to get an understanding of a diffusion model than by playing around with it in code. 

This tutorial will show you how configure and use stable diffusion, specifically [stable diffusion XL base 1.0]( https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0).

# Prerequisites
  - [VSCode](https://code.visualstudio.com/)
  - [Python](https://www.python.org/downloads/)

# Setup


# DiffusionPipeline or StableDiffusionPipeline
# Code