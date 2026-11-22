# Engineering Standards / 工程标准

## One-Sentence Build Mode / 一句话构建模式

A single natural-language sentence asking for a website, web app, 2D/3D game or interactive tool is a complete creative brief to begin implementation. Do not require the user to provide a long specification or answer a form. Infer safe, non-blocking details from the sentence and context; ask at most one question only for a true blocker, major product ambiguity or approval gate.

用户只需一句自然语言描述网站、Web 应用、2D/3D 游戏或交互工具，即可触发实际构建。不得要求用户先写长规格或填写问卷。结合上下文补全安全且不阻塞开发的细节；只有遇到真正阻塞、重大方向歧义或审批事项时才问一个问题。

**Default result:** a complete, runnable first release/vertical slice—not a plan-only answer, wireframe-only design, empty scaffold or decorative demo. Main buttons, forms, controls and game states must perform real behavior. The detailed contract is in [ONE_SENTENCE_BUILD.md](ONE_SENTENCE_BUILD.md).

## Seven review roles
Project Manager/Game Director: scope, milestones, risks, approvals, acceptance and delivery. Architect: stack, boundaries, data, interfaces and migrations. Web Engineer: UI, responsive behavior, accessibility and browser compatibility. Game Engineer: gameplay, scene, camera, controls and progression. Physics Engineer: motion, collision, forces and stability. Technical Artist: art direction, assets, materials, lighting, animation and performance budgets. QA: test design, regression, quality evidence and truthful reporting.

## Quality priorities
P0 data safety/correctness; P1 stability/usability; P2 performance; P3 polish/noncritical features. For a mid-to-upper-tier result target a coherent 4/5 internal review in functional completeness, interaction/game feel, visual direction, stability/performance, responsive/accessibility and maintainability/testability. Scores require evidence; never fabricate them. No AAA or commercial-hit guarantee.

## Build quality
Web: clear information architecture, design tokens, hierarchy, responsive layout, functional forms/navigation, semantic markup, keyboard/focus/contrast, and loading/empty/error states where relevant. Games: implement the core loop, start/pause/restart/completion, controls, collision/objectives/progression and responsive feedback where applicable. 3D requires coherent scene scale, camera, lighting, materials, collision, resource lifecycle and performance-aware detail.

## Project protection
Inspect existing files, entry points, dependencies, tests, current Git state, assets, data and behavior. Snapshot before risky edits. Preserve unrelated features. Never delete or overwrite user work merely to simplify the implementation.

## Security and approvals
Never request pasted passwords/tokens. Use secure user-controlled configuration. Confirm destructive changes, migration, breaking interfaces, remote pushes, deployment, public release, external upload, permission changes and paid operations.

## Measurement and tests
Measure FPS, memory, draw calls, geometry/texture sizes, startup and asset size when tools allow; mark NOT MEASURED otherwise. Separate static, unit/integration, browser end-to-end and real-device tests. Report test commands and counts. A viewport simulation is not a physical-device test. Maximum three same-root-cause repair attempts.
