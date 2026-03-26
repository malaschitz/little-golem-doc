---
title: "Sixfold"
date: 2026-03-20
weight: 260
description: >
  A two-player abstract game on 36 active cells with six colors, six shapes, and randomly selected board layouts.
---

## Sixfold

Sixfold is a two-player abstract connection and grouping game played on exactly 36 active cells.
There are 36 unique stones in the game, each formed by one of 6 colors and one of 6 shapes.

![](/games/sixfold01.png)

The two roles are:

- `Shapes`
- `Colors`

The Shapes player moves first.

## Turn Structure

At the start of the game the board is empty and 6 random stones are revealed in the offer.

On each turn, a player:

1. may optionally move one stone already on the board in a straight line along the current board geometry
2. must place one offered stone onto an empty active cell

After placement, the offer is refilled back to 6 stones until the draw sequence is exhausted.

## Random Board Layouts

The board layout is not a separate variant.
It is selected randomly as part of the setup move.

Every Sixfold random setup uses one of these 4 layouts:

- `Square`: 6x6 board
- `Hex`: hex-style adjacency in 6 directions, with the center cell removed
- `Cross`: 7x7 board with the corner triads removed and the center cell removed
- `Triangle`: a hexagon-based isosceles triangular board with side length 8, similar in shape to the WYPS triangle boards

All four layouts contain exactly 36 active cells.

## Movement

If a player chooses to move a stone before placing, the stone moves in a straight line until blocked by:

- the board edge
- an inactive cell
- another stone

On square and cross boards, movement uses 4 orthogonal directions.

On hex and triangle boards, movement uses 6 hex-style directions.

## Scoring

Scoring is evaluated after the last stone is placed.

Shapes and Colors score independently.
For each connected group of size `N`, the score is:

`N * (N - 1) / 2`

The player with the higher total score wins.
If both totals are equal, the game is a draw.
