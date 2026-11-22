# DeepSeek target capability notes

- DeepSeek chat package type: portable system prompt; no native Web Skill import is claimed.
- API route: Chat Completions supports system messages; Responses API supports top-level instructions.
- Tool use: DeepSeek API documents function tool calls and server-side tools. A client must execute function calls and validate parameters; model text is not execution.
- Current API model IDs and features may change; select an available model in the account's current model list rather than hardcoding a model here.
- No API key, paid service, MCP server or backend is bundled.
- Installation state: NOT RUN. API integration test: NOT RUN. Certification: NOT CERTIFIED.

Official references:
- https://api-docs.deepseek.com/api/create-chat-completion/
- https://api-docs.deepseek.com/api/create-response/
- https://api-docs.deepseek.com/guides/tool_calls/
