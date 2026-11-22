# Claude installation guide

## Target: Claude Code

This package uses the Claude Code plugin layout. It is not a generic executable and does not install MCP servers or grant additional permissions.

### Local plugin directory

1. Download and extract the Claude plugin ZIP.
2. Keep the extracted directory intact so `.claude-plugin/plugin.json` and `skills/web-game-engineer/SKILL.md` remain in their expected locations.
3. From a terminal where Claude Code is installed, launch Claude Code with the extracted plugin directory using the supported local plugin development option: `claude --plugin-dir /path/to/extracted/plugin`.
4. In Claude Code, confirm the plugin/skill is listed by the host and invoke the `web-game-engineer` skill for a small read-only task.
5. Verify that it inspects the project before edits and reports unavailable tools honestly.

The path above is a placeholder; replace it with the actual extracted directory. Do not paste credentials into the conversation.

### Claude.ai

This ZIP is a Claude Code plugin package, not a claim that Claude.ai can install Claude Code plugins. If the Claude.ai account exposes a Skills upload/import feature, use a separately prepared Skills-compatible archive and follow the exact format requested by that interface. Do not label Claude.ai installation successful based on Claude Code packaging.

## Manual fallback

If plugin installation is unavailable, open `skills/web-game-engineer/SKILL.md` and add its instructions to a supported Project/custom instruction workflow, if available. This is manual instruction use, not plugin installation.

## Known limitations

- Status: Experimental / NOT CERTIFIED.
- CI checks archive structure only; target-host installation and runtime are not yet verified.
- Claude.ai Skills and Claude Code plugins are separate distribution targets.
- MCP servers, terminal access, file access, and subagents depend on host configuration.
