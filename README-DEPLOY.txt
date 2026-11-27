CAR MODEL LINEUP - GITHUB PAGES ROOT TESTER

This package is arranged to extract into the ROOT of the Small-Gift-Manual repository.
It adds:
  index.html
  models/cars/viewer-manifest.json
  models/cars/<category>/<vehicle-folder>/...
  models/cars/credits/...

The page uses relative paths and can be deployed from the repository's main branch root.
It uses Three.js 0.166.1 modules from jsDelivr, so browsers need internet access to fetch the viewer library.
The 3D model and texture files themselves are loaded from this repository.

GITHUB PAGES
1. Extract this package in the repository root (merge folders; do not extract into a subfolder).
2. Commit and push index.html and models/.
3. In the repository's Settings > Pages, choose Deploy from a branch, branch main, folder / (root).
4. Open the Pages URL. For a project repository, the relative file paths continue to work under /Small-Gift-Manual/.

CONTROLS
- Drag: orbit
- Scroll: zoom
- Right-drag: pan
- Fit all: frame the full lineup
- Select a model name along the bottom: move the camera to that vehicle

BROWSER SUPPORT
18 model entries are configured for the viewer: FBX, OBJ/MTL, GLB, and DAE.
The 2 Blender .blend files are included but need exporting to GLB/GLTF before browser viewing.
The two old rusty-car items are preserved as RAR archives; their models have not been extracted.
The vehicle source files and textures retain their original relative folder structure inside each category.

NOTE
This is a static viewer. No build step, workflow, backend, or dedicated deploy folder is needed.
