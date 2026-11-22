# Web & Game Engineer

<p align="center"><strong>ONE SENTENCE. A COMPLETE BUILD. PROFESSIONAL WEB & GAME ENGINEERING.</strong></p>
<p align="center">
<a href="https://github.com/wzh131213-dev/Web-Game-Engineer-skills/releases/tag/v0.2.0-alpha-platform-bundle-20261123"><img alt="Release" src="https://img.shields.io/badge/release-0.2.0--alpha-2563eb?style=for-the-badge"></a>
<img alt="Platforms" src="https://img.shields.io/badge/AI%20platforms-6-0891b2?style=for-the-badge">
<img alt="Modules" src="https://img.shields.io/badge/engineering%20modules-9-7c3aed?style=for-the-badge">
<img alt="Certification" src="https://img.shields.io/badge/status-experimental%20%2F%20not%20certified-d97706?style=for-the-badge">
</p>

**Web & Game Engineer** is a cross-platform AI engineering Skill for turning concise creative briefs into complete websites, web applications, browser games, 2D/3D games and interactive workbenches. One shared Core, nine specialist modules, seven professional review roles and six independent platform adapters provide a structured route from idea to implementation, testing and delivery.

**Web & Game Engineer** 是一套跨 AI 平台的专业工程 Skill，将简短创意需求转化为完整网站、Web 应用、网页游戏、2D/3D 游戏和交互式工作台。统一 Core、九大专业模块、七个专业审查角色和六个平台适配器，形成从想法到实现、测试和交付的完整流程。

> **One sentence. A complete first build. Verifiable quality.**  
> **一句话启动，完整首版交付，质量有据可查。**

## One sentence. A complete first build. / 一句话，直接生成完整作品

Describe the website or game you want in one natural-language sentence. The Skill treats it as a creative brief, fills safe non-blocking details with professional defaults, chooses the relevant modules, builds a runnable first version/playable vertical slice and tests the flows that the active AI host can actually execute.

只需一句自然语言描述你想要的网站或游戏。Skill 会自动补全非关键细节、选择相关模块、构建可运行首版/可玩垂直切片，并测试当前 AI 平台真实能够执行的流程。

**Example / 示例：** “制作一款移动端 3D 海岛探索游戏，玩家可以自由奔跑、收集遗迹、与守卫战斗，并拥有精致的环境光照和完整任务循环。”

**Quality target / 质量目标：** a polished mid-to-upper-tier independent web product or browser/indie-game vertical slice—not an AAA guarantee. Six dimensions are reviewed with evidence: functional completeness, interaction/game feel, visual coherence, stability/performance, responsive/accessibility/input, and maintainability/testability.

目标是专业、完整、体验连贯的中上游独立 Web 产品或浏览器/独立游戏切片，不虚称 AAA。以六项维度和实际证据检查功能完整性、交互手感、视觉一致性、稳定性/性能、响应式/无障碍/输入及可维护性。

Read the [One-Sentence Build Specification](core/ONE_SENTENCE_BUILD.md) and [benchmark suite](benchmarks/ACCEPTANCE.md).

## Download / 下载

**[Open the unified six-platform GitHub Release / 六个平台统一下载入口](https://github.com/wzh131213-dev/Web-Game-Engineer-skills/releases/tag/v0.2.0-alpha-platform-bundle-20261123)**

The Release contains six ZIP packages and a SHA-256 checksum sidecar for every archive.  
统一 Release 提供六个平台 ZIP，每个压缩包均附 SHA-256 校验文件。

| Platform | Package ZIP |
|---|---|
| ChatGPT | `web-game-engineer-chatgpt-0.2.0-alpha.zip` |
| Claude | `web-game-engineer-claude-0.2.0-alpha.zip` |
| Gemini | `web-game-engineer-gemini-0.2.0-alpha.zip` |
| DeepSeek | `web-game-engineer-deepseek-0.2.0-alpha.zip` |
| Qwen | `web-game-engineer-qwen-0.2.0-alpha.zip` |
| Doubao | `web-game-engineer-doubao-0.2.0-alpha.zip` |

[All ZIPs and checksums / 全部安装包与校验文件](dist/packages/INDEX.md) · [GitHub Releases](https://github.com/wzh131213-dev/Web-Game-Engineer-skills/releases)

## Nine engineering modules / 九大专业模块

1. **Web Development:** responsive interfaces, information architecture, forms, routing, state, accessibility and performance.
2. **2D Game Development:** game loops, controls, animation, collision, maps, levels, progression and saves.
3. **3D Game Development:** Three.js scenes, terrain, models, lighting, materials, camera, collision and resource lifecycle.
4. **3D Workbench:** scene/object editing, transforms, inspectors, terrain tools, assets and export.
5. **Physics Engine:** physics core, vehicle/character/environment physics, contacts, stability and destruction simulation.
6. **Animation System:** skeletons, keyframes, state machines, blending, IK and events.
7. **AI Game Logic:** NPC state machines, behavior trees, pathfinding, perception, dialogue and quests.
8. **Testing & Repair:** unit, integration, interaction, visual, performance and regression tests with bounded repair.
9. **Deployment & Git:** builds, packaging, version control, GitHub automation, deployment and handoff.

Modules are loaded only when relevant. A simple site does not need a 3D engine; a 2D game should not inherit an unnecessary 3D physics stack.

模块按需加载。简单网站不需要 3D 引擎，2D 游戏不应承担无关的 3D 物理依赖。

## Seven professional review roles / 七大专业角色

Project Manager/Game Director · System Architect · Web Engineer · Game Engineer · Physics Engineer · Technical Artist · QA Engineer.

项目经理/游戏总监 · 系统架构师 · Web 工程师 · 游戏工程师 · 物理工程师 · 技术美术 · 测试工程师。

These are structured role perspectives, not a claim that seven independent AI agents always run. If the host lacks multi-agent execution, the roles review work sequentially.

这些是专业职责视角，不代表七个独立 AI Agent 始终并行运行。宿主不支持多智能体时，按流程顺序审查。

## Engineering workflow / 工程工作流

`One-sentence brief → acceptance criteria → inspect → infer safe defaults → select modules → build → test → bounded repair → measure/polish → deliver`

`一句话需求 → 验收标准 → 项目检查 → 安全默认补全 → 模块选择 → 构建 → 测试 → 有限修复 → 测量与打磨 → 交付`

- Build a complete first version, not only a plan or mockup. / 交付完整首版，而不只是计划或样机。
- Preserve existing projects and regression-test changes. / 保护既有项目并执行回归测试。
- Use only the tools and permissions that the active host actually provides. / 只使用当前宿主真实提供的工具与权限。
- Never fake API results, tests, assets, performance measurements or certification. / 不伪造 API、测试、资产、性能数据或认证。
- Ask approval for destructive changes, paid operations, external uploads, remote pushes, deployments and public releases. / 删除覆盖、付费操作、外部上传、远程推送、部署及公开发布必须审批。

## Platform status / 平台状态

ChatGPT, Claude, Gemini, DeepSeek, Qwen and Doubao each have independent adapters and independent acceptance records. Every platform remains Experimental / NOT CERTIFIED until host installation, tools and benchmark workflows have been tested with evidence.

六个平台均有独立适配器和验收记录。宿主安装、工具能力与基准工作流尚未取得实际证据前，全部保持 Experimental / NOT CERTIFIED。

## Documentation / 文档

- [One-Sentence Build Specification](core/ONE_SENTENCE_BUILD.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Features & Modules](docs/FEATURES.md)
- [Roadmap](docs/ROADMAP.md)
- [Cross-platform Benchmarks](benchmarks/ACCEPTANCE.md)
- [Contributing](CONTRIBUTING.md)
- [Changelog](CHANGELOG.md)
- [Release Policy](release/POLICY.md)
- [Distribution Contract](release/DISTRIBUTION.md)

## Current release / 当前版本

**0.2.0-alpha · Experimental · No platform certified.**

This is an evolving alpha. The one-sentence workflow is now specified across all six adapter entry points, but generated build quality, runtime tool availability and host compatibility must still be verified independently.

**0.2.0-alpha · 实验阶段 · 暂无平台通过正式认证。**

本版本已将一句话构建流程写入六个平台的实际指令入口，但生成效果、运行工具可用性和宿主兼容性仍需分别实测。
