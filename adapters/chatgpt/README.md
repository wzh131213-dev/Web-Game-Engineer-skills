# ChatGPT adapter

<badge>Experimental / NOT CERTIFIED</badge>

**Adapter version:** 0.1.1-alpha  
**Core version:** 0.1.0-alpha  
**Target:** ChatGPT web/app experiences only when the relevant feature is available. ChatGPT API or third-party wrappers require a separate adapter profile and are not covered by this status.

## Purpose

Expose the shared Web & Game Engineer Core inside ChatGPT without assuming that a prompt or Skill grants new tools or permissions. The adapter has three responsibilities:

1. Install or load the engineering instructions through a method actually available in the user's ChatGPT product.
2. Detect the tools available in the current conversation and select a truthful workflow.
3. Run the adapter acceptance suite and preserve evidence before any compatibility claim.

## Choose an installation route

The exact interface and feature availability can vary by account, plan, workspace and product release. Do not tell the user to click a control unless it is visible or documented for their environment.

### Route A — Native Skills (conditional)

Use this only if the user's ChatGPT interface explicitly exposes a Skills feature and accepts the package format provided by that feature.

1. Open the Skills management/import interface shown in that account.
2. Import the ChatGPT adapter package in the format the interface accepts.
3. Enable it for a test conversation.
4. Ask it to identify its version and summarize the safety rules.
5. Verify that it can find the Core instructions and that it does not claim unavailable tools.

If the interface does not expose Skills or rejects the package, stop. Do not describe the adapter as natively installed.

### Route B — ChatGPT Project instructions

Use this when Projects and project instructions are available.

1. Create a dedicated Project for Web & Game Engineer.
2. Copy `HOST_INSTRUCTIONS.md` into that Project's instructions.
3. Add `SKILL.md`, `core/ENGINEERING.md`, `modules/MODULES.md`, `team/ROLES.md` and `schemas/PROJECT_STATE.md` as project files/knowledge where supported.
4. Add only the task-relevant module files and project artifacts.
5. Start a new chat inside the Project and run the smoke tests in `TESTS.md`.

Project instructions and attached knowledge are a portable configuration route, not proof of native Skill installation.

### Route C — Custom GPT instructions/knowledge (conditional)

Use only if the account can create or configure a custom GPT.

1. Put `HOST_INSTRUCTIONS.md` in its instruction field.
2. Add the Core and relevant reference files to its knowledge area, respecting the host's file-count and size limits.
3. Keep actions/API integrations disabled unless separately reviewed and authorized.
4. Run the acceptance tests in a fresh conversation.

A custom GPT configuration is a separate deployment form; it does not mean the same package is installed as a native Skill.

### Route D — Current conversation

If none of the above options is available, attach or paste `SKILL.md` and the relevant Core references into the current conversation. This is session-scoped use only. Do not claim persistent installation or cross-chat availability.

## Capability detection

Before each substantial task, read `CAPABILITY_PROFILE.md` and classify each capability as AVAILABLE, LIMITED, UNAVAILABLE or NOT VERIFIED. The current conversation's actual tools take precedence over remembered or assumed features.

## Security and approvals

Follow the shared `SKILL.md` and `core/ENGINEERING.md` rules. Never request pasted passwords or API tokens. Confirm destructive edits, major architecture changes, remote pushes, deployments, public releases, external uploads, permission changes and paid operations. Routine in-scope work may proceed within the three-attempt repair limit.

## Certification

The adapter remains **NOT CERTIFIED**. Installation route, account context, model, tool access and test evidence must be recorded independently. See `CERTIFICATION.md` and `TESTS.md`.
