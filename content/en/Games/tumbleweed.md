---
title: "Tumbleweed"
date: 2022-08-12
weight: 240
description: >
  Modern game invented by Mike Zapawa during COVID
---

**Tumbleweed** is a two-player game. 
It is played on a hexhex board and a sufficient supply of stacked checkers.

![Tumbleweed in the Little Golem app](/games/tumbleweed-app.png)

A stack can "see" a hex, when they are connected by a straight line, with no stacks in between. 
The players take turns placing stacks of their tokens on hexes that are seen by at least one friendly stack. 
The height of every newly-placed stack equals the number of your stacks that see the new stack. 
Replacing an existing stack with a new stack is possible, as long as the new stack is taller than the previous one. 
This works with opponent stacks (to capture), or your own stacks (to reinforce).

Before the game, the host sets up the board and the guest decides which side he wants to play.
On Little Golem the board starts with one neutral stack of height 2 in the
center. The first move places one black stack and one white stack on two empty
hexes. The second player may then either accept the colors or play `swap`, which
swaps the two starting colors.

After setup, a normal move places or replaces one stack for the player to move.
The new stack height is the number of friendly stacks visible from that hex in
the six hex directions. A move with zero friendly visibility is illegal. A stack
may replace an existing stack only if the new stack is strictly taller.

The game ends after two successive passes. Little Golem scores occupied hexes
plus empty hexes controlled by influence. An empty hex is controlled by the
player with more visible stacks from that hex. The higher total wins; equal
totals are a draw.

## Links

The best article about Tumbleweed is on [Abstract Games](https://www.abstractgames.org/tumbleweed.html)

[Tumbleweed on Board Game Geek](https://boardgamegeek.com/boardgame/318702/tumbleweed)

## Variants

On Little Golem are supported four sizes of board: 4,6,8 and 11.

![board](/games/tw01.png)
