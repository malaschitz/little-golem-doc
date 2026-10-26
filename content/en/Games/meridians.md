---
title: "Meridians"
date: 2026-10-26
draft: true
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
