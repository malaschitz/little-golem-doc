---
title: "Quantum Control"
date: 2026-10-26
lastmod: 2026-10-30
draft: false
description: "Standard Quantum Control: placement, captures and seven-area scoring."
weight: 260
---

Quantum Control by Néstor Romeral Andrés and Kanare Kato has 49 playable spaces
in seven 7-space areas and 12 unoccupiable gaps. Black starts with one placement;
Starting with White, players then alternate two-stone placements. A pair must occupy two different
areas whenever empty sites in different areas remain. After all 49 sites are
filled, White starts capture play.

A capture jumps along one of the six grid directions by exactly the moving
stone's number of adjacent friendly stones, counted BEFORE moving, including
across area boundaries. Zero neighbours means no move. The destination must
contain an enemy stone, which is removed; intermediate pieces and gaps can be
jumped over. Each gap counts as one unit of distance.

During capture play, either player may pass, even when a capture is available.
The game ends when both players pass in succession or neither has a legal capture. Each area is
claimed by the colour with more surviving stones; tied/empty areas are unclaimed.
The player who claims the most areas wins. Tied area totals are broken by the last capture.
The first Little Golem format uses standard placement, without Blitz or swap.

Select the placement(s), or the capture source and destination, then use the
standard Send move action. Pending moves can be cancelled. Pass is available
only during capture play.

Computer opponents use the independently tested enhanced alpha-beta engine.
Its highest profile uses a search depth of 12, a 200,000-node budget and a
cooperative 2-second search limit. Lower levels are not calibrated human ratings. Completed-game analysis
is separate from move-selection bots and is not provided by this implementation.

[Publisher rules](https://cdn.shopify.com/s/files/1/0578/3502/8664/files/QuantumControl_QuantumLeap_EN.pdf?v=1782373284).
Implementation agreement with Néstor was confirmed by Richard.

![Quantum Control board showing seven areas, dark gaps and both colours of stones](/games/qcontrol-board.png)

*The seven areas decide the result. Dark gaps count when measuring a jump but cannot hold stones.*

## Placement step by step

1. Black places **one** stone on any playable space.
2. White places **two**, then Black places two, continuing in alternating turns.
3. The pair must use different areas if at least two areas still have empty
   spaces. Only when all remaining empty spaces are in one area may both go there.
4. Once all 49 spaces are occupied, Black has 25 stones and White has 24. **White
   starts the capture phase**, although Black started placement.

There is no pass or colour swap during standard placement. The twelve dark
spaces between the seven areas are gaps: stones can never occupy them.

## Capture example

A stone with two friendly neighbours must jump exactly two spaces in one of
six straight directions onto an enemy stone. It cannot jump one space or land
on an empty space. Remove the enemy and put the moving stone in its place.
Intermediate stones do not block the jump. Gaps count towards the distance but
cannot be landing spaces. Count neighbours **before** moving, including across
area boundaries. With zero friendly neighbours a stone cannot move. Each turn
captures just one stone; there is no multiple-capture sequence.

## Passing, ending and scoring

During capture play you may pass even when a capture exists; with no capture,
you must pass. A capture resets the consecutive-pass count. The game ends after
two consecutive passes, or as soon as neither colour has a legal capture.

An area with three White stones and two Black stones belongs to White. An area
with one of each, or no stones, belongs to neither. Controlling four areas beats
controlling three regardless of the overall stone count. If controlled-area
totals tie, the player who made the **last capture** wins; passing does not
change the last capturer.

## Sending and correcting a move

During placement select an empty playable space, then the second placement
when required. During captures select your stone and then the destination.
Review the pending move and press **Send move**; selecting spaces does not
submit the turn. Cancel before sending to choose again. Pass is available only
in capture play and uses the standard move submission workflow. You may resign.

## Formats and computer opponents

This is standard Quantum Control, without Blitz or swap. Quantum Leap is a
separate game with different rules. GolemBot One through Five are registered
for test games. Their levels are not calibrated human ratings. Completed-game
analysis is not currently provided.
