---
title: "XiangQi"
date: 2026-07-08
weight: 300
description: >
  Chinese chess.
---

XiangQi, also known as Chinese chess, is played on the intersections of a
9x10 board. Red moves first.

## Goal

The goal is to checkmate the opponent's general. A player may not make a move
that leaves their own general in check.

## Board

Each player has a 3x3 palace. The general and advisors may not leave the
palace.

The river divides the two sides of the board. Elephants cannot cross the river.
Soldiers gain sideways movement after crossing it.

## Pieces

| Piece | Symbol | Movement |
| --- | --- | --- |
| General | K | One point orthogonally inside the palace. The two generals may not face each other on the same file with no piece between them. |
| Advisor | A | One point diagonally inside the palace. |
| Elephant | B | Exactly two points diagonally. It cannot jump over a blocking piece and cannot cross the river. |
| Horse | N | One point orthogonally, then one point diagonally outward. It cannot move in a direction where the first orthogonal point is occupied. |
| Chariot | R | Any number of clear points orthogonally. |
| Cannon | C | Moves like a chariot when not capturing. To capture, it must jump exactly one piece of either color, then land on an enemy piece. |
| Soldier | P | One point forward. After crossing the river, it may also move one point sideways. It never moves backward. |

Pieces do not promote in XiangQi.

## Variant on Little Golem

Little Golem currently supports the standard XiangQi variant.

## Links

- [XiangQi on Wikipedia](https://en.wikipedia.org/wiki/Xiangqi)
- [XiangQi on BoardGameGeek](https://boardgamegeek.com/boardgame/2393/xiangqi)
