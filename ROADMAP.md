# BANANA — Production Roadmap

## Character law
The uploaded 48×48 MASTER is immutable for identity: face, eyes, mouth, stem, palette and core silhouette are the source of truth.

## Current
- [x] MASTER reconstructed as 48×48 pixel data
- [x] MASTER LOCK animation studio
- [x] 8-frame animation workspace
- [x] GitHub Actions structural guard
- [x] First in-game 8-frame WALK prototype
- [x] PEEL BACK time-rewind mechanic

## Next animation pass
1. Refine WALK contact/down/passing/up poses by pixel diff.
2. Add IDLE breathing without scaling the whole sprite.
3. Add JUMP anticipation / rise / fall / land.
4. Add SIT transition + SIT idle.
5. Export approved frames into a single canonical animation-data file.

## Quality gate
No frame is accepted if the character identity changes. Animation comes from motion of selected pixels, not regeneration of the character.
