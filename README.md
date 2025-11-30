# Chesso Attack Board

A minimalist chess experience that foregrounds control. Small, shaded pieces sit on top of tinted attack maps so you can see both the position and the pressure on every square at a glance.

## Running
Open `index.html` in your browser. No build tools required.

## Playing
- Click your piece, then click any highlighted destination to move it.
- The black side auto-plays with a simple capture-seeking AI after each of your moves.
- Use **Undo** to step back (it undoes your move and the AI reply) or **New Game** to reset the position.

Color legend:
- Pink/red tint: squares controlled by White.
- Blue tint: squares controlled by Black.
- Purple tint: overlapping control from both sides.
- Deeper shading means multiple pieces aim at the same square.
- Number tags show how many pieces (from either side) currently attack each square.
