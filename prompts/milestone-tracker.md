---
type: prompt
id: milestone-tracker
title: Milestone Tracker
description: "Task prompt for assessing velocity impact on milestones"
tags: [Production]
connections:
  - target: progress-tracking
    type: derived_from
---

## Purpose

Projects milestone delivery dates based on current velocity trends and priority changes.

## Prompt

Given the following project milestones, current velocity trend, and any priority changes, assess each milestone's projected delivery date. Compare projected dates against planned dates, flag any milestones at risk of slipping, and recommend corrective actions such as scope reduction, resource addition, or deadline adjustment.

## Velocity Trend Analysis

{{steps.track-progress.output}}

## Priority Changes

{{input.priority_changes}}
