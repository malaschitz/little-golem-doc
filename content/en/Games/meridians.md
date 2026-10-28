---
title: "Meridians"
date: 2026-10-26
lastmod: 2026-10-28
draft: false
description: "Meridians 114: paths, group survival and colour choice."
---

Meridians by Kanare Kato is an elimination game. Little Golem's first format
uses the114-point board and pie opening. Stones are placed on intersections;
they never move. Adjacent friendly stones form a group, including single stones.
A path joins DIFFERENT friendly groups along a straight line of one or more
empty intersections. A group lives if any of its stones has such a path.

The first participant places one Light and one Dark stone. The other chooses
Keep colours (Light remains with the first participant) or Swap colours (the
chooser takes Light). Light continues. Each colour's second stone must see its
first across at least one empty point, without being adjacent to it.

On each normal turn, remove all opposing dead groups, then place one friendly
stone on an empty intersection visible along a grid line from an existing
friendly stone without an intervening enemy. A threatened group gets its own
turn to restore a path or join a living group before removal. Voluntary pass
is unavailable; when no placement exists, the turn is forced to pass. After
the opening, a player with no stones loses. Territory and prisoners are not scored.

Select points on the board, then use the standard Send move action. The first
opening selects Light's point and then Dark's point. Colour choice is on the
board. Pending moves can be cancelled before sending.

Computer opponents use the tested guarded Biased MCTS policy. Opening balance
and human strength remain under evaluation; levels are not human ratings.

[Publisher rules](https://cdn.shopify.com/s/files/1/0578/3502/8664/files/Meridians_EN.pdf?v=1693585479).
Permission for the Little Golem implementation was granted by Kanare.

## Opening step by step

1. The first participant selects White's point and then Black's point. Send
   these two placements together as one opening move.
2. The other participant chooses **Keep colours (Black)** or **Swap colours
   (White)**, then sends that choice. Keeping leaves White with the first
   participant. Swapping gives White to the chooser without moving the stones.
3. **White moves next**, placing its second stone; Black then places its second.
   Each second stone must be separated from its first by at least one empty
   point along an unobstructed board line. They cannot be adjacent.

## Understanding survival

A group needs a path to a **different friendly group**. Two separated friendly
stones with an empty point between them support each other. Two adjacent stones
alone form one group, so they do not support each other. An intervening stone
blocks a path; seeing another part of the same group is insufficient.

During ordinary play, a legal placement may be adjacent to a friendly stone.
It only needs an unobstructed straight line to an existing friendly stone.
Legal placement and survival are different conditions.

When your opponent cuts your group's last path, you have one turn to save it:
restore a path or connect it to a living group. If it is still dead, it is removed
at the start of the opponent's next turn. Little Golem resolves that boundary
at the end of your rescue turn, so the next player already sees the removals.
The special opening establishes both colours before ordinary removal begins.

## Sending and correcting a move

Selecting a point or colour does not submit it. Review the pending move, then
press **Send move**. The colour-choice move explicitly names Keep or Swap.
Cancel the pending move before sending to choose again. The board handles
legal placements and removals. Pass is available only if no placement exists.
You may also resign.

## Formats and computer opponents

Only Meridians **114 points with pie rule** is currently implemented; the
smaller and larger boards are not included. GolemBot One through Five are
registered for test games. Their levels are not calibrated human ratings.
Automatic analysis of completed games is not currently provided.
