# Contributing / 参与贡献

Contributions should improve reliability, completeness, usability, portability and verifiability. / 贡献应提升可靠性、完整性、可用性、可移植性和可验证性。

## Before contributing / 贡献前
1. Read [README](README.md), [Shared Core](SKILL.md), [One-Sentence Build Specification](core/ONE_SENTENCE_BUILD.md) and the relevant adapter.
2. Check [benchmarks](benchmarks/ACCEPTANCE.md) and [acceptance matrix](release/acceptance-matrix.csv).
3. Discuss major architecture changes, new host targets and breaking changes before implementation.
4. Never submit secrets, private data, unlicensed assets or proprietary source.

## Engineering standards / 工程规范
- Inspect existing files, interfaces and behavior before modifying.
- Prefer scoped, reversible changes and protect existing functionality.
- Turn one-sentence behavior changes into measurable acceptance criteria.
- Build complete primary flows; avoid inert UI, fake service responses and TODO-only paths.
- Test normal, boundary, failure and regression paths where applicable.
- Distinguish static inspection, automated tests, browser/runtime tests and real-device validation.
- Never weaken tests to obtain a passing result.
- Report exact commands, results, limitations and unmeasured metrics.
- Keep Core instructions and all platform entry points aligned.

## Quality target / 质量目标
Aim for polished mid-to-upper-tier independent web/game product quality, not an AAA guarantee. Use the shared six-dimension 1–5 rubric and retain evidence. Do not claim a score, runtime success or certification without proof.

## Platform adapter requirements / 平台适配器
Document the host product and entry point, installation route, actual tools/permissions, fallback, limitations and separate test/certification status. Claude.ai/Claude Code, Qwen Code/Model Studio, and prompt/API routes are separate targets. Do not transfer certification.

## Pull request checklist / PR 检查清单
- [ ] Scope and acceptance criteria are clear.
- [ ] Existing project behavior is protected.
- [ ] One-sentence entrypoint instructions match the shared Core.
- [ ] Relevant tests were added/updated and actually run.
- [ ] No secrets or unauthorized assets are included.
- [ ] Documentation, manifests, versions and ZIP naming are consistent.
- [ ] Certification claims match recorded evidence.

Public releases, deployments, remote publication, destructive changes and paid actions require maintainer approval.
