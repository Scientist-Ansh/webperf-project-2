**General requirements:**

- [x] Get rid of duplicate lodash in our bundles.
- [x] Switch to tree-shared lodash imports.
- [x] Code-split each route to have its own bundle.
      ** Frontpage requirements: **
- [x] Use `contain` and `content-visibility` for “everything” below the fold.
- [x] Fix layout shifting of the hero image with HTML/CSS.
- [x] Don’t lazy load the Hero section (Fix JS waterfall).
- [x] Lazy load the entire Form component.
- [ ] Only load the phone number validation if I’m actually interacting with the form.
- [x] Replace moment.js with a smaller date library (which supports tree-shaking?).
- [x] Ignore side-effects in the News component.
      ** Videogame requirements: **
- [ ] Move entities with transform instead of left/top (so it can skip layout/paint).
- [ ] Create GPU layers for all entities so they composite on the GPU (“will-change”).
- [ ] Improve removeDeadEntities to be O(n) instead of O(n^2).
- [ ] Get rid of unnecessary re-paints in the game “status” element (in the corner).
- [ ] Eliminate constant repaints when switching between levels. Don’t animate background-color. Instead animate opacity of 2 differently coloured elements.
- [ ] Optimise game elements with `contain` style.
- [ ] Get rid of forced reflows when moving entities (don’t read and write constantly, either store locations in JS or batch the reads/writes).
- [ ] Optimise collision detection to be “O(n) + O(s\*e)” where `s` is the number of shots and `e` is the number of enemies (only check if shots collide with enemies).
      ** Either: **
- [ ] Hide “dead” elements with opacity and remove them from the DOM in the end of the level.
- [ ] Remove “dead” elements from the DOM after collision detection is finished.
      ** Extra challenges (max 2): **
- [ ] Reimplement the game graphics with Canvas.
- [ ] Rewrite position and collision detection to not read ANYTHING from the DOM.
- [ ] Implement pooling of entities (instead of removing them from the DOM, just hide them, and reuse them later instead of creating a new element).
- [ ] Make the game better. Add features/graphics/audio.
