# Install — Gemini Apps

**Version:** 0.1.0-alpha · **Status:** Experimental / NOT CERTIFIED

## Native Gemini Skills import
This package is built as a Gemini Apps Skill archive: the ZIP root contains `SKILL.md`, which is the required main-folder entry.

1. Open Gemini at https://gemini.google.com and sign in.
2. Open the Skills area (typically Customize/Personalize → Skills; labels may vary by account).
3. Choose Create → Upload.
4. Select `web-game-engineer-gemini-skill-0.1.0-alpha.zip` from this package's download.
5. Review the imported instructions, then choose Create.
6. Start a new chat and invoke `/web-game-engineer` or select the Skill where available. Also test whether Gemini automatically recognizes a matching task.

Google's current help describes uploading a SKILL.md file, a folder containing it, or a ZIP whose main folder contains it. It also notes account/age/availability restrictions; confirm that the Skills page is available to your account before relying on this route:
https://support.google.com/gemini/answer/17094296

## iPad / mobile note
The Gemini Skills upload route can vary by app/browser and account. If the iPad browser does not expose file upload, open Gemini in the browser's desktop-site mode or use the manual fallback below. Do not assume a successful download equals installation.

## Manual fallback
Open `SYSTEM_PROMPT.md` and paste it into a Gemini Gem or other persistent instruction area only if your account exposes one. This is a manual instruction setup, not a native Skill import.

## Host validation
Ask Gemini to identify the Skill and version, explain its project-protection rules, list only tools actually available, and classify a test task's checks as PASS/NOT RUN. Verify it can see an uploaded test file before authorizing edits.

## Limitations
- Gemini Apps Skills availability and management depend on account, age and app rollout.
- The Skill cannot grant Gemini shell, filesystem, browser automation, GitHub or deployment permissions.
- Scripts that need external network access are not bundled; do not assume Skill text can execute code.
- Gemini Apps installation and Gemini API integration are separate targets.
- **Actual Gemini host installation: NOT RUN. Certification: NOT CERTIFIED.**
