---
title: "GIPF"
linkTitle: "GIPF"
weight: 135
date: 2026-11-13
lastmod: 2026-11-13
description: >
  GIPF Tournament rules, row removal, GIPF pieces and useful external links.
---

Little Golem supports **GIPF Tournament**. The game is currently in a private
trial. Basic and Standard starting positions, and Project GIPF potentials, are
not used here.

## Board, pieces and opening

There are 37 playing points and 24 entry dots around the edge. Each player has
18 single pieces. Two stacked pieces form a **GIPF piece**: it costs two reserve
pieces but occupies one point and counts once when forming a row.

Start with an empty board; White plays first. Each player's first insertion
must be a GIPF piece. On later turns, that player may continue inserting GIPF
pieces or switch to singles. **After inserting your first single, you may never
insert another GIPF piece.** The players make that switch independently.

These are the Tournament opening rules; see the
[official complete rules](https://www.gipf.com/gipf/rules/complete_rules.html).

## Inserting a piece

Choose an edge dot, then an inward direction along a marked line. Insert one
piece from your reserve onto the first playing point. If occupied, push the
contiguous pieces one point along that line until a vacant point is filled.
Colours do not matter when pushing. **Pushing a piece off the board is illegal.**

You must make an insertion on your turn. Taking pieces is a consequence or an
allowed preliminary action, not a substitute for inserting. The
[official illustrated introduction](https://www.gipf.com/gipf/rules/rules.html)
shows how insertion and pushing work.

## Resolving rows

Four or more consecutive pieces of one colour form a row. Resolve the entire
uninterrupted occupied segment on that line, including pieces extending beyond
the matching row in either direction; an empty point ends the segment.

* Remove all single pieces in that segment. Your own return to your reserve;
  opposing pieces are captured permanently.
* For each GIPF piece in the segment, choose separately whether to take it or
  leave it. A friendly GIPF piece taken back provides two reserve singles.
* The **owner of the matching row** makes these choices, even when the opponent's
  insertion created the row.
* If both colours have rows, the inserting player's rows are resolved first.
  Resolve rows one at a time and reassess the board. Taking an intersecting row
  may destroy another; retaining a GIPF piece at the intersection may preserve it.

A row consisting entirely of GIPF pieces is optional: leave it intact or take
one or more GIPF pieces. If it survives, its owner may reclaim pieces before a
later insertion. Reclaiming a double does not end the opening permission to play
doubles; only inserting a single does that.

The [official FAQ](https://www.gipf.com/gipf/faq/faq.html), especially questions
1, 3, 4, 8 and 9, clarifies ownership and the order of these decisions.

## Winning and repeated positions

You lose if your last GIPF piece is removed, or if you cannot make the required
insertion. Recovering pieces from an available optional GIPF row may replenish
an empty reserve before insertion. If one removal takes both players' last
GIPF pieces, **the player making the removal wins** (official FAQ 10).

The Morris 50-move and 10-move draw limits do not apply. Three repetitions do
not automatically produce a GIPF draw. Official FAQ 7 describes a referee-led
restart with exchanged colours and remaining clock times after repeated play.
**Little Golem does not yet automate that restart procedure.** A repeated
position must not be interpreted as a completed draw.

## Playing in the Little Golem client

During insertion, select an edge dot and then the inward destination, or drag
from the edge dot to that first inward point. Invalid or cancelled drops leave
the position unchanged. Reserve counts appear as numbered stones inside the
upper-right and lower-right corners of the board. The
upper-left corner icon selects single or double pieces while doubles remain legal.
Confirm the prepared action with **Send**.

For a row decision, use the upper-left arrow to cycle eligible rows if necessary,
tap the GIPF pieces you want to take, then use the upper-right checkmark
(**Take row**). Singles are included automatically. The lower-right icon
skips an optional pure-GIPF row (**Leave row**), or enters **Reclaim GIPF**
before insertion. A back arrow exits reclaim selection. Tooltips name each
icon; controls stay inside the board so row decisions do not resize it. Confirm the decision with Send. Row decisions may therefore
require the other player to act before the next insertion.

## External rules and further reading

* [Complete official rules](https://www.gipf.com/gipf/rules/complete_rules.html)
  — Basic, Standard and Tournament; use Tournament on Little Golem.
* [Official illustrated Tournament introduction](https://www.gipf.com/gipf/rules/rules.html)
  — diagrams explaining the main ideas.
* [Official FAQ](https://www.gipf.com/gipf/faq/faq.html)
  — detailed rulings, optional rows and repetition.
* [Publisher's English rulebook (PDF)](https://www.riograndegames.com/wp-content/uploads/2013/02/GIPF-Rules.pdf)
  — printable illustrated rules from Rio Grande Games.
* [Official GIPF introduction](https://www.gipf.com/gipf/intro/intro.html)
  — background and an overview of the game.
