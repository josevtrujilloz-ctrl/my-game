# Game improvement board

Move stories from Backlog to Doing to Done. Limit: one story in Doing.
Done requires checking the deployed game against its acceptance criteria.

## Doing

No stories currently in progress.

## Done

Priority decision: the visual improvement benefits laptop and phone viewers and reuses existing controls. Phone play requires new input controls and device testing. A visual redesign alone does not enable touch play.

### 1. A more appealing snake

As a player, I want a more visually appealing snake, so that the game feels more enjoyable to play.

Chosen visual direction: a more realistic, scary snake within the game's simple graphics.

Acceptance criteria:
1. The snake has a tapered head, visible eyes, and a forked tongue.
2. Its body has a dark green scale pattern.
3. Arrow controls, scoring, collisions, and Restart still work as specified in SPEC.md.

Implemented and deployed in commit ba1bf35. SPEC.md now describes the approved appearance; its other requirements were preserved.

Live verification completed with the student:
- Confirmed the new appearance, one-point/one-segment pellet growth, and replacement food in an empty space.
- Confirmed all arrow directions, prevention of immediate reversal, wall collision, and the game-over statistics.
- Confirmed Restart restores four segments, score 0 and timer 0:00 while preserving best score; timer waits for an arrow key.
- Confirmed self-collision ends the game and movement is smooth in the active browser tab.

Independent reviewer tested the live URL in Chrome and corroborated the appearance, controls, a pellet collection, wall collision, end display, and Restart. Self-collision was inconclusive in that review, and background-tab throttling prevented a fair smoothness check; the student verified both on production. The student checked each reviewer finding before accepting it.

## Backlog

### 2. Play on a phone

As a player on a phone, I want to control the snake without a keyboard, so that I can play on the device I have with me.

Acceptance criteria:
1. On a phone without a keyboard, the player can start and steer in all four directions.
2. The board, score, and Restart button remain usable on a phone screen.
3. Restart resets the round while preserving best score, and desktop arrow controls still work.

### 3. Understand the timer

As a player, I want to understand what the timer measures, so that I know whether I am racing against time.

Source: Players 2 and 4 in FEEDBACK.md. Future candidate; not started.

Acceptance criteria:
1. Before starting, the player can find a plain-language explanation that the timer measures elapsed playing time, not a countdown or time limit.
2. In a follow-up playtest, the player can correctly explain whether the timer affects losing the game.

### Ideas needing clarification

- Player 2: increasing challenge or another target beyond personal best.
- Players 4 and 5: variety and rewards for replay or risk.
- Players 3 and 5: best-score motivation. Ask Player 3 what felt missing from the existing Restart button and best-score display.

These ideas need further scoping before becoming implementation stories. No additional game changes are part of the completed snake story.

