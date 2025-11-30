# Chesso Attack Board

A minimalist chess experience that foregrounds control. Small, shaded pieces sit on top of tinted attack maps so you can see both the position and the pressure on every square at a glance. The board runs directly in the browser and is locked to the chess.js 1.4.0 API so all rules and move generation stay correct.

## Running
Open `index.html` in your browser. No build tools required.

## Playing
- Click your piece, then click any highlighted destination to move it.
- Click the same square again to deselect if you change your mind.
- The black side auto-plays with a simple capture-seeking AI after each of your moves.
- Use **Undo** to step back (it undoes your move and the AI reply) or **New Game** to reset the position.

Color legend:
- Pink/red tint: squares controlled by White.
- Blue tint: squares controlled by Black.
- Purple tint: overlapping control from both sides.
- Deeper shading means multiple pieces aim at the same square.
- Attack badges show white and black attack counts side-by-side (pink for White, blue for Black) with the center value showing the white-minus-black edge on that square.
