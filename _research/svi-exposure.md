---
layout: page
title: Street-Level Environmental Exposure Modelling
permalink: /research/svi-exposure/
---

# Street-Level Environmental Exposure Modelling

**An interpretable GeoAI framework for deriving human-centered environmental exposure indicators from street-level imagery**

<div class="project-meta">
  <span class="badge">Independent Research</span>
  <span class="badge">Street-Level Imagery</span>
  <span class="badge">Environmental Exposure</span>
  <span class="badge">GeoAI</span>
</div>

---

## Overview

This project develops an interpretable framework for modelling urban environmental exposure from street-level imagery. Street-view images provide rich information about everyday environmental conditions, but many image-based exposure studies rely on simplified visual indicators or end-to-end prediction models whose internal reasoning is difficult to interpret.

This research explores how street-level environments can be represented in a more mechanism-aware way. Instead of treating an image as a black-box input, the framework distinguishes between **semantic composition** — what environmental elements are visible — and **spatial structure** — how those elements are organised within the scene.

The broader goal is to support more interpretable environmental exposure assessment for urban health, mobility, and human-centered planning research.

---

## Research Motivation

Environmental exposure is not only about whether a visual feature is present or absent. The spatial dominance, continuity, adjacency, and configuration of environmental elements also shape how people experience streets and public spaces.

For example, traffic-related exposure may depend not only on whether roads or vehicles are visible, but also on their visual dominance, proximity to pedestrian space, and relationship with surrounding built form. Similarly, greenery, sky openness, enclosure, and building frontage may contribute differently depending on how they are spatially arranged.

This project therefore asks:

> How can street-level imagery be transformed into interpretable environmental exposure indicators that preserve both visual content and spatial structure?

---

## Research Questions

This project is guided by three main questions:

1. **How can street-level images be represented beyond simple pixel composition?**
   The project explores how semantic segmentation and spatial indicators can jointly describe visible urban environments.

2. **How can visual indicators be linked to mechanism-aware exposure interpretation?**
   Rather than predicting exposure outcomes directly, the framework aims to construct indicators that can be interpreted in relation to traffic dominance, visual enclosure, greenery, pedestrian space, and other environmental mechanisms.

3. **How can computer vision outputs be integrated with GIS-based spatial analysis?**
   The project examines how image-derived indicators can be connected to urban locations, street networks, land-use context, and broader spatial patterns.

---

## Methodological Framework

The proposed workflow includes three main components.

### 1. Semantic Representation

Street-level images are processed using semantic segmentation to identify visible environmental elements, such as:

* road surface;
* sidewalk or pedestrian space;
* buildings;
* vegetation;
* sky;
* vehicles;
* walls, fences, and other barriers;
* street furniture and other urban objects.

This step provides a basic compositional understanding of the image: what is visible, and how much of the scene each element occupies.

---

### 2. Structural Representation

Beyond semantic composition, the project explores spatial indicators that describe how environmental elements are organised within the image.

Potential indicators include:

* **visual dominance**: whether certain elements occupy a large share of the visual field;
* **adjacency**: whether features appear next to or separated from one another;
* **continuity**: whether pedestrian or environmental features form connected visual patterns;
* **enclosure**: how buildings, vegetation, or barriers shape perceived spatial containment;
* **openness**: how sky visibility and visual depth contribute to perceived openness;
* **traffic-pedestrian relationship**: how road space, vehicles, and pedestrian areas are visually arranged.

This structural layer is intended to preserve information that is often lost when images are reduced to simple feature percentages.

---

### 3. GIS-Based Interpretation

Image-derived indicators are linked with spatial data through GIS-based analysis. This allows street-level visual exposure to be interpreted in relation to:

* geographic location;
* street network structure;
* land-use context;
* neighbourhood morphology;
* accessibility and mobility conditions;
* broader urban environmental patterns.

Through this integration, street-view imagery becomes not only a visual dataset, but also part of a spatial analytical workflow.

---

## Conceptual Contribution

This project contributes to human-centered GeoAI and urban environmental exposure research in three ways.

First, it proposes a distinction between **semantic composition** and **spatial structure** in street-level environmental representation. This helps move beyond feature-counting approaches and supports more nuanced interpretation of visual urban environments.

Second, it emphasizes **mechanism-aware interpretation**. Instead of using computer vision only to predict environmental qualities, the framework asks how image-derived indicators can be connected to plausible urban health, mobility, and environmental experience mechanisms.

Third, it connects street-level computer vision with **GIS-based spatial reasoning**, allowing visual indicators to be situated within wider urban context.

---

## Relevance to Human-Centered Spatial Intelligence

This project is part of my broader research interest in **Human-Centered Spatial Intelligence**: how environments are perceived by people, represented through spatial data, and interpreted by computational systems.

Street-level imagery sits at the intersection of these concerns. It captures the everyday visual environment from a human-scale perspective, while also providing scalable data for computational analysis. By developing interpretable indicators from street-view images, this project aims to make AI-assisted urban assessment more transparent, spatially grounded, and relevant to human experience.

---

## Current Status

This project is currently under development as an independent research framework.

Ongoing work includes:

* testing semantic segmentation workflows for street-level imagery;
* developing interpretable visual and spatial indicators;
* linking image-derived metrics with GIS-based urban context;
* refining the conceptual framework for mechanism-aware exposure modelling;
* preparing case-study demonstrations and visual outputs.

---

## Methods and Tools

<div class="method-grid">

<div class="method-card">
<strong>Computer Vision</strong><br>
Semantic segmentation, street-level image processing, visual feature extraction.
</div>

<div class="method-card">
<strong>Spatial Analysis</strong><br>
GIS-based contextual analysis, street network linkage, land-use interpretation.
</div>

<div class="method-card">
<strong>Urban Exposure Modelling</strong><br>
Traffic dominance, visual enclosure, greenery, pedestrian space, and environmental proxies.
</div>

<div class="method-card">
<strong>Interpretability</strong><br>
Mechanism-aware indicators, structural representation, human-centered environmental assessment.
</div>

</div>

---

## Project Links

* **Code / Repository:** Coming soon
* **Demo:** Coming soon
* **Related tools:** See [Tools](/tools/)
* **Related research:** See [Research](/research/)

---

## Suggested Citation

Zhang, X. Street-Level Environmental Exposure Modelling: An interpretable GeoAI framework for deriving human-centered environmental exposure indicators from street-level imagery. Independent research project, ongoing.
