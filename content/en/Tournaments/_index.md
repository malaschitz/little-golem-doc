
---
title: "Tournaments"
linkTitle: "Tournaments"
weight: 8
description: >
  Tournament description
---

On *LittleGolem* are played tournaments for every game:

* Championship
* Monthly Cup
* Ladder
* User tournaments

There exists Waitting Room and is possible to invite to play some player.

[Time control](http://localhost:1313/time/) is used in all tournaments.

## Championship

The championship is the main type of tournament on LG.
Players are divided into groups in each league.
There is only one group in the first league.
In the second league there are two groups.
In the third league four groups, etc.

The winner in the first league is the champion.

The **top three** players in each group advance to the next higher league. 
Players up to **seventh** stay playing in their league. 

A new championship starts for each variant twice a year. 
There is a start date for each variant. 

### Calendar

Year-round championship calendar for all variants. 
Each year the championships starts on this date. 
However, the previous championship must be completed.

#### January and July 1st
     Draughts - Dameo
     Go - Size 37x37, Size 13x13
     WYPS - Italian 14, Japanese 8, Dutch 8
     Hex - Size 19
     Reversi - Size 6x6
     EinStein würfelt nicht! - 3-points match, Backwards capture
     Morelli - Size 9
     ConHex - ConHex
     Polyomino - penta
     Twixt PP - Size 30
     Breakthrough - Size 8
     Havannah - Size 6

#### February and August 1st
     Chess - Chess, Crazyhouse
     Go - Hahn Pointing System
     QYPS - Size 5
     Twixt PP - Size 24
     Four in a row - Size 6x7
     Four in a row - Size 10x10
     Lines of Action - Scramble, Quick, Black Hole
     EinStein würfelt nicht! - 1-point game
     Havannah - Size 10
     Tumbleweed - Size 8
     Draughts - International Draughts     
     WYPS - German 8, French 14, Spanish 14, Russian 11, WYPS - Slovak 5, Slovak 14, Russian 8
     Polyomino - small
     OSKI - Italian
     Reversi - Size 10x10
     Amazons - Size 10
     Dots and Boxes - Size 6x6
     EinStein würfelt nicht! - 7-points match
     Havannah - Size 7
     Slither - Size 9
     Catchup - Random
     Morelli - Size 13, Size 31
     Tumbleweed - Size 11

#### March and September 1st
     Go - Random100
     WYPS - English 14, English 5, Polish 8
     OSKI - French, Spanish, Slovak
     Hex - Size 13
     Golem Word Game - 100 letters
     EinStein würfelt nicht! - 11-points match
     Slither - Size 13
     WYPS - Greek 14
     Polyomino - hexa
     Hex - Size 15
     Four in a row - Size 8x8
     Gomoku - Gomoku Pro
     Gomoku - Gomoku
     Dots and Boxes - Size 7x7
     EinStein würfelt nicht! - Black hole
     Havannah - Size 8 

#### April and October 1st
     Go - Size 19x19
     Shogi - Shogi 5x6, Shogi 5x6 PLUS
     WYPS - Italian 8, Dutch 14, Czech 8, Japanese 14
     Polyomino - mini
     OSKI - Greek, English
     Twixt PP - Size 48     
     Reversi - Size 12x12
     Connect6 - Connect6
     Havannah - Size 9
     Tumbleweed - Size 4

#### May and November 1st
     Draughts - English Draughts/Checkers
     Shogi - Shogi
     WYPS - Slovak 8
     QYPS - Size 8
     OSKI - Dutch
     Hex - Size 11
     Amazons - Cross
     StreetSoccer - Street Soccer
     Havannah - Size 4
     XiangQi - XiangQi
     Chess - Grand Chess
     Shogi - Tori Shogi
     WYPS - French 8, Spanish 8, Slovak 11, Russian 5, Russian 14, Numeric small, German 14
     Reversi - Size 8x8
     DVONN - DVONN
     Four in a row - Size 9x9
     EinStein würfelt nicht! - 19-points match
     Catchup - Size 7

#### June and December 1st
     Go - Size 9x9, Size 27x27, Toroidal Go
     Chess - Chess960
     Shogi - Mini Shogi, Shogi 3x4
     LYNGK - Stack6
     Gomoku - Gomoku Pro 9x9
     Dots and Boxes - Size 4x4
     Lines of Action - Size 8x8
     EinStein würfelt nicht! - 5-points match, 50-points match
     Havannah - Size 5
     Morelli - Size 11       
     WYPS - English 11, Polish 14, Greek 8, Numeric, English 8
     OSKI - German
     TZAAR - Random
     Dots and Boxes - Size 5x5
     Catchup - Size 5
     Tumbleweed - Size 6
     Oceans 11 - Deck 54

## Monthly Cup

The tournament starts immediately when 5 players are logged in. 
Each player plays against every other player.
The winners of all groups started during the month will play in the following month's tournament.
The winners of all monthly cups during the year play in the following year's tournament.

## Ladder 

For each game there is a running tournament. 
The players are lined up in a list.
Players challenge the player in the higher position, up to CEIL (SQRT (position)).
Example:

| Position | CEIL(SQRT(position)) | Can challenge |
|----------|----------------------|---------------|
|    1     |          -           |       -       |
|    2     |          2           |       1       |
|    3     |          2           |      1-2      |
|    4     |          2           |      2-3      |
|    5     |          3           |      2-4      |
|    6     |          3           |      3-5      |
|    7     |          3           |      4-6      |
|    8     |          3           |      5-7      |
|    9     |          3           |      6-8      |
|    10    |          4           |      6-9      |

If the challenger wins the game, he overtakes his opponent. 
Players challenge a maximum of 1 player and defend against 2 players.
A new game with the same opponent is possible only after 14 days after the common game.
The game starts immediately when the player registers for the tournament.
The games are started automatically. 
Players always challenge the player in the highest available position.

## Waiting Room

Simple waiting room for playing rated games.

## User tournaments

Players can create their own round robin tournaments.

## Invite players

The player can invite another player to a game.
