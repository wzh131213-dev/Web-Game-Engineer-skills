# Web & Game Engineer — Claude

**Version:** 0.2.0-alpha  
**Status:** Experimental / NOT CERTIFIED.

This source contains two separate Claude distribution targets:

1. **Claude Code plugin** — `.claude-plugin/plugin.json` plus `skills/web-game-engineer/SKILL.md`.
2. **Claude.ai Agent Skill** — a ZIP containing `web-game-engineer/SKILL.md` for the Skills upload/import workflow, when available in the account.

These are separate host formats and must be installed and certified independently. Neither package grants terminal, filesystem, MCP, network, or Git permissions. Claude only uses capabilities available in the active environment.

The central GitHub Actions workflow generates both ZIPs, validates their required paths, creates SHA-256 sidecars, and adds both download links to `dist/packages/INDEX.md`.

## Compatibility status

CI validates the archive structure only. Actual Claude.ai upload, Claude Code plugin loading, and runtime behavior remain NOT RUN until tested in the respective host.


All shipped Skill entry points include the One-Sentence Build Mode. Host installation and runtime compatibility remain NOT RUN until independently tested.
