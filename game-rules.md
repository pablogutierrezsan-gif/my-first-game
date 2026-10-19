# Alien Tic-Tac-Toe: rules and states

| State | Player sees | Allowed action → result |
| --- | --- | --- |
| Instructions | Goal, counter table, Start | Start → empty board. Nothing happens before Start. |
| Choose a square | Board, "Choose an empty square" | Pick an empty square → battle starts, board locks. |
| Choose a response | Pending square, both health values, alien's move | One response → one damage result, responses lock. |
| Exchange feedback | What happened, updated health | Next exchange (only if both have health). |
| Battle over, board continues | Square marked, battle summary | Return to board → only empty squares unlock. No extra mark. |
| Board over | Final board, result | Play again → fresh empty board. |
| Any active state | Restart game button | Clears board, battle, health, feedback → empty board. |

Win lines: 1-2-3, 4-5-6, 7-8-9, 1-4-7, 2-5-8, 3-6-9, 1-5-9, 3-5-7.
Check for a line before declaring a draw.
Reopening help keeps the current board and battle as they were.
