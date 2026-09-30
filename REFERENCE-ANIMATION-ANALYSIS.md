# Reference animation analysis — 2026-10-01

Source supplied by user: 1320×1404 GIF, 12 GIF frames, 100 ms per GIF frame, looping.

## What the sheet teaches us
The reference is a character-sheet presentation containing separate animation families: STANDING, RUN, JUMP, ATTACK-SWORD, ATTACK-HAMMER, ATTACK-LANCE. It uses readable key poses, anticipation, contact, follow-through, recovery, smear/FX frames, and consistent ground baselines.

## What BANANA should adopt (technique, not the other character artwork)
- State machine: IDLE / RUN / JUMP_RISE / APEX / FALL / LAND / ACTION / REWIND.
- RUN: 8-phase loop with wider contact poses and faster playback than idle.
- JUMP: do not loop a walk sprite in air. Use rise, apex, fall and landing phases.
- LAND: short squash only; MASTER identity pixels stay unchanged.
- ACTION: PEEL DASH is BANANA's original action. Fast startup, burst, recovery.
- FX layer must be separate from character pixels so effects never corrupt MASTER.
- Ground anchor stays fixed; animation is measured from the feet.
- MASTER face/stem/core silhouette remain protected.

## Verified source facts
- GIF dimensions: 1320×1404
- GIF frames: 12
- nominal frame duration: 100 ms
- loop: infinite

## Production target
1. Finalize RUN 8 key poses.
2. Author dedicated jump frames.
3. Add landing dust as separate FX.
4. Add PEEL DASH anticipation/impact/recovery frames.
5. Add animation event markers (footstep, takeoff, landing, dash impact).
6. Move animation data out of index.html into canonical assets/animation-data.js.
