---
type: workflow
id: roadmap-update-flow
title: Roadmap Update Flow
description: "Revises roadmap based on velocity trends and priority changes"
tags: [Needs Review]
connections:
  - target: progress-tracking
    type: uses
  - target: resource-allocation
    type: uses
  - target: track-progress
    type: uses
  - target: allocate-resources
    type: uses
  - target: milestone-tracker
    type: uses
---

## Overview

This workflow analyses current velocity trends and priority shifts to produce an updated project roadmap with revised timelines and resource needs.

## Pipeline Stages

### Stage 1: Progress Analysis

Invoke the **progress-tracking** skill to gather and analyse velocity trends, burndown data, and milestone completion rates.

### Stage 2: Milestone Impact Assessment

Invoke the **milestone-tracker** prompt to assess how current velocity and any priority changes affect upcoming milestones.

### Stage 3: Resource Reallocation

Invoke the **resource-allocation** skill to recommend resource adjustments needed to support the revised roadmap.

### Stage 4: Roadmap Revision

Combine outputs to produce an updated roadmap with revised dates, resource allocations, and risk flags.

## Output

Updated roadmap containing:

- Revised milestone dates based on actual velocity
- Resource allocation adjustments
- Priority change impact analysis
- Risk flags for at-risk milestones
