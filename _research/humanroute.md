---
layout: page
title: VLM Capacity and Limitations
permalink: /research/humanroute/
---

# HumanRoute

**How Does Visual Context Shape VLM Assessments of Pedestrian Routes?**

<div class="project-meta">
  <span class="badge">Independent Research</span>
  <span class="badge">Vision-Language Models</span>
  <span class="badge">Street-View Imagery</span>
  <span class="badge">Accessibility Assessment</span>
  <span class="badge">Human-centered AI</span>
</div>

---

## Overview
Pedestrian accessibility is not simply a property of individual locations. A route unfolds through a sequence of environments, and its usability may depend on how these environments connect, where barriers occur, and whose mobility needs are considered.
<br/>
<br/>
Vision-language models (VLMs) offer a way to assess pedestrian environments from street-level imagery. However, evaluating isolated images may overlook information that emerges across a route, while providing more visual context does not necessarily lead to more meaningful assessments.
<br/>
<br/>
HumanRoute investigates how the spatial organization of visual evidence influences VLM-generated assessments of pedestrian routes, with particular attention to visual context, sequential information, and user-specific accessibility needs.

## Research Questions
The project examines three related questions:
<br/>
### 1. Visual context
How do VLM assessments change when models receive isolated street-view images versus multiple images representing a route segment?
<br/>
### 2. Spatial sequence
To what extent are model judgments sensitive to the order and organization of visual evidence, rather than merely the amount of information provided?
<br/>
### 3.User profiles
How do assessments vary when the same environment is evaluated for users with different mobility requirements?
<br/>
Rather than assuming that additional images improve performance, the project treats visual context as an experimental variable.

## Dataset and Experimental Design
The study uses street-level imagery collected from Mapillary along 13 pedestrian routes in Seattle, covering approximately 7.97 km.
<br/>
A multi-scale sampling framework was developed to represent route environments at different spatial intervals, including 12 m, 24 m, and 48 m. The current dataset includes 52 selected keyframes.
<br/>

<figure class="text-center my-4">
  <img
    src="{{ '/assets/images/humanroute/figure1' | relative_url }}"
    alt="Seattle study routes and spatial sampling framework"
    class="img-fluid rounded"
    style="max-width: 850px; width: 100%;"
  >
  <figcaption class="text-muted small mt-2">
    <strong>Figure 1.</strong>
    Study area and spatial sampling framework.
  </figcaption>
</figure>

The experimental framework considers:
<br/>
### 1. Visual context
Single-image assessments and multi-image windows of three, five, and nine frames.
<br/>
### 2. Sequence organization
Ordered route imagery and planned sequence perturbations to examine sensitivity to spatial order.
<br/>
### 3. User profiles
Assessments for a general adult pedestrian, an older adult, and a wheelchair or stroller user.
<br/>
### 4. Structured outputs
Multi-dimensional environmental ratings alongside descriptions of route-level characteristics, including coherence and route patterns.
<br/>
These conditions are designed to distinguish changes associated with the amount, arrangement, and interpretation of visual evidence.

<figure class="text-center my-4">
  <img
    src="{{ '/assets/images/humanroute/figure2' | relative_url }}"
    alt="Visual context conditions and structured VLM assessment"
    class="img-fluid rounded"
    style="max-width: 850px; width: 100%;"
  >
  <figcaption class="text-muted small mt-2">
    <strong>Figure 2.</strong>
    Visual context conditions and structured assessment
    framework. Single-frame and multi-frame inputs are
    organized for profile-conditioned VLM evaluation.
  </figcaption>
</figure>

## Current Progress
The project has established a street-view sampling workflow, a structured evaluation schema, and an initial VLM inference pipeline.
<br/>
Implemented work includes route data preparation, keyframe selection, visual-context construction, and preliminary structured model inference.
<br/>
Systematic comparisons, human reference development, and validation remain ongoing. No definitive conclusions about model accuracy or spatial reasoning are claimed at this stage.

## Next Steps
The next stage focuses on completing human reference assessments, implementing controlled comparisons across context and sequence conditions, and examining the robustness of model-generated judgments.
<br/>
Ultimately, HumanRoute aims to contribute to a broader methodological question: how should multimodal AI systems be evaluated when the environments they assess are sequential, spatially connected, and experienced differently by different people?
