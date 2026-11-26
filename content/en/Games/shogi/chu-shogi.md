---
title: "Chu Shogi"
weight: 20
aliases: ["/games/chu-shogi/"]
description: "The lion, promotions and competition rules on the 12 × 12 board."
---

Each player starts with 46 pieces on a 12 × 12 board. Select a piece to see its destinations. Captured pieces leave play permanently. To win, capture or mate the opponent's last royal piece. Promoting the drunk elephant creates a crown prince who can carry on after the king falls.

![Starting position with international picture pieces. The lion starts beside the free king.](/games/chu-international.png)

## Reading the pieces

Open the **Game design** palette under the board. On narrow screens open **Game actions (⋯)** and select a design. **Kanji** uses the traditional characters. **International pictures** uses pictograms for each piece and its promotion. The abbreviations beside the piece names are used in move notation. **Movement diagram** shows the piece’s moves facing its own forward direction. A circle means one step, a line means any unobstructed distance, and a star marks a jump. For the lion the diagram shows all reachable squares. Its two captures and return move are explained below.

## Playing a lion move

A lion can jump up to two squares in any direction, or take two king steps in one turn. It may capture on the first step and return to its starting square. Select the destination, then choose the capture if more than one route leads there. Select the lion's square again for a return move. A return through an empty square passes the turn. Confirm the complete move with **Send move**.

For example, a lion on **f6** can take an enemy on **g7**, then an enemy on **h7**, in one turn. It can also take on **g7** and return to **f6**. A direct jump from **f6** to **h7** leaves the piece on **g7** in place.

Two adjacent lions may capture each other. From two squares away a lion may take a defended enemy lion only if its first step captures a piece other than a pawn or go-between. A non-lion that takes an enemy lion also protects its own defended lions from immediate recapture.

## Promotion and repetition

The opponent's nearest four ranks form the promotion zone. A piece can promote as it enters. After declining, it can promote on a capture from within the zone, or upon leaving and entering again. Pawns and, in correspondence play, lances have another opportunity on the last rank.

The player who initiates a repeated sequence must vary before a fourth occurrence. Perpetual check takes priority, followed by a one-sided attack. When both players repeatedly pass in place, the first to pass must vary.

See the federation's illustrated examples of lion captures and endgames. [Japanese Chu Shogi Federation competition rules](https://www.chushogi-renmei.com/kouza/rule2007.htm)


International piece artwork by CouchTomato87, rasterized for Little Golem. [Lishogi artwork](https://github.com/WandererXII/lishogi/tree/268c10c7f11d64ad306090c397bb38319c8d8cd3/ui/%40build/pieces/assets/chushogi/intl) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

WinBoard also offers a graphical mnemonic set for Chu Shogi. [HaChu author’s illustrated guide](https://hgm.nubati.net/HaChu.html)

## Piece guide

Forward is **up** in every diagram. The dark tile is the starting square. A **dot** marks a reachable square, an **arrow** means any distance on a clear line, and a **diamond** marks a jump over intervening pieces. Slides stop at the first occupied square. You may capture an opposing piece there.

The pictures beside each diagram match the **International pictures** design. Where an original and a promoted piece share a move, both pictures are shown. A promoted piece keeps its new movement for the rest of the game. Only an original, unpromoted piece can promote. For example, an original rook can become a dragon king. A gold general that has already become a rook ends its promotion there.

### Bishop · 角 (B)

{{< shogi-move "bishop" "Bishop · 角 (B)" "bishop" "leopard_promoted" >}}
Slides any distance along a diagonal.

Promotes to **Dragon horse**. Also reached by promoting the ferocious leopard.
{{< /shogi-move >}}

### Blind tiger · 虎 (BT)

{{< shogi-move "blindTiger" "Blind tiger · 虎 (BT)" "blindTiger" "" >}}
Steps one square in any direction except straight forward.

Promotes to **Flying stag**.
{{< /shogi-move >}}

### Copper general · 銅 (C)

{{< shogi-move "copper" "Copper general · 銅 (C)" "copper" "" >}}
Steps one square straight forward, diagonally forward or straight backward.

Promotes to **Side mover**.
{{< /shogi-move >}}

### Crown prince · 太 (CP)

{{< shogi-move "crownPrince" "Crown prince · 太 (CP)" "" "drunkElephant_promoted" >}}
Steps one square in any direction. It is a second royal piece. If either the prince or the king falls, the surviving royal can continue the game.

No further promotion. Reached by promoting the drunk elephant.
{{< /shogi-move >}}

### Dragon horse · 馬 (DH)

{{< shogi-move "dragonHorse" "Dragon horse · 馬 (DH)" "dragonHorse" "bishop_promoted" >}}
Slides along any diagonal. It can also step one square horizontally or vertically.

Promotes to **Horned falcon**. Also reached by promoting the bishop.
{{< /shogi-move >}}

### Dragon king · 龍 (DK)

{{< shogi-move "dragonKing" "Dragon king · 龍 (DK)" "dragonKing" "rook_promoted" >}}
Slides along a rank or file. It can also step one square diagonally.

Promotes to **Soaring eagle**. Also reached by promoting the rook.
{{< /shogi-move >}}

### Drunk elephant · 象 (DE)

{{< shogi-move "drunkElephant" "Drunk elephant · 象 (DE)" "drunkElephant" "goBetween_promoted" >}}
Steps one square in any direction except straight backward.

Promotes to **Crown prince**. Also reached by promoting the go-between.
{{< /shogi-move >}}

### Ferocious leopard · 豹 (FL)

{{< shogi-move "leopard" "Ferocious leopard · 豹 (FL)" "leopard" "" >}}
Steps one square straight forward, straight backward or along any diagonal.

Promotes to **Bishop**.
{{< /shogi-move >}}

### Flying ox · 牛 (FO)

{{< shogi-move "flyingOx" "Flying ox · 牛 (FO)" "" "verticalMover_promoted" >}}
Slides straight forward, straight backward or along any diagonal.

No further promotion. Reached by promoting the vertical mover.
{{< /shogi-move >}}

### Flying stag · 鹿 (FS)

{{< shogi-move "flyingStag" "Flying stag · 鹿 (FS)" "" "blindTiger_promoted" >}}
Slides in either direction on its file. It may also step one square sideways or on any diagonal.

No further promotion. Reached by promoting the blind tiger.
{{< /shogi-move >}}

### Free boar · 猪 (FB)

{{< shogi-move "freeBoar" "Free boar · 猪 (FB)" "" "sideMover_promoted" >}}
Slides sideways or along any diagonal.

No further promotion. Reached by promoting the side mover.
{{< /shogi-move >}}

### Free king (queen) · 奔 (FK)

{{< shogi-move "queen" "Free king (queen) · 奔 (FK)" "queen" "phoenix_promoted" >}}
Slides any distance along a rank, file or diagonal.

No further promotion. Reached by promoting the phoenix.
{{< /shogi-move >}}

### Go-between · 仲 (GB)

{{< shogi-move "goBetween" "Go-between · 仲 (GB)" "goBetween" "" >}}
Steps one square straight forward or straight backward.

Promotes to **Drunk elephant**.
{{< /shogi-move >}}

### Gold general · 金 (G)

{{< shogi-move "gold" "Gold general · 金 (G)" "gold" "pawn_promoted" >}}
Steps one square straight forward, diagonally forward, sideways or straight backward.

Promotes to **Rook**. Also reached by promoting the pawn.
{{< /shogi-move >}}

### Horned falcon · 鷹 (HF)

{{< shogi-move "hornedFalcon" "Horned falcon · 鷹 (HF)" "" "dragonHorse_promoted" >}}
Slides on all four diagonals, sideways and straight backward. Straight forward it may step once, jump two squares, or take the adjacent piece and continue one more square forward or return home. It may also step to an empty adjacent square in that direction and return, passing the turn.

No further promotion. Reached by promoting the dragon horse.
{{< /shogi-move >}}

### King · 玉 (K)

{{< shogi-move "king" "King · 玉 (K)" "king" "" >}}
Steps one square in any direction. It is a royal piece.

No further promotion.
{{< /shogi-move >}}

### Kirin · 麒 (Kr)

{{< shogi-move "kirin" "Kirin · 麒 (Kr)" "kirin" "" >}}
Steps one square diagonally, or jumps exactly two squares along a rank or file. A jump passes over the intervening square.

Promotes to **Lion**.
{{< /shogi-move >}}

### Lance · 香 (L)

{{< shogi-move "lance" "Lance · 香 (L)" "lance" "" >}}
Slides any distance straight forward.

Promotes to **White horse**.
{{< /shogi-move >}}

### Lion · 獅 (Ln)

{{< shogi-move "lion" "Lion · 獅 (Ln)" "lion" "kirin_promoted" >}}
Moves anywhere within two king steps. It can jump directly over an occupied square, or make two successive steps, changing direction between them. The first step can capture; the second can capture again or return to the starting square.

No further promotion. Reached by promoting the kirin.
{{< /shogi-move >}}

### Pawn · 歩 (P)

{{< shogi-move "pawn" "Pawn · 歩 (P)" "pawn" "" >}}
Steps one square straight forward. It captures the same way it moves.

Promotes to **Gold general**.
{{< /shogi-move >}}

### Phoenix · 鳳 (Ph)

{{< shogi-move "phoenix" "Phoenix · 鳳 (Ph)" "phoenix" "" >}}
Steps one square along a rank or file, or jumps exactly two squares diagonally over the intervening square.

Promotes to **Free king (queen)**.
{{< /shogi-move >}}

### Reverse chariot · 反 (RC)

{{< shogi-move "reverseChariot" "Reverse chariot · 反 (RC)" "reverseChariot" "" >}}
Slides any distance straight forward or backward along its file.

Promotes to **Whale**.
{{< /shogi-move >}}

### Rook · 飛 (R)

{{< shogi-move "rook" "Rook · 飛 (R)" "rook" "gold_promoted" >}}
Slides any distance along a rank or file.

Promotes to **Dragon king**. Also reached by promoting the gold general.
{{< /shogi-move >}}

### Side mover · 横 (SM)

{{< shogi-move "sideMover" "Side mover · 横 (SM)" "sideMover" "copper_promoted" >}}
Slides any distance sideways. It can also step one square straight forward or backward.

Promotes to **Free boar**. Also reached by promoting the copper general.
{{< /shogi-move >}}

### Silver general · 銀 (S)

{{< shogi-move "silver" "Silver general · 銀 (S)" "silver" "" >}}
Steps one square straight forward or along any diagonal.

Promotes to **Vertical mover**.
{{< /shogi-move >}}

### Soaring eagle · 鷲 (SE)

{{< shogi-move "soaringEagle" "Soaring eagle · 鷲 (SE)" "" "dragonKing_promoted" >}}
Slides in six directions: along ranks and files and on both backward diagonals. On either forward diagonal it may step once, jump two squares, or capture on the adjacent square and continue on the same diagonal or return home. It may also step to an empty adjacent square in that direction and return, passing the turn.

No further promotion. Reached by promoting the dragon king.
{{< /shogi-move >}}

### Vertical mover · 竪 (VM)

{{< shogi-move "verticalMover" "Vertical mover · 竪 (VM)" "verticalMover" "silver_promoted" >}}
Slides any distance straight forward or backward. It can also step one square sideways.

Promotes to **Flying ox**. Also reached by promoting the silver general.
{{< /shogi-move >}}

### Whale · 鯨 (W)

{{< shogi-move "whale" "Whale · 鯨 (W)" "" "reverseChariot_promoted" >}}
Slides in either direction on its file and along either backward diagonal.

No further promotion. Reached by promoting the reverse chariot.
{{< /shogi-move >}}

### White horse · 駒 (WH)

{{< shogi-move "whiteHorse" "White horse · 駒 (WH)" "" "lance_promoted" >}}
Slides in either direction on its file and along either forward diagonal.

No further promotion. Reached by promoting the lance.
{{< /shogi-move >}}
