---
title: "Street soccer"
date: 2021-07-26
weight: 260
description: >
  
---

[Board Game Geek](https://boardgamegeek.com/boardgame/3421/streetsoccer)

StreetSoccer on Little Golem keeps the legacy Java move flow. Each player first
places three extra players on legal empty fields. Yellow starts at the bottom
goal and red starts at the top goal.

After both setup moves, yellow kicks off. A turn is driven by a deterministic
die roll. A player piece moves orthogonally by the die value; if it reaches the
ball, the remaining movement value determines the legal ball kick fields. The
ball may travel straight, turn diagonally, or continue through same-color
players according to the legacy StreetSoccer rules.

When the ball enters the opponent goal, the scoring player gets one goal and
the next turn is a restart: the goalkeeper is placed on one of the two keeper
fields and then kicks the ball back into play.

The Java-compatible move notation is:

- `Pabcdef` for setup placement of three players.
- `Bxy` for first kickoff.
- `Mabcd` for a player-only move.
- `Mabcd|Bxy` for a player move followed by a ball kick.
- `Pxy|Buv` for an after-goal goalkeeper placement and ball kick.
