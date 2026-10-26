---
title: "Quantum Control"
date: 2026-10-26
draft: true
description: "Standard Quantum Control: placement, captures and seven-area scoring."
---

Quantum Control by Néstor Romeral Andrés and Kanare Kato has49playable spaces
in seven7-space areas and12unoccupiable gaps. Black starts with one placement;
White then starts alternating two-stone placements. A pair must occupy two
areas whenever empty sites in different areas remain. After all49sites are
filled, White starts capture play.

A capture jumps along one of the six grid directions by exactly the moving
stone's number of adjacent friendly stones, counted BEFORE moving, including
across area boundaries. Zero neighbours means no move. The destination must
contain an enemy stone, which is removed; intermediate pieces and gaps can be
jumped over. Each gap counts as one unit of distance.

During captures either player may pass, including with captures available. End
when both pass in succession or neither has a legal capture. Each area is
claimed by the colour with more surviving stones; tied/empty areas are unclaimed.
Most claimed areas wins. Tied area totals are broken by the last capture.
The first Little Golem format uses standard placement, without Blitz or swap.

Select the placement(s), or the capture source and destination, then use the
standard Send move action. Pending moves can be cancelled. Pass is available
only during capture play.

Computer opponents use the independently tested enhanced alpha-beta engine.
Its highest profile uses depth12,200,000nodes and a cooperative2-second search
limit. Lower levels are not calibrated human ratings. Completed-game analysis
is separate from move-selection bots and is not provided by this implementation.

[Publisher rules](https://cdn.shopify.com/s/files/1/0578/3502/8664/files/QuantumControl_QuantumLeap_EN.pdf?v=1782373284).
Implementation agreement with Néstor was confirmed by Richard.
