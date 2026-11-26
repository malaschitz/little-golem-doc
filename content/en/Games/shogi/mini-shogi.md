---
title: "Mini Shogi"
weight: 25
description: "5 × 5 board. The promotion zone covers the farthest rank."
---

Each player starts with one king, gold, silver, bishop, rook and pawn.

Sente moves first. Each turn, move one piece or drop one from your hand onto an empty square. Checkmate wins. Your move must leave your king safe. Capturing a promoted piece returns it to its original form in your hand.

The default Little Golem rules draw a fourfold repetition. With the competition repetition rule, the player who gave check on every turn of the repeated sequence loses. Otherwise the second player (gote) wins a fourfold repetition.

## Drops and promotion

A pawn drop is illegal on the last rank, on a file containing one of your unpromoted pawns, or if the drop gives immediate checkmate. A piece may promote when its move begins or ends in the promotion zone (the farthest rank). A drop places an unpromoted piece.

## Piece guide

Forward is **up** in every diagram. The dark tile is the starting square. A **dot** marks a reachable square, an **arrow** means any distance on a clear line, and a **diamond** marks a jump over intervening pieces. Slides stop at the first occupied square. You may capture an opposing piece there.

### King · 王 (K)

{{< shogi-move "king" "King · 王 (K)" >}}
Steps one square in any direction. It is a royal piece.

Does not promote.
{{< /shogi-move >}}

### Rook · 飛 (R)

{{< shogi-move "rook" "Rook · 飛 (R)" >}}
Slides any distance along a rank or file.

Promotes to **Dragon king**.
{{< /shogi-move >}}

### Bishop · 角 (B)

{{< shogi-move "bishop" "Bishop · 角 (B)" >}}
Slides any distance along a diagonal.

Promotes to **Dragon horse**.
{{< /shogi-move >}}

### Gold general · 金 (G)

{{< shogi-move "gold" "Gold general · 金 (G)" >}}
Steps one square straight forward, diagonally forward, sideways or straight backward.

Does not promote.
{{< /shogi-move >}}

### Silver general · 銀 (S)

{{< shogi-move "silver" "Silver general · 銀 (S)" >}}
Steps one square straight forward or along any diagonal.

Promotes to **Promoted silver**.
{{< /shogi-move >}}

### Pawn · 歩 (P)

{{< shogi-move "pawn" "Pawn · 歩 (P)" >}}
Steps one square straight forward. It captures the same way it moves.

Promotes to **Tokin**. Promotion is compulsory on the last rank.
{{< /shogi-move >}}

### Dragon king · 龍 (+R)

{{< shogi-move "dragonKing" "Dragon king · 龍 (+R)" >}}
Slides along a rank or file. It can also step one square diagonally.

On capture it returns to the opponent’s hand as a **rook**.
{{< /shogi-move >}}

### Dragon horse · 馬 (+B)

{{< shogi-move "dragonHorse" "Dragon horse · 馬 (+B)" >}}
Slides along any diagonal. It can also step one square horizontally or vertically.

On capture it returns to the opponent’s hand as a **bishop**.
{{< /shogi-move >}}

### Promoted silver · 全 (+S)

{{< shogi-move "gold" "Promoted silver · 全 (+S)" >}}
Steps one square straight forward, diagonally forward, sideways or straight backward.

On capture it returns to the opponent’s hand as a **silver general**.
{{< /shogi-move >}}

### Tokin · と (+P)

{{< shogi-move "gold" "Tokin · と (+P)" >}}
Steps one square straight forward, diagonally forward, sideways or straight backward.

On capture it returns to the opponent’s hand as a **pawn**.
{{< /shogi-move >}}

## Further reading

[Background and examples on Wikipedia](https://en.wikipedia.org/wiki/Minishogi)
