# Checkmate Quest

A kid-friendly chess game that runs in the browser as a single `index.html` file, with no build step and no server.

**Play it:** https://jooziv.github.io/checkmate-quest/

## Play chess
- 2 players on one screen, or you vs the computer (Very Easy, Beginner, Easy, Medium, Hard)
- Full rules: castling, en passant, promotion, check, checkmate and draws (stalemate, threefold repetition, 50-move rule, insufficient material)
- Undo, flip board, captured pieces and move list
- **Resume codes:** every game has a code such as `G-C2W-2F2G2F25-2823`. It is kept in the page address and updates after every move, so reopening the link continues the game. You can also paste a code into the Resume box.

## Puzzles
- Checkmate-in-1, 2 and 3 puzzles generated from a code (for example `M2-BRAVE-OTTER-47`)
- The same code always makes the same puzzle, and each puzzle has exactly one winning first move
- Hints, stars and streaks

## How the codes work
- **Game codes** record the game type, computer level and your color, then each move as its position in a fixed, sorted list of the legal moves.
- **Puzzle codes** seed a random generator. A chess solver keeps generating positions until one has a forced mate in exactly N moves with a single winning first move.

Progress such as stars and your record against the computer is saved in your browser's local storage.
