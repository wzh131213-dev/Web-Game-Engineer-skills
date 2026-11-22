# Features & Modules / 功能与模块

This document describes the product's intended engineering scope. A listed capability is a workflow area, not a claim that every host adapter has completed runtime certification.

本文介绍产品的工程能力范围。列出的能力代表工作流覆盖方向，不代表每个平台适配器都已完成运行时认证。

## Nine professional modules / 九大专业模块

### 01 — Web Development / Web 开发
Responsive web interfaces, HTML/CSS/JS/TS, routing, forms, application state, browser storage, accessibility and integration.

响应式网页、HTML/CSS/JS/TS、路由、表单、应用状态、浏览器存储、无障碍与系统集成。

### 02 — 2D Game Development / 2D 游戏开发
Game loops, input systems, Canvas/WebGL rendering, animation, collision, maps, level flow, save systems and gameplay state.

游戏循环、输入系统、Canvas/WebGL 渲染、动画、碰撞、地图、关卡流程、存档与玩法状态。

### 03 — 3D Game Development / 3D 游戏开发
Three.js scene architecture, cameras, lighting, materials, models, terrain, world chunks, interaction and resource lifecycle.

Three.js 场景架构、相机、光照、材质、模型、地形、世界分块、交互与资源生命周期。

### 04 — 3D Workbench / 3D 工作台
Scene/object selection, transform controls, property inspection, terrain editing, asset management, skeleton workflows and export.

场景/物体选择、变换控制、属性检查、地形编辑、资产管理、骨骼工作流与导出。

### 05 — Physics Engine / 物理引擎
Physics core, vehicle and character dynamics, contact and collision, environmental forces, stability and destruction-oriented simulation.

物理核心、载具与角色动力学、接触与碰撞、环境力、稳定性及破坏模拟。

### 06 — Animation System / 动画系统
Skeletons, keyframes, animation state machines, blending, inverse kinematics and event-driven animation.

骨骼、关键帧、动画状态机、混合、逆向运动学与事件驱动动画。

### 07 — AI Game Logic / AI 游戏逻辑
NPC state machines, behavior trees, pathfinding, perception, dialogue, quests and gameplay decision logic.

NPC 状态机、行为树、寻路、感知、对话、任务与玩法决策逻辑。

### 08 — Testing & Repair / 测试与修复
Unit, integration, interaction, visual, performance and regression tests; root-cause analysis and bounded repair attempts.

单元、集成、交互、视觉、性能与回归测试；根因分析与有限次修复。

### 09 — Deployment & Git / 部署与 Git
Build pipelines, packaging, version control, GitHub automation, release preparation, deployment and handoff.

构建流水线、打包、版本控制、GitHub 自动化、发布准备、部署与交接。

## Seven virtual roles / 七大虚拟角色

| Role / 角色 | Primary focus / 主要职责 |
|---|---|
| Project Manager / Game Director 项目经理 / 游戏总监 | Scope, priorities, milestones and acceptance criteria. / 范围、优先级、里程碑与验收标准。 |
| System Architect 系统架构师 | Architecture, interfaces, data flow and technical risk. / 架构、接口、数据流与技术风险。 |
| Web Engineer Web 工程师 | Browser UI, responsive behavior and web integration. / 浏览器界面、响应式行为与 Web 集成。 |
| Game Engineer 游戏工程师 | Gameplay, controls, scenes and state transitions. / 玩法、控制、场景与状态转换。 |
| Physics Engineer 物理工程师 | Forces, motion, collision and simulation stability. / 力、运动、碰撞与仿真稳定性。 |
| Technical Artist 技术美术 | Assets, materials, lighting, animation and visual budgets. / 资产、材质、光照、动画与视觉预算。 |
| QA Engineer 测试工程师 | Test coverage, regression, triage and release evidence. / 测试覆盖、回归、问题分级与发布证据。 |

Roles are sequential perspectives when the host does not expose independent agents. The product does not claim that seven autonomous agents are always active.

如果宿主没有独立 Agent 能力，角色将作为流程中的顺序审查视角，不宣称七个自治 Agent 始终并行运行。

## Quality model / 质量模型
- Correctness and data integrity first. / 正确性与数据完整性优先。
- Stability and usability before visual polish. / 稳定性与可用性优先于视觉打磨。
- Performance optimization based on measurements. / 基于测量数据进行性能优化。
- Explicit PASS, FAIL, PARTIAL, NOT RUN and MANUAL states. / 明确区分通过、失败、部分通过、未运行与人工验证。
- Regression checks after behavior-changing edits. / 行为变更后执行回归检查。

## Module loading / 模块加载
Modules are enabled by default but loaded only when relevant. Keep dependencies proportional to the project: simple websites do not require a 3D stack, and 2D projects should not inherit unrelated 3D physics.

模块默认启用，但仅在任务相关时加载。依赖应与项目规模相称：简单网站不需要 3D 技术栈，2D 项目也不应继承无关的 3D 物理系统。
