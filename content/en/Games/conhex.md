---
title: "Conhex"
date: 2021-07-26
weight: 50
description: >
  Game invented by Michail Antonow in 2006
---

Conhex is a two-player connection game invented by Michail Antonow. The goal is
to claim a connected chain of spaces between the player's two assigned sides.
The board is made of polygonal spaces. Players do not place stones inside the
spaces directly; they place stones on the vertices around them.

![Conhex in the Little Golem app](/games/conhex-app.png)

![](/games/conhex01.png)

## Rules

Blue moves first. A move is made by placing one stone on any empty playable
vertex. Some visual points on the board are gaps and cannot be played.

After a stone is placed, every still-unclaimed space is checked. A player claims
a space as soon as that player owns at least half of the playable vertices
around it. For example, a four-vertex space is claimed with two vertices, and a
five-vertex space is claimed with three vertices. Once a space is claimed, it
keeps that owner.

The first player who connects their two opposite sides with a connected group
of claimed spaces wins.

On Little Golem:

- Blue connects the bottom side to the top side.
- Red connects the left side to the right side.
- Spaces are connected when they share at least one vertex.
- Draw offers are possible, but the game itself has no normal draw condition.

## Swap move

Conhex uses the swap rule. After Blue's first placement, Red may play `swap`
instead of placing a normal stone. The swapped stone is moved to the reflected
point used by the Little Golem board geometry, and the colors continue from
there with Blue to move.

## Links

- [Board Game Geek](https://boardgamegeek.com/boardgame/10989/conhex)

