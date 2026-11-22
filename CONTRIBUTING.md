# Contributing / 参与贡献

Thank you for your interest in improving Web & Game Engineer. Contributions should make the framework more reliable, understandable, portable and verifiable.

感谢你参与改进 Web & Game Engineer。我们希望每项贡献都能提升框架的可靠性、可理解性、可移植性与可验证性。

## Before you start / 开始之前
1. Read the root [README](README.md), [Shared Core](SKILL.md) and relevant module or adapter documentation. / 阅读根目录 README、统一核心指令及相关模块/适配器文档。
2. Check the [Acceptance Matrix](release/acceptance-matrix.csv) to understand current verification gaps. / 查看验收矩阵，了解当前验证缺口。
3. Open an issue or discussion for major architecture changes, new platform targets or breaking changes. / 对重大架构调整、新平台目标或破坏性变更，先发起 Issue 或讨论。
4. Do not include secrets, private keys, tokens, personal data or proprietary assets without permission. / 不得未经许可提交密钥、令牌、个人数据或专有资产。

## Contribution areas / 可贡献方向
- Core workflow and documentation / 核心工作流与文档
- Engineering modules and reusable templates / 工程模块与可复用模板
- Platform adapters and installation guidance / 平台适配器与安装指南
- Automated tests, benchmark tasks and regression coverage / 自动化测试、基准任务与回归覆盖
- Packaging, checksums and release automation / 打包、校验与发布自动化
- Translations, examples and accessibility / 翻译、示例与无障碍体验

## Engineering standards / 工程标准
- Inspect existing behavior before proposing changes. / 提出修改前先检查现有行为。
- Prefer small, scoped and reversible changes. / 优先小范围、可回滚的修改。
- Preserve compatibility unless a breaking change is explicitly approved. / 除非明确批准破坏性变更，否则保持兼容。
- Add or update tests for behavior changes. / 行为变更必须增加或更新测试。
- Never weaken tests simply to obtain a passing result. / 不得为了获得通过结果而削弱测试。
- Document dependencies, limitations and migration steps. / 记录依赖、限制与迁移步骤。
- Report only tests actually executed. / 只报告真实执行过的测试。

## Platform adapter requirements / 平台适配器要求
Each adapter must document the exact host product and entry point, supported installation/import route, required tools and permissions, fallback behavior, known limitations, adapter version and independent acceptance status.

每个适配器必须说明准确的宿主产品与入口、支持的安装/导入方式、所需工具与权限、降级行为、已知限制、适配器版本及独立验收状态。

Do not claim native Skill or plugin support unless the target host actually supports and verifies that route. Never transfer certification from one platform to another.

除非目标宿主真实支持并完成验证，否则不得宣称支持原生 Skill 或插件导入。不得将一个平台的认证转移给另一个平台。

## Pull request checklist / PR 检查清单
- [ ] Scope and motivation are clear. / 修改范围与原因清晰。
- [ ] Existing behavior and project boundaries were inspected. / 已检查既有行为与项目边界。
- [ ] Relevant tests were added or updated. / 已增加或更新相关测试。
- [ ] Applicable tests were executed and results reported. / 已执行适用测试并报告结果。
- [ ] Documentation and version metadata are consistent. / 文档与版本元数据一致。
- [ ] No secrets or unauthorized assets are included. / 不包含密钥或未经授权的资产。
- [ ] Package manifests, ZIPs and checksums are valid when distribution changes. / 涉及分发时，Manifest、ZIP 与校验文件有效。
- [ ] Certification claims match actual evidence. / 认证声明与真实证据一致。

## Versioning and releases / 版本与发布
Core, modules, adapters and installable packages may have independent versions. Follow [Release Policy](release/POLICY.md) and [Distribution Contract](release/DISTRIBUTION.md). Public releases and deployment require maintainer approval.

Core、模块、适配器和可安装包可独立版本管理。请遵循发布政策与分发规范。公开发布与部署需要维护者批准。

## Questions / 联系与讨论
Use GitHub Issues for reproducible defects and feature proposals. Include the affected package, version, host product, expected behavior, actual behavior and sanitized logs where possible.

可通过 GitHub Issues 提交可复现缺陷与功能建议。尽可能注明受影响的安装包、版本、宿主产品、预期行为、实际行为及脱敏日志。
