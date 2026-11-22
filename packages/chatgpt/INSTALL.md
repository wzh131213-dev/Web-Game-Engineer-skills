# ChatGPT package installation

**Version:** 0.2.0-alpha · Experimental / NOT CERTIFIED.

This is a portable instruction package. It does not assume every ChatGPT account supports native Skills import or ZIP import.

1. Choose a route actually available in your account: Project instructions, custom GPT instructions/knowledge, conditional native Skills import, or current-chat attachment.
2. Load `WEB_GAME_ENGINEER_CHATGPT.md`; keep a backup of existing instructions before replacement.
3. For a new website/game request, use one sentence. The adapter should infer safe defaults and build a complete first version when the host exposes the needed tools.
4. Run the acceptance prompts in `adapters/chatgpt/TESTS.md` in a clean conversation. Record real evidence; do not infer certification from a successful response.

Never assume file writing, code execution, browser control, GitHub access, API credentials or persistent storage. A current-chat attachment is session-scoped.

Downloads: [Unified six-platform GitHub Release](https://github.com/wzh131213-dev/Web-Game-Engineer-skills/releases/tag/v0.2.0-alpha-platform-bundle-20261123) · [Package Index](../../dist/packages/INDEX.md).
