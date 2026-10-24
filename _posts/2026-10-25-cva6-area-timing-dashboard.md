---
layout: post
title: "Tracking CVA6 area and timing with an open-source flow"
date: 2026-10-25 09:00:00 +0100
description: A public dashboard of area and timing for the latest CVA6 RTL, produced with OpenROAD-flow-scripts on ASAP7 and Nangate45.
tags: risc-v cva6 asic openroad
categories: projects
featured: false
giscus_comments: true
related_posts: false
track_views: true
show_views: true
meta: '<span id="view-meta"><span id="view-count">...</span> views</span>'
---

**[Open the dashboard →](https://isa084.github.io/cva6-synthesis/)**

This is ongoing work: a reproducible area and timing view of the latest
[CVA6](https://github.com/openhwfoundation/cva6) RTL, built entirely with
open-source tools.

- **What is measured:** the `cva6` core for five standard configurations,
  through synthesis and floorplan with
  [OpenROAD-flow-scripts](https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts),
  in two technologies (ASAP7 and Nangate45). Cache memories are SRAM macros.
- **Settings:** aligned with the open-source physical-design flow proposed
  for CVA6 upstream (clock, synthesis options, no timing repair).
- **Two kinds of results:** `fast` runs complete the whole flow with cheap
  settings and are available first; detailed `opt` runs follow.
- **Reproducible:** every number links to its commit, and the same results
  can be regenerated from a fresh clone of
  [`isa084/cva6`](https://github.com/isa084/cva6) (branch `ft-synthesis`)
  with the flow in [`isa084/cva6-synthesis`](https://github.com/isa084/cva6-synthesis).

Timing is pre-layout and indicative. The dashboard is updated as new results
are generated.
