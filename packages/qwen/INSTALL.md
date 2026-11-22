# Install — Qwen

**Version:** 0.1.0-alpha · **Status:** Experimental / NOT CERTIFIED

This adapter includes two independently supported Skill layouts. Choose the one matching your host.

## A. Qwen Code — Agent Skills
Qwen Code discovers personal Skills under `~/.qwen/skills/` and project Skills under `.qwen/skills/`.

1. Download `web-game-engineer-qwen-code-skill-0.1.0-alpha.zip`.
2. Extract the folder `web-game-engineer/` into either `~/.qwen/skills/` (personal) or the project folder `.qwen/skills/` (shared with the project).
3. Confirm the final path is `<skills-root>/web-game-engineer/SKILL.md`.
4. In Qwen Code, run `/skills` or invoke `/web-game-engineer`.
5. Ask Qwen Code to confirm the Skill name and version.

Official guide: https://qwenlm.github.io/qwen-code-docs/zh/users/features/skills/

## B. Alibaba Cloud Model Studio — Agent Skills
The separate Model Studio managed-agent service supports custom Skill ZIP uploads whose ZIP root contains `SKILL.md`.

1. Download `web-game-engineer-qwen-agent-skill-0.1.0-alpha.zip`.
2. Open the Model Studio / 百炼 console and enter Agent Skills management.
3. Upload the ZIP as a custom Skill and wait for the service-side review to finish.
4. Only after it becomes active, edit or create an Agent and attach this Skill version.
5. Run a small test task and confirm the agent selected the Skill.

Official guide: https://help.aliyun.com/zh/model-studio/managed-agents-skill

## Qwen Chat app fallback
If you only use the consumer Qwen chat app and no Skill/Agent configuration is exposed in your account, open `SYSTEM_PROMPT.md` and paste it at the beginning of the conversation. This is not a persistent Skill installation.

## Important
- Qwen Code, Model Studio managed Agents and the consumer Qwen app are separate host targets.
- Do not assume Model Studio Agent Skills are automatically available in Qwen Code or the consumer app.
- Qwen Code file/terminal permissions and Model Studio tools depend on the configured workspace and agent.
- **Actual host installation: NOT RUN. Certification: NOT CERTIFIED.**
