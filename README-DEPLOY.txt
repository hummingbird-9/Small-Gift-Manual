SMALL-GIFT MANUAL — CAR TEST GROUNDS

This is a static, root-deployable Three.js driving sandbox. It loads supported vehicles from ./models/cars/viewer-manifest.json and the model files in this repository.

DEPLOY
- Keep index.html at the repository root.
- Keep models/cars/ and its category folders at the same root level.
- GitHub Pages: Settings > Pages > Deploy from a branch > main > /(root).
- The viewer uses Three.js 0.166.1 modules from jsDelivr. The page and model assets are served from GitHub Pages; the library requires internet access.

CONTROLS
- On foot: WASD / arrow keys to move, Shift to walk faster, E beside a car to enter.
- Driving: W / Up to accelerate, S / Down to brake/reverse, A/D or arrows to steer, Space to handbrake/drift, Shift to brake, R to recover and repair the current vehicle, E to exit.
- Mouse drag to orbit, wheel to zoom, right-drag to pan.

IMPLEMENTED SYSTEMS
- Procedural rolling terrain, oval asphalt test track, lane marks, pit apron, instanced trees and rocks.
- Placeholder third-person character with a basic walk cycle.
- Enter/exit vehicles and third-person follow camera.
- Per-vehicle acceleration/top-speed presets, lateral grip, handbrake drift, braking/reverse.
- Four-corner terrain sampling, spring/damper chassis movement, pitch and body roll.
- Tree and parked-vehicle collisions, basic localized mesh dents, damage state, reduced power at high damage, recover/repair.
- Texture path resolution by asset basename, missing-map paint fallback for affected OBJ/MTL materials, vertex-normal fallback, double-sided body panels.
- Performance defaults: capped pixel ratio, no real-time shadow maps, instanced scenery, sequential model loading, bounded terrain mesh.

MODEL NOTES
- 18 browser-supported models are listed in the manifest (FBX, OBJ/MTL, GLB and DAE).
- Blender-only .blend sources and unextracted RAR-only downloads are excluded from the playable roster because browsers cannot load them directly.
- This is an early arcade-style foundation, not a full vehicle simulator. Wheel travel is approximated by chassis spring motion and body pitch/roll; handling values can be tuned after testing. The character is a temporary placeholder for your custom model.
