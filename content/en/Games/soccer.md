---
title: "Street soccer"
date: 2021-07-26
weight: 260
description: >
  
---

StreetSoccer is a two-player football board game by Corné van Moorsel. Little
Golem uses the legacy online flow from the Java implementation.

![StreetSoccer in the Little Golem app](/games/soccer-app.png)

## Setup

Yellow starts at the bottom goal and red starts at the top goal. Each player
has five players on the field, including one keeper. At the beginning the
keeper and one field player are already placed. The first phase is compressed
into two setup moves:

- Yellow places three extra field players on legal empty fields.
- Red places three extra field players on legal empty fields.
- Each setup must place at least one player in the opponent's half.
- Players may not be placed in the center circle.
- Only the keeper may occupy the two keeper fields in front of their own goal,
  except when the ball is there.

After both setup moves, Yellow kicks off. The kickoff die is generated from the
two first virtual dice as the absolute difference between them, ignoring zero.
The kickoff places only the ball; it cannot score a goal.

## Turn

Each normal turn is driven by a deterministic die roll from 1 to 6. The player
chooses one of their five pieces and moves it orthogonally by exactly the die
value. A moving player may change direction between steps, but may not move
through occupied fields.

If the moving player reaches the ball before using all die steps, the player
stops on the ball and kicks it. The unused movement determines the kick length;
Little Golem calculates all legal ball destinations.

## Ball movement

The ball may move in the eight straight or diagonal directions. During one kick
it may make one direction change: from straight to diagonal, or from diagonal to
straight. The ball may not pass through an opponent.

If the ball reaches a friendly player, that player immediately redirects it:
the remaining kick distance continues from that player's field, again with a
new choice of direction and one allowed direction change. This is how passes are
handled.

A move must also leave the ball reachable for the opponent. Little Golem rejects
moves that surround the ball so tightly that the opponent cannot reach it.

## Goals and restart

A goal is scored when the ball crosses the opponent's end line through the goal
area. On Little Golem the goal mouth is the four central columns, and the last
field before the end line must be one of the two fields directly in front of
the goal.

After a goal, the next turn is a restart. The keeper is placed on one of the two
keeper fields and then kicks the ball back into play. After-goal kicks use a die
from 2 to 6.

## End of game and tournament points

The normal game ends after 52 online moves. If the score is not tied, the
leader wins. If the score is tied, sudden death begins and lasts at most 20
more moves. Any goal in sudden death wins immediately. If nobody scores in
sudden death, the player who scored the last goal wins; if there was no goal,
the game is drawn.

Tournament scoring follows the legacy StreetSoccer system:

- Normal-time win: 5 tournament points to the winner, 0 to the loser.
- Sudden-death win: 4 points to the winner, 1 to the loser.
- Undecided game with goals: 3 points to the player who scored last, 2 to the
  other player.
- Scoreless undecided game: 2 points for each player.

## Move notation

The Java-compatible move notation is:

- `Pabcdef` for setup placement of three players.
- `Bxy` for first kickoff.
- `Mabcd` for a player-only move.
- `Mabcd|Bxy` for a player move followed by a ball kick.
- `Pxy|Buv` for an after-goal goalkeeper placement and ball kick.

## Links

- [Board Game Geek](https://boardgamegeek.com/boardgame/3421/streetsoccer)
