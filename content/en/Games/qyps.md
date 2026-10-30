---
title: "QYPS"
date: 2021-07-26
weight: 270
description: >
  Game invented by Richard Malaschitz in 2016
lastmod: 2026-10-30
---

## Rules

The game is played on a triangular board. The game is played with special stones. The stones have two sides (white and black). Each stone has two different colors. The game can be played on any board size:

![QYPS in the Little Golem app](/games/qyps-app.png)

![](/games/qyps01.png)

- The number of colors is the board size plus one.
- All color combinations are included in the game.
- The number of stones equals the number of spaces on the board.
- The size of each player's rack depends on the board size (3 for size 5, 5 for size 8).
- Each player has their own stones on a rack. After the initial racks are dealt,
  the opening choice is either `swap` or `noswap`.
- On their turn, a player can place several stones on the board. At least
  one stone must come from the player's rack.
- The stones used in one turn must form one connected path. The path may use
  newly placed rack stones and stones already on the board.
- All stones used in the turn must share at least one common color.
- After the turn, both racks are refilled from the bag.

![](/games/qyps02.png)

It is also possible to use stones already on the board. A player may explicitly
flip one used opponent stone to their own side. If all stones used in the turn
are in a straight line, then all opponent stones in that line are flipped to the
moving player's side.

![](/games/qyps03.png)

The game is evaluated when the board is full. The goal is to have a connected
group touching all three sides of the triangular board at the end of the game.
Little Golem marks a move that creates such a connection with a `+` in the
displayed move.

![](/games/qyps04.png)
