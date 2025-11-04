---
layout: distill
title: The Super-Human Touch: An RL Research Story 
description: The story of my first PhD publication
tags: rl tactile dexterity ssl
giscus_comments: true
date: 2025-11-04
featured: true

authors:
  - name: Elle Miller

bibliography: 2025-11-04-tactilerl.bib

# Optionally, you can add a table of contents to your post.
# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
toc:
  - name: Equations
    # if a section has subsections, you can add them as follows:
    subsections:
      - name: Example Child Subsection 1
      - name: Example Child Subsection 2
  - name: Citations
  - name: Footnotes
  - name: Code Blocks
  - name: Interactive Plots
  - name: Layouts
  - name: Other Typography?

# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
_styles: >
  .fake-img {
    background: #bbb;
    border: 1px solid rgba(0, 0, 0, 0.1);
    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
    margin-bottom: 12px;
  }
  .fake-img p {
    font-family: monospace;
    color: white;
    text-align: left;
    margin: 12px 0;
    text-align: center;
    font-size: 16px;
  }
---

The purpose of this blog post is three-fold: to chat about the **major findings** (including some interpretations too uncertain for the paper), to share the **human side** of the story, because our brains work in narratives, and to highlight the most important **lessons** I learned about doing useful RL research.

Let’s go!

## Part 1: Human Side to the Research

### 1.1 Why Study Tactile RL?

This research kicked off my journey into Reinforcement Learning (RL) as a first-year PhD student. My background was all over the place: assistive robotics (DLR), semantic perception (JPL), and even astrophysics. I had *zero* prior experience in RL, but I thought it was the most compelling form of robot learning, so I was determined to study it.

I was immediately drawn to learning from **tactile feedback** because of the ultimate goal I had in mind: **physical human-robot interaction**. My interest in robotics stems from the belief that they can dramatically improve the quality of life for many people as physical assistants (less so to just do my laundry, though that’d be nice).

However, being up close with full-size robots was quite scary for me; it took some serious getting used to. This is me in 2022 as a Bachelors student, pretty terrified to go near the robot and standing way out of the way…
![image.png](attachment:19a40e50-81d1-42a1-889a-0254fa1edf25:image.png)
…to me this year in Japan, happy for a robot to squeeze my torso and lift me up 

<aside><p>(still a bit scary but ok!)</p></aside>

![image0.jpeg](attachment:a21ec868-93a3-4aa0-8879-a5d839d91eec:image0.jpeg)

I was comfortable with this robot (named AIREC) lifting me up because it was controlled with **impedance control**. That means it could actually modulate its motion based on the torques placed on the joints. **AKA, it could feel me.**

However, most robots who learn policies with RL cannot “feel”. They're typically controlled via joint position commands (**position control**). For observations, they know where their body is (**proprioception**), and they might be given the exact pose of the object (**ground-truth information**) or a camera stream (**vision**).

For instance, one of the biggest and most cited works in RL for manipulation—from OpenAI in 2020 <d-cite key="openai2018learning"></d-cite> —made a very specific design choice. To quote the paper:

> “We give the control policy observations of the fingertips using PhaseSpace markers and the object pose either from PhaseSpace markers or > the vision based pose estimator. Although the Shadow Dexterous Hand contains a broad array of built-in sensors, we specifically avoided 
> providing these as observations to the policy because they are subject to state-dependent noise that would have been difficult to model in > the simulator.”



<!-- 
Colons can be used to align columns.

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |   centered    |   $12 |
| zebra stripes |   are neat    |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| _Still_  | `renders` | **nicely** |
| 1        | 2         | 3          | -->

<!-- > Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a _separate paragraph_.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the _same paragraph_. -->
