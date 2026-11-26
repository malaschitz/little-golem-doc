---
title: "Morris"
linkTitle: "Morris (9, 10, 12)"
weight: 225
date: 2026-11-13
lastmod: 2026-11-13
description: >
  Nine Men's Morris, Lasker Morris and Morabaraba: the rules used on Little Golem.
---

Morris is one game family with three variants. These are the **Little Golem
rules**, including our automatic draw policy. The draw limits below apply to all three variants on Little Golem.

| Variant | Stones per player | Board surface | Placement and movement |
| --- | --- | --- | --- |
| **9 — Nine Men's Morris** | 9 | Sand | Place all stones, then move |
| **10 — Lasker Morris** | 10 | Light blue | Place or move from the first turn |
| **12 — Morabaraba** | 12 cows | Lilac | Place all cows, then move; extra diagonal connections |

## Board and objective

The board has 24 points on three nested squares, joined at the midpoints of
their sides. Morabaraba also joins corresponding corners diagonally. There is
no playable centre point and no connection through the centre.

Form **mills**: three of your stones on a marked straight three-point line.
Completing a mill lets you remove an opposing stone. Win by leaving the opponent
with fewer than three stones available for play, or with no legal action.

## Taking stones

After a placement or movement completes a mill, remove exactly **one** opposing
stone. Even if the action completes two mills, it earns only one capture.
Choose a stone outside an opposing mill whenever one exists. If every opposing
stone is in a mill, any opposing stone may be removed. Captured stones never
return to the reserve.

The placement or movement and its required capture form **one completed turn**.
You must finish the capture before sending the turn. In the client, choose the
stone to remove, then confirm with Send; Cancel discards the draft.

## 9 — Nine Men's Morris

White starts on an empty board. Players alternate placing one stone from their
reserve on a vacant point. Once both reserves are empty, move one stone along a
connection to an adjacent vacant point. A player with exactly three stones may
instead **fly** to any vacant point.

A mill may be opened and closed again on later turns. After placement, a player
loses with fewer than three stones or with no legal move.

## 10 — Lasker Morris

White starts. On every turn, either place a reserve stone on a vacant point or
move one of your stones to an adjacent vacant point. You may move while stones
remain in reserve; there is no separate placement phase.

Flying becomes available when **your own reserve is empty** and you have exactly
three stones on the board, even if your opponent still has reserve stones.
You lose with fewer than three stones in total (board plus reserve), or with no
legal action. Being unable to move a board stone is not defeat if a legal
placement remains available.

## 12 — Morabaraba

Dark starts. Each player has twelve cows. Placement, movement, flying and taking
cows work as in the nine-stone variant, with the extra diagonal mills and
connections shown on the board.

There is an additional restriction: if you transfer a cow from one mill into
another mill during movement, you may not immediately reverse that transfer on
your next turn to form a mill again. Little Golem applies this restriction during
flying too. A different legal action remains possible.

For example, moving F4–G4 from the F6–F4–F2 mill into the G7–G4–G1
mill prevents G4–F4 on your next turn. Play a different move first. Simply
opening a mill without forming another does not impose this restriction.

## Coordinates and controls

The board uses files **a–g** and ranks **1–7**, with a1 at the lower left in
normal orientation. Labels rotate with the board. You can click a stone and its
destination, or drag it there. Confirm the prepared move with **Send**; after
forming a mill, first select the opposing stone to capture.

History uses coordinates: **F2** places a stone, **G4-F4** moves it, and
**F4-G4 xB4** also captures the stone on B4. Older moves display the same notation.

## Automatic draws

These rules apply to all three variants:

* **50 individual moves without placement or capture.** Count each player's
  completed turn once: two players moving once each count as two moves.
  A placement or capture resets the counter to zero. In Lasker Morris, movement
  while reserve stones remain also counts toward the limit.
* **Three occurrences of the same position.** Compare positions only after
  completed turns, including the initial position. They must have the same
  occupied points, player to move, reserve counts and any restrictions affecting
  legal moves. In Morabaraba this includes mill-return restrictions. The draw
  counter itself is not part of the position. Rotations and reflections do not
  count as identical; the three occurrences need not be consecutive.

Morabaraba has a shorter endgame limit: once both reserves are empty and either
player has exactly three cows, **10 subsequent individual moves without capture**
produce a draw. The turn that first enters this endgame sets the counter to zero;
the next quiet turn counts as one. A capture resets it to zero if play continues.
Earlier turns do not count toward this limit. This ten-move limit does not apply
to variants 9 or 10.

Resolve the entire turn, including a capture, before checking the result.
**A win takes precedence over a draw.** A capture on the threshold turn resets
the counter instead of causing a draw. No draw claim is required.
