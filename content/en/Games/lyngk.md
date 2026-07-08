---
title: "Lyngk"
date: 2026-07-08
weight: 180
description: >
  A GIPF Project stacking game with color claims.
---

LYNGK is a two-player abstract strategy game by Kris Burm. Little Golem plays
the `Stack6` variant.

## Setup

The board is filled with a random mix of colored stones. The colors are white,
black, red, blue, green, and gray. Gray is neutral and cannot be claimed.

White moves first.

## Color claims

During the game, each player may claim up to two non-gray colors. A color can
be claimed by only one player.

A color claim is made together with a move or pass. Once you claim a color,
stacks topped by that color are yours.

## Movement

On a turn, move one stack in a straight line along the board lines to the first
occupied stack in that direction. Empty spaces may be crossed; occupied stacks
may not be jumped.

You may move:

- a stack topped by one of your claimed colors
- a stack topped by an unclaimed non-gray color

The moving stack is placed on top of the destination stack.

A combined stack may not contain the same non-gray color twice. Gray stones may
repeat. On Little Golem, a stack may contain at most six stones.

If the moving stack is neutral, it may not be moved onto a taller stack.

Passing is allowed only when no legal move is available.

## Winning and scoring

In `Stack6`, a player wins immediately by creating a stack of six stones topped
by one of their claimed colors.

Once four colors have been claimed and neither player has a legal move, the
game is scored by stacks topped by claimed colors. Taller stacks are worth
more:

| Height | Points |
| --- | --- |
| 1 | 1 |
| 2 | 10 |
| 3 | 100 |
| 4 | 1000 |
| 5 | 10000 |

The higher score wins. Equal scores are a draw.

## Variant on Little Golem

Little Golem supports `Stack6`.

## Links

- [Board Game Geek](https://boardgamegeek.com/boardgame/217083/lyngk)
