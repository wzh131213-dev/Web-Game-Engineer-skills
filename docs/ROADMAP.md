# Product Roadmap / 产品路线图

This roadmap describes the intended evolution of Web & Game Engineer. Items are planning targets, not promises that a feature is already implemented or certified.

本路线图描述 Web & Game Engineer 的计划演进方向。路线图条目属于规划目标，不代表功能已经实现或通过认证。

## Current baseline / 当前基线
**Release:** 0.1.3-alpha · **Channel:** Experimental · **Platform certification:** No platform certified  
**版本：** 0.1.3-alpha · **通道：** Experimental · **平台认证：** 暂无平台通过正式认证

Six platform adapters are packaged in one GitHub Release with per-archive SHA-256 files. / 六个平台适配包集中在一个 GitHub Release 中，每个压缩包附 SHA-256 校验文件。

## Phase 1 — Foundation & consistency / 第一阶段：基础与一致性
- Consolidate shared Core instructions and module boundaries. / 整理统一核心指令与模块边界。
- Keep platform adapters independently versioned and documented. / 保持平台适配器独立版本与文档。
- Improve bilingual documentation and installation clarity. / 完善双语文档与安装说明。
- Maintain reproducible ZIP and checksum generation. / 维护可复现的 ZIP 与校验文件生成流程。
- Keep the acceptance matrix honest and current. / 保持验收矩阵真实、及时。

## Phase 2 — Verification & certification / 第二阶段：验证与认证
- Execute installation checks for each host target. / 分别执行各宿主目标的安装检查。
- Validate host capability detection and tool availability. / 验证宿主能力检测与工具可用性。
- Run shared benchmarks across web, 2D, 3D, physics, legacy-project protection and delivery. / 对 Web、2D、3D、物理、旧项目保护与交付执行统一基准测试。
- Record reproducible evidence and platform-specific limitations. / 记录可复现证据与平台限制。
- Certify each platform independently only after its acceptance requirements pass. / 仅在满足验收要求后独立认证对应平台。

## Phase 3 — Engineering depth / 第三阶段：工程能力深化
- Strengthen reusable project templates and state schemas. / 强化可复用项目模板与状态 Schema。
- Expand 3D workbench workflows and asset pipelines. / 扩展 3D 工作台与资产流水线。
- Improve physics, animation and AI gameplay workflow guidance. / 深化物理、动画与 AI 玩法工作流。
- Improve automated regression and bounded self-repair patterns. / 改进自动回归与有限自修复模式。
- Add performance budgets and profiling guidance. / 增加性能预算与分析指导。

## Phase 4 — Ecosystem & release maturity / 第四阶段：生态与发布成熟度
- Improve cross-platform project handoff. / 改进跨平台项目交接。
- Add adapter conformance checks as host capabilities evolve. / 随宿主能力变化增加适配器一致性检查。
- Improve release notes, migration guidance and compatibility history. / 完善发布说明、迁移指南与兼容历史。
- Establish a stable-release gate based on repeatable evidence. / 基于可复现证据建立稳定版发布门槛。

## Release principles / 发布原则
1. No certification by implication. / 不通过暗示授予认证。
2. No stable label without completed release gates. / 未完成发布门禁不标记 Stable。
3. No destructive migration without explicit approval and rollback planning. / 未经明确批准与回滚规划不执行破坏性迁移。
4. Quality and data integrity outrank feature count. / 质量与数据完整性高于功能数量。
5. Update the roadmap when priorities or evidence change. / 优先级或验证证据变化时同步更新路线图。
