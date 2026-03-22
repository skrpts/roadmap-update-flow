---
type: prompt
id: track-progress
title: Track Progress
description: "Core prompt for analysing project progress data"
tags: [Production]
connections:
  - target: progress-tracking
    type: derived_from
---

## Purpose

Analyses project metrics to identify velocity trends and their impact on roadmap projections.

## Prompt

You are a project analytics specialist. Given the following project metrics (velocity history, burndown data, milestone progress), analyse trends over the last several sprints. Identify whether velocity is stable, increasing, or declining. Project forward to estimate likely completion dates for upcoming milestones based on current trends.

## Project Metrics

**Velocity data:** {{input.velocity_data}}

**Milestone data:** {{input.milestone_data}}

**Priority changes:** {{input.priority_changes}}
