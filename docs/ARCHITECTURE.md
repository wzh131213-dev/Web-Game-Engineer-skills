# Architecture / 系统架构

Web & Game Engineer is designed as a layered engineering system: shared standards at the center, capability modules around the Core, and independent adapters at the platform boundary.

Web & Game Engineer 采用分层工程架构：核心层统一标准，能力层提供专业模块，平台边界层负责独立适配。

## 1. Architecture principles / 架构原则
- **One Core, multiple adapters:** common workflows are defined once; host-specific behavior stays in adapters. / 一个核心、多个适配器：通用流程统一定义，宿主差异留在适配层。
- **Modular by relevance:** load only the modules required by the task. / 按需加载：只加载任务所需模块。
- **Explicit boundaries:** do not assume identical tools, permissions, memory or execution environments across AI products. / 边界明确：不假设不同 AI 产品拥有相同工具、权限、记忆或执行环境。
- **Project files are authoritative:** portable project state is the cross-platform source of truth. / 项目文件为准：可移植项目状态是跨平台事实来源。
- **Evidence-driven delivery:** test claims must match the checks actually executed. / 证据驱动交付：测试结论必须对应真实执行过的检查。

## 2. Logical layers / 逻辑分层

| Layer | Responsibility / 职责 |
|---|---|
| Shared Core | Engineering principles, workflow, safety gates, quality standards and delivery contract. / 工程原则、工作流、安全门禁、质量标准与交付约定。 |
| Professional Modules | Nine task-focused capability areas. / 九个面向任务的专业能力模块。 |
| Platform Adapters | Installation guidance, host capability detection, prompt/Skill/plugin packaging and host-specific limitations. / 安装说明、宿主能力检测、提示词/Skill/插件打包及平台限制。 |
| Project State | Versioned project metadata, architecture, tasks, logs, test reports and handoff files. / 版本化项目元数据、架构、任务、日志、测试报告与交接文件。 |
| Quality & Release | Acceptance matrix, archive validation, checksums, release automation and certification records. / 验收矩阵、压缩包校验、哈希、发布自动化与认证记录。 |

## 3. Engineering lifecycle / 工程生命周期
`Requirements → Inspect → Architect → Plan → Implement → Test → Repair → Optimize → Deliver`

1. **Requirements:** define outcomes, constraints and acceptance criteria. / 明确目标、约束与验收标准。
2. **Inspection:** inspect existing files, dependencies, assets, entry points and tests. / 检查现有文件、依赖、资源、入口和测试。
3. **Architecture:** define module boundaries, data flow, interfaces and rollback strategy. / 定义模块边界、数据流、接口与回滚策略。
4. **Planning:** split work into small, verifiable tasks. / 拆分为小型、可验证任务。
5. **Implementation:** make scoped changes and preserve existing behavior. / 局部实现并保护既有行为。
6. **Testing:** run applicable static, automated and runtime checks. / 执行适用的静态、自动化和运行时检查。
7. **Repair:** fix root causes with bounded retries. / 限次修复根因。
8. **Optimization:** measure before tuning performance or visual fidelity. / 先测量，再优化性能与视觉效果。
9. **Delivery:** package source, instructions, test evidence, known issues and version details. / 交付源码、说明、测试证据、已知问题与版本信息。

## 4. Platform adapter boundary / 平台适配边界
Each platform adapter owns its supported host products and entry points, installation/import instructions, capability and permission assumptions, fallback routes, limitations, tests, version and certification status.

每个适配器分别负责宿主产品与入口、安装/导入说明、能力与权限假设、降级路线、限制、测试、版本和认证状态。

Claude.ai Skills and Claude Code plugins are distinct targets. DeepSeek chat prompts and API instructions are distinct routes. Qwen Code and Model Studio Agent Skills are distinct targets. Doubao chat prompts and Volcengine Ark API instructions are distinct routes.

Claude.ai Skills 与 Claude Code 插件是不同目标；DeepSeek 对话提示词与 API 指令是不同路线；Qwen Code 与 Model Studio Agent Skills 分别适配；豆包对话提示词与火山引擎 Ark API 指令也分别处理。

No platform inherits another platform's certification. A package archive is not proof of host compatibility.

平台之间不得继承认证结果。压缩包可用不等于宿主兼容。

## 5. Technology policy / 技术选型策略
- Web: HTML5, CSS, JavaScript/TypeScript. / Web：HTML5、CSS、JavaScript/TypeScript。
- 2D: Canvas, WebGL or a suitable framework. / 2D：Canvas、WebGL 或合适框架。
- 3D: Three.js as a practical baseline; WebGPU is optional. / 3D：以 Three.js 为实用基线，WebGPU 为可选项。
- Physics: Rapier can provide primitives behind project-specific interfaces. / 物理：可通过项目专属接口封装 Rapier 等基础能力。
- Assets: prefer portable GLTF/GLB and explicit resource lifecycle management. / 资产：优先使用可移植 GLTF/GLB，并明确资源生命周期。
- Dependencies: avoid adding heavy dependencies without a measurable need. / 依赖：没有可衡量的必要性时避免引入重型依赖。

## 6. Project state and handoff / 项目状态与交接
Portable project files should record project identity, schema version, goals, approved decisions, architecture, task status, development log, test report, known issues and handoff notes.

可移植项目文件应记录项目身份、Schema 版本、目标、已批准决策、架构、任务状态、开发日志、测试报告、已知问题与交接说明。

See [Project State Schema](../schemas/PROJECT_STATE.md).

## 7. Release integrity / 发布完整性
Each installable package has a manifest, a matching ZIP and a SHA-256 sidecar. GitHub Actions validates archive structure before publishing. The acceptance matrix remains the authority for host testing and certification.

每个可安装包均有 Manifest、对应 ZIP 与 SHA-256 校验文件。GitHub Actions 在发布前验证压缩包结构。宿主测试与认证状态以验收矩阵为准。

See [Distribution Contract](../release/DISTRIBUTION.md) and [Acceptance Matrix](../release/acceptance-matrix.csv).
