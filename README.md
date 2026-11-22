# Web & Game Engineer

**Release:** 0.1.3-alpha · **Channel:** Alpha · **Certification:** no platform certified

A cross-AI engineering Skill with one shared Core, nine professional modules, seven virtual roles and independently versioned platform adapters. Platforms are used separately; no AI-to-AI communication is required.

## Download packages
Every installable platform adapter has its own matching ZIP and SHA-256 checksum. Native host formats receive additional target-specific archives where the host documents a distinct structure. The full source bundle is also packaged. See [package download index](dist/packages/INDEX.md) and [distribution contract](release/DISTRIBUTION.md). ZIPs are generated and committed by GitHub Actions after package changes. Published npm packages are also distributed through the GitHub Packages npm registry; install with `npm install @wzh131213-dev/web-game-engineer-chatgpt --registry=https://npm.pkg.github.com` (replace the adapter name as needed). GitHub Packages visibility is set to Public by the publishing workflow where the connected GitHub permissions allow it.

## Platform adapters
- **ChatGPT:** [portable package](packages/chatgpt/) · [plugin source](plugin-distribution/chatgpt/) · Experimental / NOT CERTIFIED.
- **Claude:** [portable package](packages/claude/) · [Claude.ai Skill and Claude Code plugin sources](plugin-distribution/claude/) · Experimental / NOT CERTIFIED. Claude.ai Skills and Claude Code plugins are separate targets.
- **Gemini:** [Gemini Apps Skill adapter](packages/gemini/) · native Skill ZIP with root-level `SKILL.md` · Experimental / NOT CERTIFIED.
- **DeepSeek:** [portable system-prompt/API adapter](packages/deepseek/) · no consumer-app Skill import is claimed · Experimental / NOT CERTIFIED.
- **Qwen:** [Qwen adapter](packages/qwen/) · separate Qwen Code Agent Skill and Alibaba Cloud Model Studio Agent Skill archives · Experimental / NOT CERTIFIED.
- **Doubao:** [portable prompt/Volcengine Ark adapter](packages/doubao/) · consumer chat prompt and Ark API system-message routes are separate · Experimental / NOT CERTIFIED.

## Start
1. Read root `SKILL.md` for the shared Core.
2. Read the relevant platform adapter's `INSTALL.md` and `PLATFORM_CAPABILITIES.md`.
3. Download the matching adapter ZIP or host-specific archive from `dist/packages/INDEX.md`.
4. Follow only an installation path actually supported by the target account/host.
5. Run the host-specific acceptance tests and record evidence.

All target certifications are independent. A ZIP structure check does not certify host installation, tool permissions or runtime capability. See `release/POLICY.md` and `release/acceptance-matrix.csv`.
