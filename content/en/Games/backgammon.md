---
title: "Backgammon"
date: 2026-10-19
lastmod: 2026-10-20
weight: 20
description: >
  Rules, controls, computer opponents and game analysis.
---

Backgammon is a race for two players, combining checker play with dice and,
in match play, decisions about the doubling cube. Little Golem supports two
formats:

| Format | Board | Scoring and doubling |
| --- | --- | --- |
| Single game | Green | One game, without a doubling cube. The first player to bear off all fifteen checkers wins. |
| 7-point match | Orange | A sequence of games until a player reaches at least seven points, with a doubling cube and the Crawford rule. |

Both formats support computer opponents and analysis of completed games.

## Moving the checkers

Each player has fifteen checkers. From that player's perspective, start with
two on point 24, five on 13, three on 8 and five on 6, moving toward point 1.
Each player rolls one die to start; ties are rerolled. The higher roller starts
using both dice. Later turns use two dice; doubles allow four moves.

A checker can land on an empty point, a friendly point or a single opposing
checker. A lone opposing checker is hit onto the bar and must re-enter before
other checkers move. Two or more opposing checkers block a point.
Use as many dice as legally possible. If only one unequal die can be used,
use the higher one if possible. Bearing off starts only when all remaining
checkers are in the home board. An oversized die can bear off only the checker
furthest from the exit. The first player to bear off all checkers wins.

## Match scoring and the doubling cube

In a seven-point match, an ordinary win scores one point, a gammon two (the
loser has borne off none), and a backgammon three (also a losing checker on
the bar or in the winner's home board), multiplied by the doubling cube.
Before rolling, a player may offer a double if the cube is centered or owned
by that player. Acceptance doubles its value and gives ownership to the
accepting player. Refusal loses the game at its previous value.
Further doubles are disabled when the current cube already guarantees the
match to either game's winner.
The first player to reach at least seven points wins the match.

### Crawford rule

When either player first reaches six points, the next game is the Crawford
game: doubling is forbidden for that game only. The cube returns in subsequent
games. Each new game starts with a centered cube of value one. Little Golem
does not use the Jacoby rule, beavers or automatic doubles.

## Playing on Little Golem

### Rolling and choosing the dice order

The opening roll is automatic. On later turns, the dice roll automatically
when you have no legal doubling decision. If you can offer a double, choose
between the cube and **Roll**, which appears on the board where the dice
normally sit.

New rolls display the higher die first. Click or tap the dice to swap their
order. Reopening the game preserves a roll that has already been made; it
does not give you another roll or another opportunity to double before it.

### Moving and sending a turn

1. Click or tap one of your checkers. It moves using the first available die
   in the displayed order, or the other die if the first cannot legally be
   used from that point. You do not need to select a destination.
2. Continue moving until you have used all the dice that can legally be
   played. Used dice fade. A double provides four moves.
3. Use **Undo** on the board to revise an unsent checker move.
4. Press the standard **Send move** button below the game to submit the
   completed turn.

You can also drag a checker to a legal destination. Enter checkers from the
bar before moving any others; when bearing off, you can tap a checker or
drag it to your **Off** tray. The interface enforces the requirement to use
as many dice as possible, including the higher-die rule. If no checker can
move, use **Send move** to submit the forced pass.

Moving checkers on the board prepares your turn; it does not send each
individual checker move to your opponent. Rolling is recorded immediately.

### Offering and responding to a double

In a 7-point match, click or tap the doubling cube before rolling to prepare
a double, then press **Send move**. Use **Cancel** to discard an unsent cube
decision.

When your opponent offers a double, choose on the board:

- **Take**: accept the new value and take ownership of the cube.
- **Drop**: concede the current game at the previous cube value.

Confirm either response with **Send move**. After a take, the player who
offered the double resumes their turn and rolls; the accepting player does
not immediately move.

The cube starts in the center. After an accepted double, it moves to the
accepting player's side, showing who may offer the next double. It is
centered while an offer awaits a response. During the Crawford game it
cannot be used. Single games do not display a doubling cube.

## Playing against a bot

Little Golem offers five computer-opponent levels powered by GNU Backgammon
for both formats. Sign in, open **Robots**, select **Backgammon**, choose the
format and an opponent, then select **Play**.

The levels use different engine settings. The ratings shown on the opponent
cards are their current Little Golem ratings, not fixed Elo promises for
an engine level. Bots follow the same rules as human players, including
cube decisions in a 7-point match.

## Analysing a completed game

GNU Backgammon analysis is available for completed single games and completed
7-point matches. Allow time for processing after the game finishes. Open the
completed game to see its evaluation panel, or use **Learning → My analyses**
to find games whose analysis is ready. If the panel is hidden, leave the
full-screen board view.

For an analysed decision, you can compare the move played with the engine's
recommended move and other alternatives. Match analysis also evaluates cube
decisions: whether to roll or double, and whether to take or drop.

The evaluation uses **match-winning chance (MWC)**: an estimated probability
of winning. For a single game, this is the chance of winning that game; for
a 7-point match, it includes the match score, cube and Crawford state.
The graph shows player 1's chance. Individual decision comparisons use the
perspective of the player making that decision.

Decision loss is expressed in percentage points relative to the engine's
preferred choice in the same position, with the same dice. A change in the
graph after a roll can also reflect the luck of the dice, so it should not
automatically be read as a playing mistake.

The **Analyse** button opens a local board where you can explore moves. It
does not request or start the server's GNU Backgammon evaluation.

Rules reference: [USBGF](https://usbgf.org/backgammon-basics-how-to-play/).
