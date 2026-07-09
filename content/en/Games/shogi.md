---
title: "Shogi"
date: 2026-07-08
weight: 240
description: >
  Japanese chess and several smaller Shogi variants.
---

Shogi is a chess-family game with drops: captured pieces can return to the
board as your own pieces. Little Golem supports standard Shogi and several
smaller variants.

## Common rules

Sente moves first. Players alternate one move at a time.

On a turn you either:

- move one of your pieces on the board
- drop one captured piece from your hand onto an empty square

Pieces cannot move onto a square occupied by a friendly piece. A move may
capture an opponent piece on the destination square. Captured pieces are added
to the capturing player's hand in their unpromoted form.

The usual goal is to checkmate the opponent's royal piece. Fourfold repetition
is a draw.

Forward always means toward the opponent's side of the board.

## Drops

Captured pieces in hand may be dropped onto empty squares, with these
restrictions:

- A drop must not leave your own king in check.
- A pawn, lance, or Tori Shogi swallow may not be dropped on the last rank,
  where it would have no forward move.
- A knight may not be dropped on either of the last two ranks.
- In standard-piece variants, except Shogi 3x4, you may not drop an
  unpromoted pawn on a file where you already have an unpromoted pawn.
- A pawn drop that gives immediate checkmate is illegal in standard-piece
  variants, except Shogi 3x4.
- In Tori Shogi, a swallow drop that gives immediate checkmate is illegal.
- In Tori Shogi, a swallow may be dropped on a file only if you have fewer
  than two unpromoted swallows on that file before the drop.

## Promotion

A piece may promote when a move starts or ends in the promotion zone.
Promotion is optional unless the piece would otherwise have no legal move on a
later turn.

Promotion is forced for:

- pawn, lance, and Tori Shogi swallow on the last rank
- knight on either of the last two ranks

Promotion zones on Little Golem:

| Variant | Board | Promotion zone |
| --- | --- | --- |
| Shogi | 9x9 | last 3 ranks |
| Mini Shogi 5x5 | 5x5 | last rank |
| Tori Shogi | 7x7 | last 2 ranks |
| Shogi 3x4 | 3x4 | last rank |
| Shogi 5x6 | 5x6 | last 2 ranks |
| Shogi 5x6+ | 5x6 | last 2 ranks |

## Supported variants

| Variant | Board | Initial material per player | Notes |
| --- | --- | --- | --- |
| Shogi | 9x9 | King, rook, bishop, 2 golds, 2 silvers, 2 knights, 2 lances, 9 pawns | Standard Shogi. |
| Mini Shogi 5x5 | 5x5 | King, gold, silver, bishop, rook, pawn | Standard piece moves on a small board. |
| Tori Shogi | 7x7 | Phoenix, 2 quails, falcon, 2 cranes, 8 swallows, 2 pheasants | Bird-themed Shogi variant. |
| Shogi 3x4 | 3x4 | Lion, giraffe, elephant, chick | Also known as Dobutsu or Animal Shogi. |
| Shogi 5x6 | 5x6 | King, 2 golds, 2 silvers, 3 pawns | Compact Shogi using standard Shogi movement. |
| Shogi 5x6+ | 5x6 | Same as Shogi 5x6, plus a lance and knight in hand at the start | Extra opening drops from the first move. |

## Standard Shogi pieces

These pieces are used in Shogi, Mini Shogi, Shogi 5x6, and Shogi 5x6+.

| Piece | Symbol | Kanji | Movement | Promoted kanji | Promoted movement |
| --- | --- | --- | --- | --- | --- |
| King | K | 王 | One step in any direction. | - | Does not promote. |
| Rook | R | 飛 | Any number of squares orthogonally. | 龍 | Dragon king: rook movement plus one step diagonally. |
| Bishop | B | 角 | Any number of squares diagonally. | 馬 | Dragon horse: bishop movement plus one step orthogonally. |
| Gold general | G | 金 | One step forward, sideways, straight backward, or diagonally forward. | - | Does not promote. |
| Silver general | S | 銀 | One step forward, diagonally forward, or diagonally backward. | 全 | Moves as a gold general. |
| Knight | N | 桂 | Jumps two squares forward and one square sideways. | 圭 | Moves as a gold general. |
| Lance | L | 香 | Any number of squares straight forward. | 杏 | Moves as a gold general. |
| Pawn | P | 歩 | One step straight forward. | と | Moves as a gold general. |

## Shogi 3x4 pieces

Shogi 3x4 uses animal pieces. The Little Golem move notation also uses the
small symbols shown below.

| Piece | Symbol | App label | Movement | Promoted label | Promoted movement |
| --- | --- | --- | --- | --- | --- |
| Lion | K | 🦁 | One step in any direction. | - | Does not promote. |
| Giraffe | r | 🦒 | One step orthogonally. | - | Does not promote. |
| Elephant | b | 🐘 | One step diagonally. | - | Does not promote. |
| Chick | P | 🐥 | One step straight forward. | 🐔 | Hen: moves as a gold general. |

Shogi 3x4 also has a campmate rule: a lion wins by legally reaching the
opponent's back rank.

## Tori Shogi pieces

| Piece | Symbol | Kanji | Movement | Promoted kanji | Promoted movement |
| --- | --- | --- | --- | --- | --- |
| Phoenix | K | 鵬 | One step in any direction. | - | Does not promote. |
| Left quail | Ql | 鶉 | Slides straight forward and on one backward diagonal; steps one square on the other backward diagonal. | - | Does not promote. |
| Right quail | Qr | 鶉 | Mirror image of the left quail. | - | Does not promote. |
| Falcon | Fa | 鷹 | One step forward, sideways, or diagonally. It has no straight-back step. | 鵰 | Eagle. |
| Eagle | +Fa | 鵰 | Falcon movement plus extra long moves: slides straight backward, and can continue along a forward diagonal when the adjacent diagonal square is empty. It can also move two squares backward diagonally when the adjacent diagonal square is empty. | - | Already promoted. |
| Crane | Cr | 鶴 | One step straight or diagonally forward, and one step straight or diagonally backward. It has no sideways move. | - | Does not promote. |
| Swallow | Sw | 燕 | One step straight forward. | 鴈 | Goose. |
| Goose | +Sw | 鴈 | Jumps two squares diagonally forward or two squares straight backward. | - | Already promoted. |
| Pheasant | Pt | 雉 | Jumps two squares straight forward, or steps one square diagonally backward. | - | Does not promote. |

## Links

- [Shogi on Wikipedia](https://en.wikipedia.org/wiki/Shogi)
- [Mini Shogi on Wikipedia](https://en.wikipedia.org/wiki/Minishogi)
- [Dobutsu Shogi on Wikipedia](https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi)
- [Tori Shogi on Wikipedia](https://en.wikipedia.org/wiki/Tori_shogi)
