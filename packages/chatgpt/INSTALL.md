# ChatGPT package installation

**Version:** 0.1.2-alpha · **Status:** Experimental / NOT CERTIFIED

This is a portable source package. It does not assume that all ChatGPT accounts support native Skills import or ZIP import.

## 1. Project route (if Projects are available)
1. Create a dedicated Project.
2. Copy the contents of `WEB_GAME_ENGINEER_CHATGPT.md` into Project instructions (or split the document into instructions and knowledge if the interface requires it).
3. Keep the same file as Project knowledge if supported, and add task-specific project files separately.
4. Start a fresh chat in the Project and run the smoke tests below.

## 2. Custom GPT route (if GPT configuration is available)
1. Create/configure a custom GPT using the interface exposed by your account.
2. Put the portable instruction document into its instruction field, or divide it between instructions and knowledge according to product limits.
3. Do not enable external Actions unless separately reviewed and approved.
4. Test in a fresh conversation.

## 3. Native Skills route (conditional)
Only use if your ChatGPT interface explicitly exposes Skills import and documents an accepted format. Follow that UI's requirements. If absent or rejected, stop. Do not rename this directory to .skill and claim it is installed.

## 4. Current conversation fallback
Attach or paste the portable instruction document into the current chat. This is session-scoped and does not persist automatically to other chats.

## Smoke tests
Ask the assistant to report its Core/adapter versions, enumerate only actually available tools, explain how it protects existing projects, identify actions requiring approval, and distinguish NOT RUN from PASS. Then test file inspection, one scoped change, regression reporting, and project handoff. Record evidence. A convincing answer alone does not certify host tools.

## Update and backup
Back up existing Project/GPT instructions and knowledge before updating. Compare package versions first. Never overwrite user project state with package defaults. Use the repository as source of truth:
https://github.com/wzh131213-dev/Web-Game-Engineer-skills/tree/main/packages/chatgpt

## Not yet provided
The GitHub directory is source distribution only. ZIP archive and SHA-256 are NOT GENERATED in this release. Do not advertise them as downloadable artifacts until a release build creates and validates them.
