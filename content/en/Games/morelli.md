---
title: "Morelli"
date: 2026-07-08
weight: 190
description: >
  A center-race abstract strategy game.
---

Morelli is a two-player abstract strategy game. Black moves first.

## Setup

Little Golem uses a random setup on the edge of the board. Black and white
stones are placed on paired opposite edge cells. The center starts empty and is
the key square of the game.

## Movement

Move one of your stones in a straight line toward the center. The move may be
orthogonal or diagonal and may cross any number of empty cells, but it cannot
jump over a stone.

A move must strictly reduce the stone's distance from the center. A stone may
not move onto the center square.

## Capturing

After a move, opponent stones can be converted by custodian capture. If an
opponent stone is adjacent to the moved stone and the next cell in the same
line contains one of your stones, the opponent stone is turned to your color.
This is checked in all eight directions.

## The Morelli square

If a moved or converted stone completes a fourfold rotational set around the
center, the center becomes marked for that player.

The game ends when the player to move has no legal move. The player who owns
the center marker wins. If nobody owns the center, the game is a draw.

## Variants on Little Golem

| Variant | Board |
| --- | --- |
| Size 9 | 9x9 |
| Size 11 | 11x11 |
| Size 13 | 13x13 |
| Size 31 | 31x31 |

## Links

- [Morelli on BoardGameGeek](https://boardgamegeek.com/boardgame/103830/morelli)
