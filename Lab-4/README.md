# Lab 4 — VibeCoding: Pac-Man

**Student:** Ahan Charan  
**SRN:** PES2UG24CS037  
**Source repository:** https://github.com/SETAPESU26/34_pacman  
**Personal repository:** https://github.com/ahan-charan/SE-Lab-PES2UG24CS037

## Changes made

1. Fixed the power pellet comparison: the maze uses lowercase `o`, so `eat()` must compare against `"o"`; it now activates frightened mode, awards the power-pellet points, and reverses eligible ghosts.
2. Implemented `ghost_color(name, mode)` with a distinct colour for each ghost during frightened mode. Other modes keep the existing colour logic.
3. Implemented `on_pellet_eaten(score, pellets_left)` to trigger an approximately 1.5-second HUD flash when the final pellet is collected.
4. Implemented `bonus_life_threshold()` to return 1,000 points, a more reachable threshold for this small maze than 10,000. The existing bookkeeping awards one life at each crossed threshold.

## Run

Install Python 3.10 or newer, then run:

```bash
python -m pip install pygame
python game.py
```

Use arrow keys to move and `R` to reset.

## Still required for submission

- Record a 10-second gameplay video before changes, clearly demonstrating that the power-pellet bug exists. Do this from the original course repository before replacing anything.
- Record a 10-second gameplay video after changes, showing frightened mode and the new colour behavior. Also show the final-pellet HUD flash if practical.
- Push the code and required evidence to your personal repository under `Lab-4/`.
- Export the actual AI conversation used for this lab as a PDF or document, as requested by your course handout.

**Note:** The video recordings must be captured on your computer. This package does not contain fabricated videos or claims that those recordings have been made. The current connected GitHub integration denied repository writes, so these files have not been pushed to GitHub by this session.
