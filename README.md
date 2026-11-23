# Miracle Core

The shared toolbox both Miracle editors pull from: style packs, the effects library, the sound library, brand kits,
the Animator and voiceover. Miracle Lite (reels, `miracle-editor`) and Miracle Pro (podcasts, `miracle-podcast`)
each load what their tier allows.

Status: started Nov 23, 2026. First piece: `styles/vox/test/`, a 10-second proof that the Vox archival look renders
with HyperFrames (paper collage, stamped date, line-drawn press, counter, marker with a note, a pan, a map of presses
spreading from Mainz). The sound library and effects move here from miracle-editor next.

## Render the Vox test scene
```bash
cd styles/vox/test
HYPERFRAMES_SKIP_SKILLS=1 DO_NOT_TRACK=1 ../../../../miracle-editor/hyperframes/node_modules/.bin/hyperframes render --fps 30 -o out/scene.mp4
```
Sound and film grain are mixed after the render from miracle-editor's `sfx/` library (moves here with the library).
