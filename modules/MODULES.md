# Nine professional modules

All modules are enabled by default and loaded on demand. Each has independent version, dependencies, capability needs, tests and disable-impact notes.

1. **Web Development:** HTML5, CSS, JS/TS, responsive UI, forms, routing, state, browser storage, accessibility.
2. **2D Game Development:** Canvas/WebGL, characters, animation, collision, maps, levels, input and saves.
3. **3D Game Development:** Three.js, scenes, terrain, models, lighting, materials, camera, world chunks and resource lifecycle; WebGPU optional.
4. **3D Workbench:** scene/object editing, selection, transforms, property panels, terrain, asset management, skeleton workflow and export.
5. **Physics Engine:** Physics Core, Vehicle, Character, Environment and Destruction Physics; Rapier may provide primitives.
6. **Animation System:** skeletons, keyframes, state machines, blending, IK and events.
7. **AI Game Logic:** NPC state machines, behavior trees, pathfinding, perception, dialogue and quests.
8. **Testing & Repair:** unit/integration/interaction/visual/performance/regression tests, root-cause repair and bounded retries.
9. **Deployment & Git:** build, package, branches, commits, GitHub, deployment and delivery.

Do not load unrelated dependencies. Verify movement/collision/restart for 2D; assets/collision/FPS/memory for 3D; units/gravity/contact/stability for physics; secrets/approval/rollback for deployment.
