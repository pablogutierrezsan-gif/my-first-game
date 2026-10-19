# Alien Tic-Tac-Toe: game brief

## Concept
A solo tic-tac-toe where you fight a short alien battle for every square. Win the battle, claim X. Lose, the alien claims O.

## Player
Anyone; one round takes a few minutes.

## How it works
- 3x3 board. Pick any empty square; the board locks and a battle starts for that square.
- Win the battle: X goes in that square. Lose: O goes there.
- No automatic opponent move. One battle fills exactly one square.
- Three X in a line wins the board. Three O loses it. Full board with no line is a draw.
- Restart game is always available and clears the whole board and any battle.

## Battle
- You: 2 health. Alien: 2 health.
- Alien moves in a fixed order every battle: Laser, then Shield, then Claw.
- Correct counters: Laser → Shield, Shield → Blast, Claw → Dodge.
- Correct answer: alien loses 1. Wrong answer: you lose 1.
- One answer per exchange, then a Next exchange button (only if both sides still have health).
- First side to 0 loses. Battles last 2 or 3 exchanges; never a draw.

## Controls
Standard buttons only: mouse, touch, and keyboard (Tab + Enter/Space).

## Not in version 1
Timers, random alien moves, sound, downloaded art, logins, saved scores, extra levels.

## Completion checks
1. Winning a battle puts exactly one X in the chosen square; losing puts one O.
2. Occupied squares can't be picked, and the board is locked during a battle.
3. Three X in a line shows "You won"; three O shows "The aliens won"; full board with no line shows "Draw".
4. Rapid repeated clicks during a battle cause only one damage event per exchange.
5. Restart game, mid-battle or after a result, returns an empty board with no leftover battle.
