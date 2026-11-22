# Nine professional modules / 九大专业模块

All modules are enabled at product level and loaded only when relevant. Each module supports the One-Sentence Build Mode by turning a short product brief into concrete implementation requirements and acceptance checks.

所有模块在产品层默认启用，但只按任务需要加载。每个模块都必须支持“一句话构建模式”，把简短需求转成可执行实现与验收要求。

1. **Web Development:** HTML5, CSS, JS/TS, responsive UI, information architecture, forms, routing, state, storage, accessibility, SEO/performance. A one-sentence website brief should produce a complete, navigable and responsive product, not merely a hero screen.
2. **2D Game Development:** Canvas/WebGL, game loop, input mapping, characters, animation, collision, maps, levels, core loop, pause/restart/completion and saves. A one-sentence game brief should become a complete playable vertical slice.
3. **3D Game Development:** Three.js, scene scale, camera, lighting, materials, procedural geometry/terrain, models, collision, world boundaries, world chunks and resource lifecycle; WebGPU optional. Deliver a coherent 3D playable scene with readable framing and real interaction.
4. **3D Workbench:** scene/object editing, selection, transforms, property panels, terrain, asset management, skeleton workflow, undo/redo where appropriate and export. The core create/select/edit/save/export workflow must work.
5. **Physics Engine:** Physics Core, Vehicle, Character, Environment and Destruction Physics; Rapier may provide primitives. Define units, gravity, timestep, contacts, collision filters, stability and regression cases appropriate to the brief.
6. **Animation System:** skeletons, keyframes, state machines, blending, IK, events and transition timing. Animation must communicate state and respond to actual game/application events.
7. **AI Game Logic:** NPC state machines, behavior trees, pathfinding, perception, dialogue and quests. Use deterministic/simple local logic where no authorized AI API exists; never fake remote intelligence.
8. **Testing & Repair:** acceptance criteria, unit/integration/interaction/visual/performance/regression tests, runtime checks, root-cause repair and bounded retries. Build tests from the original one-sentence brief.
9. **Deployment & Git:** build, package, version control, GitHub workflows, deployment and delivery. Do not publish or deploy without approval.

## Cross-module delivery gate / 跨模块交付门槛
The chosen modules must compose into one working user experience. Validate entry → primary interaction → meaningful outcome → reset/return/recovery. Avoid disconnected feature fragments and visually polished but inert UI.

各模块必须组合成完整体验，验证“进入 → 核心交互 → 有意义结果 → 重开/返回/恢复”，避免模块互不关联或只有视觉效果、没有实际行为。
