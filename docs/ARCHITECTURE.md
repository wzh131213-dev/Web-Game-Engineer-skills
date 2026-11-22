# Architecture / 系统架构

Web & Game Engineer is a layered cross-platform engineering workflow: one shared Core, nine task-focused modules, seven role perspectives, six independently maintained adapters, portable project state and evidence-based release gates.

Web & Game Engineer 采用分层跨平台工程体系：统一 Core、九大任务模块、七个专业角色视角、六个独立适配器、可移植项目状态和证据驱动的发布门禁。

## Architecture layers / 架构分层

| Layer | Responsibility / 职责 |
|---|---|
| Shared Core | Common rules, one-sentence build mode, quality target, safety gates and delivery contract. / 统一规范、一句话构建模式、质量目标、安全门禁与交付约定。 |
| Specialist Modules | Web, 2D, 3D, workbench, physics, animation, AI logic, QA and deployment. / Web、2D、3D、工作台、物理、动画、AI 逻辑、测试与部署。 |
| Role Reviews | Project/Game Director, Architect, Web, Game, Physics, Technical Artist and QA. / 七个专业职责审查视角。 |
| Platform Adapters | ChatGPT, Claude, Gemini, DeepSeek, Qwen and Doubao entry points and host limits. / 六个平台入口和宿主能力边界。 |
| Project State | Versioned context, architecture, tasks, logs, tests, issues and handoff. / 版本化上下文、架构、任务、日志、测试、问题与交接。 |
| Quality & Release | Benchmarks, acceptance matrix, ZIP validation, SHA-256 and release automation. / 基准测试、验收矩阵、ZIP 校验、SHA-256 与发布自动化。 |

## One-sentence build pipeline / 一句话构建流水线

`One sentence → intent extraction → safe defaults → module selection → architecture → complete vertical slice → tests → bounded repair → quality review → runnable delivery`

A one-sentence brief is enough to begin. The workflow infers non-blocking details rather than requiring a long requirements form. It builds a complete first version when tools permit, not a plan-only response. Every platform adapter embeds this workflow in its shipped entry point.

一句话即可启动开发。工作流会自动补全非阻塞细节，而非要求用户填写长规格。宿主工具允许时直接构建完整首版，而不是只返回计划。各平台适配器均在实际打包的入口文件中内置这一流程。

## Mid-to-upper-tier quality definition / 中上游质量定义

The target is a polished independent web product or browser/indie-game vertical slice, not an AAA guarantee. Review functional completeness, game feel/interactions, visual direction, stability/measured performance, responsive/accessibility/input and maintainability/testability. Target 4/5 on an evidence-based rubric; unknown metrics remain NOT MEASURED.

目标是专业完整的独立 Web 产品或浏览器/独立游戏垂直切片，不承诺 AAA。评估功能完整性、手感/交互、视觉方向、稳定性/实测性能、响应式/无障碍/输入及可维护性/可测试性。以有证据的 4/5 为目标，未知指标标为未测量。

## Platform boundaries / 平台边界

Each adapter separately documents supported product surfaces, installation, tool capabilities, permissions, fallback paths, known limitations and certification. A Skill/prompt does not grant terminal, browser, API, file or device access. Claude.ai and Claude Code are separate targets; DeepSeek/Doubao prompt and API paths are not interchangeable; Qwen Code and Model Studio targets are separate.

每个适配器独立说明宿主产品、安装方式、工具能力、权限、降级方案、限制和认证。Skill/提示词不会授予终端、浏览器、API、文件或真机权限。Claude.ai 与 Claude Code 是不同目标；DeepSeek/豆包提示词与 API 路线不可混为一谈；Qwen Code 和 Model Studio 也是不同目标。

## Technology baseline / 技术基线

- Web: HTML5/CSS/JS/TS.
- 2D: Canvas/WebGL or suitable framework.
- 3D: Three.js baseline; WebGPU optional.
- Physics: modular interfaces; Rapier may supply primitives.
- Assets: editable procedural assets and licensed GLTF/GLB.
- Avoid unnecessary dependencies, paid services and proprietary asset copying.

## Project state and release integrity / 项目状态与发布完整性

Project files are the cross-platform source of truth. Every package has a manifest, its own ZIP and SHA-256 sidecar. A valid archive proves packaging only—not native import, runtime performance or certification.

项目文件是跨平台事实来源。每个安装包均有 Manifest、独立 ZIP 和 SHA-256 文件。压缩包校验通过只证明打包完整，不证明原生导入、运行性能或平台认证。
