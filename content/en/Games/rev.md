---
title: "Reversi"
date: 2026-07-08
weight: 230
description: >
  A disk-flipping strategy game played on several board sizes.
---

Reversi is a two-player strategy game played with black and white disks.
Black moves first.

## Rules

The game starts with four disks in the center of the board: two black and two
white on opposite diagonals.

On each turn, a player places one disk of their color on an empty square. The
move must outflank at least one straight line of opponent disks. A line is
outflanked when the newly placed disk and another disk of the moving color
enclose one or more opponent disks horizontally, vertically, or diagonally.

All outflanked opponent disks are flipped to the moving player's color.

If a player has no legal move, they pass. Passing is only legal when no move is
available. The game ends when neither player has a legal move.

The player with more disks on the board wins. If both players have the same
number of disks, the game is a draw.

## Variants on Little Golem

| Variant | Board |
| --- | --- |
| Size 6x6 | 6x6 |
| Size 8x8 | 8x8 |
| Size 10x10 | 10x10 |
| Size 12x12 | 12x12 |

## Links

- [Reversi on Wikipedia](https://en.wikipedia.org/wiki/Reversi)
