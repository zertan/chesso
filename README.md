# Chesso Attack Board

A minimalist chess experience that foregrounds control. Small, shaded pieces sit on a gray/white board with coordinates on every edge, and they’re tinted red (White) or blue (Black) to match the attack overlays so you can see both the position and the pressure on every square at a glance. The board runs directly in the browser and is locked to the chess.js 1.4.0 API so all rules and move generation stay correct.

## Running
Open `index.html` in your browser. No build tools required.

## Playing
- Click your piece, then click any highlighted destination to move it.
- Click the same square again to deselect if you change your mind.
- The black side auto-plays with a simple capture-seeking AI after each of your moves.
- Use **Undo** to step back (it undoes your move and the AI reply) or **New Game** to reset the position.
- Any piece that currently sits inside an opposing attack path is ringed in green so you can spot threats immediately.
- Turn on/off full-board shading, per-square numbers on occupied attacked squares, and rings around pieces currently aiming at an enemy using the panel checkboxes.

Color legend:
- Pink/red tint: squares controlled by White.
- Blue tint: squares controlled by Black.
- Purple tint: overlapping control from both sides.
- Deeper shading means multiple pieces aim at the same square.
- Attack badges now show only the white-minus-black difference (red for White’s edge, blue for Black’s) and can be limited to occupied attacked squares with the checkbox toggle.
