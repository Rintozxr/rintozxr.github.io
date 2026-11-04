---
layout: page
title: AFTERMATH
permalink: /research/aftermath/
---

# AFTERMATH

**Evaluating Terminal-State Externalities in Embodied Spatial Planning**

<div class="project-meta">
  <span class="badge">Independent Research</span>
  <span class="badge">Spatial Accessibility</span>
  <span class="badge">Human–Environment Interaction</span>
  <span class="badge">Counterfactual Evaluation</span>
</div>

---

## What kind of space does a robot leave behind after completing its task?
AFTERMATH is a computational research project investigating how successful robotic rearrangements alter the accessibility of shared environments for subsequent users. It examines the consequences of task-complete spatial configurations, the availability of less disruptive alternatives, and the differences between aggregate accessibility improvements and individual route requirements.<br>
<br>
*Figure 1. Different successful robot plans can leave substantially different accessibility conditions for subsequent users.*<br>

---

## The Problem
A robot is instructed to clear an entrance obstructed by five boxes. Multiple arrangements may successfully complete this task, yet the relocated boxes can obstruct other passages, create detours, or prevent users with different mobility capabilities from reaching their destinations.<br>
<br>
Conventional task-completion measures do not necessarily capture these downstream consequences.<br>
<br>
AFTERMATH investigates three questions.<br>
<br>
E1: Terminal-State Audit: What accessibility consequences remain after successful task completion?<br>
E2: Counterfactual Audit: Could an alternative successful plan reduce these consequences within a limited additional robot cost?<br>
E3: Requirement-Conditioned Evaluation: Does an aggregate accessibility improvement necessarily satisfy a specified user's route requirements?<br>

---

## The Framework
AFTERMATH uses 20 controlled indoor scenes, combining four spatial topologies (ring, linear, star, and tree) with five geometric configurations.
Each scene contains one entrance, three exits, and five boxes to be relocated. Robot plans are evaluated by execution cost and the accessibility of their resulting terminal arrangements.
Accessibility is assessed using three synthetic mobility profiles with different clearance requirements: adult (0.60 m), mobility-limited (0.75 m), and wheelchair (0.90 m).
For each terminal state, a geometric path scanner evaluates nine profile–destination combinations, recording route reachability and shortest-path detours relative to an unobstructed reference environment.<br>
<br>
Cost-bounded counterfactual analysis then compares alternative task-complete arrangements using the same accessibility measures.<br>
<br>
*Figure 2. Evaluation pipeline connecting robot task completion, terminal-state reconstruction, capability-conditioned accessibility assessment, and counterfactual comparison.*<br>

---

## Key Findings
### 01. Task completion does not determine post-task accessibility.
Successful robot plans can leave substantially different accessibility conditions. The consequences depend on the resulting box arrangement, spatial connectivity, and the clearance requirements of subsequent users.<br>

### 02. Some accessibility externalities have observable alternatives.
Across 20 controlled scenes, counterfactual analysis identified 8 scenes with improved aggregate accessibility rankings among observed task-complete arrangements within a 1.15× robot-cost budget.<br>
These results establish observed opportunities for improvement, rather than globally optimal solutions.<br>

### 03. Aggregate improvement may conflict with individual requirements.
A supplementary analysis examines whether candidate arrangements satisfy explicit, configurable route-detour limits.<br>
In the representative Tree C scenario, aggregate accessibility selection reduced unreachable routes from six to one, but increased the adult profile's maximum detour from 90.5% to 111.8%, violating a specified 100% detour limit.<br>
<br>
A subsequent requirement-constrained comparison identified a third arrangement that satisfied the adult requirement while retaining improvements for other profiles.<br>
This case illustrates why aggregate rankings and requirement-level outcomes should be examined separately.<br>
<br>
*Figure 3. Tree C: a comparison of task-cost, aggregate-accessibility, and requirement-constrained terminal-state selections.*

---

### Limitations
AFTERMATH is a controlled computational study, not a deployment or human-subject evaluation. Mobility profiles are simplified geometric models, and functional detour thresholds are synthetic experimental requirements.<br>
<br>
Counterfactual findings are limited to observed candidate arrangements and their associated robot-cost references. The framework evaluates spatial consequences; it does not establish whether an autonomous agent understands or anticipates human needs.<br>

---

## Research Materials
