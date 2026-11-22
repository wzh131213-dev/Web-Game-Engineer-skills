# Web & Game Engineer — Claude Plugin

**Version:** 0.1.0-alpha  
**Status:** Experimental / NOT CERTIFIED  
**Target:** Claude Code plugin format. Claude.ai Skills upload is a separate host workflow and is not implied by this plugin package.

This directory is the canonical source for the Claude Code plugin ZIP. The archive root contains:

- `.claude-plugin/plugin.json`
- `skills/web-game-engineer/SKILL.md`

The skill provides a modular engineering workflow for web apps, 2D/3D games, physics, animation, AI game logic, testing, repair, and delivery. It does not grant terminal, file, MCP, network, or Git permissions; Claude only uses capabilities available in the active environment.

## Local validation

From the repository root, validate the manifest JSON and required skill file. Then build the ZIP using the repository GitHub Actions workflow or the documented local packaging steps.

## Compatibility status

The archive layout is structurally validated by CI. Installation and runtime behavior must still be verified in the target Claude Code environment. Claude.ai Skills import, Claude Code plugin installation, and MCP integration are separate compatibility targets.
