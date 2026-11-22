# Claude installation guide

This adapter provides two separate archives. Choose the one matching the Claude product you use.

## A. Claude.ai — Agent Skills ZIP

1. Download `web-game-engineer-claude-skill-0.2.0-alpha.zip`.
2. In Claude.ai, open the Skills management/upload area if it is available for your account.
3. Upload the ZIP as a custom Skill and enable it for a test conversation.
4. Ask Claude to identify the Skill name and summarize its project-protection and testing rules.
5. Test a small read-only task before giving it access to a real project.

The archive contains `web-game-engineer/SKILL.md`. Menu labels and feature availability can vary by account and workspace. If the Skills upload option is unavailable, use the manual fallback below. Do not claim installation succeeded until the host confirms it.

## B. Claude Code — Plugin ZIP

1. Download `web-game-engineer-claude-plugin-0.2.0-alpha.zip`.
2. Extract it while preserving the `.claude-plugin/plugin.json` and `skills/web-game-engineer/SKILL.md` paths.
3. From a terminal where Claude Code is installed, run `claude --plugin-dir /path/to/extracted/plugin`.
4. Confirm the plugin loads and invoke its namespaced skill. The plugin name is `web-game-engineer`; Claude Code may expose the skill as `/web-game-engineer:web-game-engineer`.
5. Run a read-only test first. Verify it uses only the tools actually available.

The path is a placeholder; replace it with the extracted directory. This local flag loads the plugin for that session and is a development/test route, not a permanent marketplace installation.

## Manual fallback

If neither host import route is available, open the included `SKILL.md` and use its instructions in a supported Project or custom-instruction workflow. This is manual instruction use, not plugin installation.

## Known limitations

- Version: 0.2.0-alpha.
- Status: Experimental / NOT CERTIFIED.
- Claude.ai Skills upload and Claude Code plugin loading are independent and both remain unverified in a live host.
- MCP servers, terminal access, filesystem access, and subagents depend on host configuration.


## One-sentence build / 一句话构建

After loading the Skill/plugin, describe your website or game in one sentence. The adapter should infer safe defaults, build a complete runnable first version/playable vertical slice with tools actually available, test the main flow and report limitations. Target polished mid-to-upper-tier independent web/game quality, not an AAA guarantee. See [shared specification](../../core/ONE_SENTENCE_BUILD.md).
