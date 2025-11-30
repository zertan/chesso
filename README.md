# Chesso Attack Board

A minimalist chess experience focused entirely on control. Pieces stay hidden while their attack paths paint the board, letting you explore pressure, overlaps, and heat on every square.

## Running
Open `index.html` in your browser. No build tools required.

## Playing
- Click any square to reveal what piece (if any) occupies it and show its legal moves.
- Click a highlighted destination to move the hidden piece; the attack shading updates instantly.
- Use **Undo** to step back or **New Game** to reset the position.

Color legend:
- Pink/red tint: squares controlled by White.
- Blue tint: squares controlled by Black.
- Purple tint: overlapping control from both sides.
- Deeper shading means multiple pieces aim at the same square.
