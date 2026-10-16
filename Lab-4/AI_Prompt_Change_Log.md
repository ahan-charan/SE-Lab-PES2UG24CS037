# Lab 4 AI Prompt / Change Log

**Student:** Ahan Charan  
**SRN:** PES2UG24CS037  
**Assigned game:** Pac-Man (Pygame)

## Source inspected

- Assigned game: https://github.com/SETAPESU26/34_pacman
- Personal lab repository: https://github.com/ahan-charan/SE-Lab-PES2UG24CS037
- The assigned README specifies one deliberate bug and three empty feature functions.

## Main debugging finding

The maze contains power pellets as lowercase `o`, but `Game.eat()` originally checked for uppercase `O`. Because those characters never match, eating a power pellet only awarded the normal pellet points and did not activate frightened mode.

## Implementation decisions

- Corrected the marker comparison to lowercase `o`.
- Added distinct frightened-mode colours for Blinky, Pinky, Inky, and Clyde.
- Made the pellet callback flash the HUD briefly on the final pellet.
- Chose a 1,000-point extra-life threshold so it can plausibly be reached in the small maze; 10,000 points is unlikely to be reached given the board's pellet count.

## Prompt record for this session

1. User provided the Lab 4 VibeCoding handout and said the assigned game is Pac-Man, linking the course repository and the personal SE lab repository.
2. Assistant inspected the game README and `game.py`, identified the lowercase/uppercase power pellet bug, and listed the three unfinished functions.
3. Assistant prepared the changes above and attempted to add `Lab-4/game.py` to the personal repository. The connected GitHub integration returned a 403 permission error, so no repository write was completed by this session.

## Before submission

Please export the actual conversation from the AI interface if your instructor requires the full chat history, and add your own before/after screen recordings. This change log is a summary and is not a substitute for the full conversation export or videos.
