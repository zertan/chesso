# Chesso Attack Board

A minimalist chess experience that foregrounds control. Small, shaded pieces sit on a gray/white board with coordinates on every edge, and they’re tinted red (White) or blue (Black) to match the attack overlays so you can see both the position and the pressure on every square at a glance. The board runs directly in the browser and is locked to the chess.js 1.4.0 API so all rules and move generation stay correct.

## Running
Open `index.html` in your browser. No build tools required. Use the − / + controls to resize the board between 6×6, 8×8, 9×9, and 10×10 layouts; each size regenerates the starting position to match.

## Playing
- Click your piece, then click any highlighted destination to move it. Hover over a legal destination to highlight only the opponent pieces covering that square, and ring any enemy units you would attack from there in purple. Promotions auto-queen on the farthest rank for non-standard sizes.
- Click the same square again to deselect if you change your mind.
- The black side auto-plays with a selectable AI (Easy / **Medium** default / Hard). Medium favors captures and checks; Hard adds a short lookahead search.
- Browse the game so far with the ◀/▶ arrows, or hit **New Game** to reset the position and the history. Changing the board size resets the game into the closest symmetrical layout for that dimension.
- Any piece that currently sits inside an opposing attack path is ringed in green so you can spot threats immediately.
- Turn on/off full-board shading, per-square numbers on occupied attacked squares, rings around pieces currently aiming at an enemy, and diff-only badges using the panel checkboxes.
- Pieces slide quickly and linearly into place after every move so you can track motion without heavy animation.

Color legend:
- Pink/red tint: squares controlled by White.
- Blue tint: squares controlled by Black.
- Purple tint: overlapping control from both sides.
- Deeper shading means multiple pieces aim at the same square.
- Attack badges now show only the white-minus-black difference (red for White’s edge, blue for Black’s) and can be limited to occupied attacked squares with the checkbox toggle.

### Variant layouts and extra pieces

- **6×6** drops two files and uses: R N B Q K R on the back rank with a single pawn line.
- **8×8** uses standard chess driven by chess.js 1.4.0.
- **9×9** introduces the **Archbishop (A)**, which moves as a bishop *or* a knight.
- **10×10** adds the **Chancellor (C)**, which moves as a rook *or* a knight; the back rank is R N B Q K C B A N R.
