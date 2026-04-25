---
type: prompt
id: roadmap-status-brief
title: "Roadmap Status Brief"
description: "Collects current roadmap status for update analysis"
tags: [Production]
inputs:
  current_roadmap:
    label: "Current Roadmap"
    description: "Current roadmap or initiative list with status"
    example: "Paste your roadmap or OKR status here"
    required: true
    type: file
    accept: ".txt,.md,.csv,.docx"
  timeline:
    label: "Timeline"
    description: "Planning period"
    example: "Q3 2026"
    required: false
    type: text
connections:
  - target: progress-tracking
    type: derived_from
metadata:
  output_format: markdown
  prompt_type: task
---

You are a product strategist reviewing roadmap progress.

**Timeline:** {{input.timeline}}

### Current Roadmap

{{input.current_roadmap}}

Produce: Overall health, Per-initiative status, Velocity trends, Recommended adjustments, Risks.
