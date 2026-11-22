# Install — DeepSeek

**Version:** 0.2.0-alpha · **Status:** Experimental / NOT CERTIFIED

## DeepSeek web/app chat
This ZIP is a portable instruction package, not a claimed native DeepSeek Skill/plugin archive.

1. Download and open `SYSTEM_PROMPT.md`.
2. In DeepSeek chat, paste the prompt at the beginning of a conversation when you want to use this workflow.
3. Attach the project files you want DeepSeek to inspect, if file upload is available.
4. Ask it to first inspect the files and report available tools before making changes.
5. For a new conversation, repeat the setup unless your account explicitly offers a persistent custom-instructions or agent configuration feature.

Do not assume that a prompt in one conversation persists to every conversation.

## DeepSeek API / custom agent
The official API supports a `system` message in Chat Completions and an `instructions` field in Responses API. Put the contents of `SYSTEM_PROMPT.md` into that system-level instruction field. Official references:
- Chat Completions: https://api-docs.deepseek.com/api/create-chat-completion/
- Responses API: https://api-docs.deepseek.com/api/create-response/
- Tool calls: https://api-docs.deepseek.com/guides/tool_calls/

If connecting tools, define each tool in your own client, validate model-generated arguments, execute only approved operations and return results. The model's tool-call output does not itself execute shell, file or Git actions.

Never paste an API key into chat or commit it. Store it in a secure environment variable or secret manager. API use may incur charges according to the account's current plan.

## Host validation
First test a read-only file summary. Then test a small reversible edit in a disposable project only if the active client really exposes file-write and execution tools. Record each tool and test result.

## Limitations
- No native DeepSeek web-chat Skill upload format is claimed by this adapter.
- DeepSeek API capability does not prove the consumer chat app has the same tools.
- Tool calls require a client/backend implementation; instructions cannot perform them on their own.
- **Actual DeepSeek host installation: NOT RUN. Certification: NOT CERTIFIED.**


## One-sentence build
Use one natural-language sentence to request a website/game. The Skill should build a complete runnable first version/playable vertical slice, use safe defaults, test available flows and report limitations. It does not guarantee AAA quality or grant missing host tools. Runtime certification remains NOT CERTIFIED.
