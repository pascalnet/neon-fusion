# NEON FUSION

**Play it live: https://pascalnet.github.io/neon-fusion/**

A neon physics merge game rendered entirely with WebGL shaders. Drop glowing plasma orbs into the reactor: two identical orbs **fuse** into a bigger one, and fast back-to-back fusions build a **chain multiplier**. Fill the FEVER meter for double points, discover all 11 orbs, and don't let the pile sit over the red line.

## Controls
- **Mouse / touch**: aim, release to drop
- **Keyboard**: ← → (or A/D) to aim, Space to drop
- **1 / 2 / 3**: Bomb / Prism / Quake power-ups
- **M**: mute, **R**: instant restart

## What's inside
- Custom 2D rigid-body solver: 8 substeps, sequential impulses with restitution, Coulomb friction and rolling (angular velocity), speculative contacts and position projection for stable stacks
- Metaball field rendering (gooey orbs that bridge when touching), animated nebula background, 3-level HDR bloom, shockwave distortion, chromatic aberration, flashes and film grain, all in GLSL (WebGL2 with WebGL1 fallback)
- Dopamine loop: chain combos with rising pentatonic pitch, score popups, screen shake, hit-stop and slow-mo, particle bursts that bounce off orbs, FEVER mode with music, drop streaks, level-ups with power-up rewards, orb discoveries, close-call bonuses, walls that squeeze in as you level up
- All sound effects are synthesized live with WebAudio, so there are no audio files
- Best score, best chain and discovered orbs persist in localStorage

A single self-contained `index.html` with no build step.
