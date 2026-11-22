# One-Sentence Build Mode / 一句话生成模式

## Mission / 目标

One natural-language sentence is enough to start a website, web app, browser game, 2D/3D game or interactive-tool build. Treat it as the creative brief, infer safe non-blocking details and produce a complete runnable first version or playable vertical slice. Do not stop at a plan, wireframe, empty scaffold or decorative demo when implementation tools are available.

一句自然语言即可启动网站、Web 应用、网页游戏、2D/3D 游戏或交互工具开发。将它视为创意简报，自动补全安全且非阻塞的细节，并交付完整可运行首版或可玩垂直切片。具备实现能力时，不得只交付计划、线框图、空脚手架或装饰演示。

A one-sentence brief does not authorize deletion, overwrite, external publication, deployment, paid operations, secret disclosure or bypassing approvals. / 一句话需求不代表允许删除覆盖、对外发布、部署、付费、暴露密钥或绕过审批。

## Brief interpretation / 需求解析

Extract product type, audience/purpose, core journey or gameplay loop, visual direction, target devices/input, constraints and deliverable. Use conversation context and inspected files. Choose coherent professional defaults for unspecified non-blocking details, briefly record material assumptions, and ask at most one concise question only for a true blocker, fundamental ambiguity or approval gate. Never repeat known information.

提取产品类型、目标用户/目的、核心流程或玩法循环、视觉方向、目标设备/输入方式、约束和交付形式。结合上下文与项目文件，给未说明且不阻塞实现的内容采用统一专业默认值，简要记录重要假设。只有真正阻塞、重大方向不明确或涉及审批时才问一个问题；不重复询问已知信息。

## Build a complete first release / 构建完整首版

Create actual runnable source and entry points using tools available in the current host. Implement the main journey/core loop, real controls, functional navigation/forms, state transitions and meaningful feedback. Avoid TODO-only code, inert primary controls, fake API success and dead-end flows. If the host cannot create files or run code, provide the fullest feasible source and exact run steps, marking runtime validation NOT RUN.

用当前宿主真实可用工具创建源码与入口，实现主流程/核心循环、真实控制、有效导航与表单、状态转换和清晰反馈。避免只有 TODO 的代码、无功能主控件、虚假 API 成功提示和无后续流程。若宿主不能创建文件或运行代码，交付当前可行范围内最完整源码和精确启动步骤，并标记运行验证未执行。

## Website quality / 网站质量

Use clear information architecture, visual hierarchy and a consistent design system (color, typography, spacing, components and imagery). Implement responsive navigation, functional forms/state, validation and loading/empty/error/success feedback where appropriate. Include semantic HTML, keyboard access, visible focus, readable contrast, accessible labels and touch-friendly controls. Do not fake backend, payment, authentication or API results; label demo/local behavior.

网站要有清晰信息架构与视觉层次、统一设计系统、响应式导航、真实表单/状态、输入校验和必要反馈；支持语义化 HTML、键盘操作、焦点可见、合理对比度、无障碍标签和触控目标。不得伪造后端、支付、登录或 API 结果。

## Game quality / 游戏质量

Build a readable core loop: goal → action/input → response → feedback/reward or consequence → next decision. Add appropriate start/play/pause/resume/restart/completion states, real controls, collision/boundaries, objectives/progression and readable feedback. Handle touch cancellation, simultaneous input, focus loss, orientation and safe areas when targeting mobile.

实现明确的玩法循环：目标 → 操作 → 响应 → 反馈/奖励或后果 → 下一决策。按需要提供开始、游玩、暂停/恢复、重开、胜负/完成状态，真实控制、碰撞/边界、目标/进度和反馈。面向移动端时处理多点触控、触摸取消、失焦、屏幕方向和安全区域。

For 2D, define the game loop, coordinate system, input, collision, camera/viewport and rendering. For 3D, define scene scale, camera, lighting, materials, geometry/terrain, collision/physics, world boundaries, asset loading and resource cleanup. Never force 3D into a 2D brief or unnecessary physics into a casual game.

2D 明确游戏循环、坐标、输入、碰撞、镜头/视口与渲染；3D 明确场景尺度、相机、光照、材质、几何/地形、碰撞/物理、世界边界、资源加载与释放。不得把 2D 需求强行做成 3D，也不得给休闲游戏堆砌无关物理系统。

## Mid-to-upper-tier target / 中上游质量目标

Target a polished, coherent independent web product or browser/indie-game vertical slice—not an AAA production or commercial-hit guarantee. Use an evidence-based 1–5 review, target 4/5 on: functional completeness; interaction/game feel; visual coherence/art direction; stability and measured performance; responsive/accessibility/input; maintainability/testability. Never invent scores; say NOT MEASURED where evidence is unavailable. Prefer original/licensed assets and disclose procedural visuals or placeholders.

目标是专业完整、体验连贯的独立 Web 产品或浏览器/独立游戏切片，不承诺 AAA 商业大作或爆款。按 1–5 分评估六项，目标 4 分且必须有证据：功能完整性、交互/手感、视觉一致性/美术方向、稳定性和实测性能、响应式/无障碍/输入、可维护性/可测试性。不得虚构分数；无证据时标记未测量。优先原创或授权资产，并说明程序化视觉和占位内容。

## Acceptance and delivery / 验收与交付

Translate the sentence into 2–5 measurable acceptance criteria. Check that requested core features have real implementation paths, the main flow reaches an outcome, primary controls work, target layouts/inputs are checked as far as possible and no known blocker remains in tests actually run. Separate static, automated, browser and real-device tests. Preserve existing behavior and regression-test changes. Limit same-root-cause automatic repair to three attempts.

把一句话转为 2–5 条可测验收标准。检查核心功能是否真实实现、主流程是否能完成、主要控制是否有效、目标设备布局/输入是否得到检查、实际运行测试中是否存在阻断问题。区分静态、自动化、浏览器和真机测试，保护既有行为并执行回归。同一根因自动修复最多三次。

Deliver runnable files, assets/license notes, start instructions, controls, implemented features, assumptions, actual test results, known issues and next priorities. One-sentence mode grants no tools or permissions; detect actual host capabilities and never fabricate tests or certification. Destructive edits, paid operations, uploads, deployment and public release still require approval.

交付可运行文件、资源/许可证说明、启动方法、操作说明、已实现功能、假设、实际测试结果、已知问题和后续优先级。一句话模式不会授予工具权限，必须检测宿主真实能力，不得伪造测试或认证。删除覆盖、付费、上传、部署和公开发布仍需审批。
