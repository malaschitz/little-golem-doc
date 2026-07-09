---
title: "QYPS"
date: 2021-07-26
weight: 220
description: >
  Game invented by Richard Malaschitz in 2016
---

## Rules

The game is played on a triangular board. The game is played with special stones. The stones have two sides (white and black). Each stone has two different colors. The game can be played on any board size:

![QYPS in the Little Golem app](/games/qyps-app.png)

![](/games/qyps01.png)

- Number of colors is size+1
- All color combinations are in game
- The number of stones is equal to the number of fields on the board
- The size of rack for player's stones depends on size of board (3 for size 5, 5 for size 8)
- Each player has his own stones on rack. After the initial racks are dealt,
  the opening choice is either `swap` or `noswap`.
- When it is a player's turn, he can put several stones on the board. At least
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
