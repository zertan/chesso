# Chesso Attack Board

A minimalist chess experience that foregrounds control. Small, shaded pieces sit on a gray/white board with coordinates on every edge, and they’re tinted red (White) or blue (Black) to match the attack overlays so you can see both the position and the pressure on every square at a glance. The board runs directly in the browser and is locked to the chess.js 1.4.0 API so all rules and move generation stay correct.

## Running
Open `index.html` in your browser. No build tools required.

## Playing
- Click your piece, then click any highlighted destination to move it. Hover over a legal destination to highlight only the opponent pieces covering that square, and ring any enemy units you would attack from there in purple.
- Click the same square again to deselect if you change your mind.
- The black side auto-plays with a selectable AI (Easy / **Medium** default / Hard). Medium favors captures and checks; Hard adds a short lookahead search.
- Browse the game so far with the ◀/▶ arrows, or hit **New Game** to reset the position and the history.
- Any piece that currently sits inside an opposing attack path is ringed in green so you can spot threats immediately.
- Turn on/off full-board shading, per-square numbers on occupied attacked squares, rings around pieces currently aiming at an enemy, and diff-only badges using the panel checkboxes.
- Pieces slide quickly and linearly into place after every move so you can track motion without heavy animation.

Color legend:
- Pink/red tint: squares controlled by White.
- Blue tint: squares controlled by Black.
- Purple tint: overlapping control from both sides.
- Deeper shading means multiple pieces aim at the same square.
- Attack badges now show only the white-minus-black difference (red for White’s edge, blue for Black’s) and can be limited to occupied attacked squares with the checkbox toggle.
