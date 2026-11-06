---
layout: page
title: BeyondSemantics
permalink: /research/beyondsemantics/
---

# Beyond Semantics

**Towards Structural Understanding in Street-View-Based Urban Environmental Assessment**

<div class="project-meta">
  <span class="badge">2025</span>
  <span class="badge">Methodological Pilot Study</span>
  <span class="badge">Street-Level Imagery</span>
  <span class="badge">Semantic Segmentation</span>
  <span class="badge">Environmental Exposure</span>
  <span class="badge">GeoAI</span>
</div>

---
## Overview
What do we miss when we describe urban environments through their visible components rather than their spatial relationships?
<br/>
Street-view imagery (SVI) and semantic segmentation have enabled large-scale environmental assessment by quantifying visible elements such as greenery, buildings, roads, and sky. However, environments with similar semantic compositions may differ substantially in their spatial organization and the ways people experience and use them.
<br/>
This research proposal explores the structural blind spots of composition-based street-view analysis. Drawing on earlier behavioural observations and environmental perception research, I developed a conceptual framework for incorporating spatial continuity, connectivity, clustering, and coherence into computational environmental assessment.
<br/>
Rather than replacing semantic segmentation, the proposal considers how structural information could complement semantic indicators to support a more comprehensive understanding of urban environments.
<br/>

## Research Motivation

The initial observation came from my MSc research along the River Clyde in Glasgow, where two riverside locations appeared visually similar and shared comparable semantic elements but exhibited different patterns of observed human activity.
<br/>

<figure class="text-center my-4">
  <img
    src="{{ 'assets/images/beyondsemantics/figure1.png' | relative_url }}"
    alt="idea source"
    class="img-fluid rounded"
    style="max-width: 850px; width: 100%;"
  >
  <figcaption class="text-muted small mt-2">
    <strong>Figure 1.</strong>
    Comparison of Clyde riverside street views, semantic segmentation outputs, and observed behavioural patterns.
  </figcaption>
</figure>

This contrast raised a methodological question: if two environments contain similar visible components, what additional information is needed to explain differences in their use?
<br/>
Conventional SVI-based assessment often summarizes semantic segmentation outputs as proportions of environmental categories. While useful for identifying what is present, these measures may overlook how elements are arranged, connected, and experienced across space.
<br/>
The proposal identified four potential limitations: fragmented flow across successive viewpoints, dislocated spatial elements, limited representation of structural relationships, and perceptual flattening when distinct configurations are reduced to similar semantic proportions.
<br/>

<figure class="text-center my-4">
  <img
    src="{{ 'assets/images/beyondsemantics/figure4.png' | relative_url }}"
    alt="weakness"
    class="img-fluid rounded"
    style="max-width: 850px; width: 100%;"
  >
  <figcaption class="text-muted small mt-2">
    <strong>Figure 2.</strong>
    Weakness of semantic segementation analysis for Street View Imageries(SVI)
  </figcaption>
</figure>


## Proposed Methodology

The proposed framework extends conventional semantic indicators with structural characteristics derived from street-view imagery and complementary spatial datasets.
<br/>
Three considerations informed the research design: environmental perception unfolds sequentially as people move through space; spatial organization extends beyond individual viewpoints; and the arrangement of environmental elements may influence perception and behaviour.
<br/>
Based on these considerations, I outlined several candidate structural indicators, including viewpoint continuity, fragmented flow, patch connectivity, spatial rhythm, coherence, green clustering, and visual opening.
<br/>
Two alternative methodological pathways were proposed to operationalize these indicators.
<br/>
### Pathway 1: GNN-Based Structural Learning
<br/>
This pathway represents street-view locations as nodes in a spatial graph, combining semantic image features with contextual information from remote sensing, LiDAR, and other environmental datasets.
<br/>
Graph neural networks could model relationships between neighbouring viewpoints and generate structure-enriched representations for subsequent environmental perception or health-related analyses.
<br/>
The approach was proposed for settings with relatively rich spatial data and computational resources.
<br/>
### Pathway 2: GIS-Based Structural Analysis
<br/>
This pathway uses publicly accessible GIS, street-view, and remote sensing data to calculate interpretable structural indicators within spatial units such as buffers or hexagonal grids.
<br/>
Measures of spatial variation, clustering, connectivity, and continuity could then be linked to street-view locations to characterize broader environmental organization.
<br/>
This approach was designed as a more accessible alternative for research contexts with limited high-resolution data or computational resources.
<br/>
Both pathways were developed as methodological proposals rather than implemented and validated models.
<br/>

<figure class="text-center my-4">
  <img
    src="{{ 'assets/images/beyondsemantics/figure2.png' | relative_url }}"
    alt="framework"
    class="img-fluid rounded"
    style="max-width: 850px; width: 100%;"
  >
  <figcaption class="text-muted small mt-2">
    <strong>Figure 3.</strong>
    Proposed GNN-based and GIS-based pathways for integrating spatial structure into street-view environmental representations.
  </figcaption>
</figure>

## Potential Applications and Research Implications

The proposed structural indicators could support three complementary research purposes: incorporating spatial organization as a predictor in environmental health models, using structural characteristics to explain differences in environmental perception, and identifying spatial configurations relevant to planning interventions.
<br/>
The central hypothesis is that semantic composition alone may not adequately represent the environmental relationships relevant to human experience and behaviour. Testing this hypothesis would require operationalizing the proposed indicators and evaluating their explanatory value against behavioural, perceptual, or health-related observations.
<br/>
This proposal also raised a broader question for my subsequent research: recognizing the components of an environment is not the same as understanding how they work together.
<br/>
It motivated my continued interest in spatial context, relational representations, and the limitations of computational environmental evaluation.
