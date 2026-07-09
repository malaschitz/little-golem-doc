---
title: "Fendo"
date: 2023-04-30
weight: 105
description: >
  A modern abstract board game by Dieter Stein.
---

## Information

Fendo is probably Dieter Stein's best board game. It meets exactly all the prerequisites for a perfect abstract game: very simple rules, deep strategy and tactics. In addition, there is no possibility of a draw in the game. The game is also very nicely aesthetically made of wood. 

![Fendo in the Little Golem app](/games/fendo-app.jpg)

## Rules

Fendo is played on a 7x7 square board. Each player has seven pieces. On Little
Golem the red player starts on the middle square of the left edge and the blue
player starts on the middle square of the right edge. Each player has six
remaining pieces in hand. Fences are shared by both players.

The aim is to enclose more board squares than the opponent. A closed area is a
region of squares surrounded by board edges and fences. A closed area belongs to
the color of the single piece inside it. Areas with no piece, or with pieces of
both players, are not scored for either player.

On a turn a player must make one of these actions:

- Move one of their pieces in the open area and then build one fence.
- Add one new piece from hand to an empty legal square.

A moved piece travels horizontally or vertically through empty squares. It may
move any distance and may make at most one right-angle turn. It may not cross a
fence, pass through another piece, enter a closed area, or move diagonally. It
is legal to keep the selected piece on its current square, provided a legal
fence can then be built there.

After moving a piece, the player builds one fence on an empty side of the
piece's final square. The fence must keep the board position legal: after the
fence is added there may not be two separate open areas. In practical terms,
closing an area is legal only when the newly closed area contains exactly one
piece.

A new piece may be added on an empty square that is reachable by one legal
Fendo move from one of the player's pieces in the open area. Adding a piece
does not add a fence.

The game ends when no open area remains and the whole board is split into
closed areas. Each player scores the total number of squares in areas owned by
their pieces. The higher score wins.

## Little Golem notes

Little Golem uses the 7x7 variant. The move notation shown in game records is:

- `A1-B1/e` style display for moving a piece and building a fence on the east
  side of the destination.
- A single coordinate for adding a piece from hand.
- `Resign` ends the game immediately.

## Links

- [spielstein.com](https://spielstein.com/games/fendo)
- [Rules on spielstein.com](https://spielstein.com/games/fendo/rules)
- [Board Game Geek](https://boardgamegeek.com/boardgame/159333/fendo)
- [Online shop](https://www.spielewerkstatt.eu/gb/strategy-tactics/100-fendo.html)
