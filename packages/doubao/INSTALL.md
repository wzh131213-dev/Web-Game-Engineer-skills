# Install — Doubao / 豆包

**Version:** 0.2.0-alpha · **Status:** Experimental / NOT CERTIFIED

## Doubao chat app
This is a portable instruction package, not a claim that the consumer Doubao app imports arbitrary Skill ZIPs.

1. Download and open `SYSTEM_PROMPT.md`.
2. Paste the prompt at the beginning of a Doubao conversation.
3. Attach project files if the current chat supports file upload.
4. Ask Doubao to inspect the project and list actual tools before editing.
5. Repeat in a new conversation unless your account explicitly provides persistent agent instructions.

## Volcengine Ark API / custom agent
Volcengine Ark Chat API supports a `system` message in the messages array. Put `SYSTEM_PROMPT.md` into that message when building an Ark-powered agent. The Ark API also supports function-calling flows for supported models; your application/backend must define and execute tools, validate arguments and return tool results.

Official references:
- Chat API and system message: https://docs.volcengine.com/docs/ark/chat-api?lang=zh
- Base URL and authentication: https://docs.volcengine.com/docs/ark/base-url-and-authentication?lang=zh
- Function calling: https://docs.volcengine.com/docs/ark/function-calling?lang=zh

The common Ark data-plane Base URL is documented as `https://ark.cn-beijing.volces.com/api/v3`; choose the correct region, endpoint/model ID and billing route from your own console. Never hardcode or expose API keys.

## ArkClaw / Agent template upload
Volcengine documentation describes a ZIP-based Agent template flow in ArkClaw, but that template is distinct from this portable Skill ZIP. This package does not claim to be an ArkClaw template. Use the ArkClaw-provided sample template and adapt the instructions only after checking its current schema.

## Host validation
Test a read-only task first. If using Ark API tools, ensure your backend actually executes tool calls and requires approval for risky file or remote operations.

## Limitations
- Doubao app chat and Volcengine Ark API are separate targets.
- Function calling is model decision output; external code must execute the function.
- No API key, paid service, backend, native consumer-app Skill import or ArkClaw template is bundled.
- **Actual host installation: NOT RUN. Certification: NOT CERTIFIED.**


## One-sentence build
Use one natural-language sentence to request a website/game. The Skill should build a complete runnable first version/playable vertical slice, use safe defaults, test available flows and report limitations. It does not guarantee AAA quality or grant missing host tools. Runtime certification remains NOT CERTIFIED.
