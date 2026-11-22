# ChatGPT capability profile

This is a detection checklist, not a promise that a feature exists. Re-evaluate for every new conversation or materially different host environment.

| Capability | Detection evidence | State if not confirmed | Safe fallback |
|---|---|---|---|
| Read uploaded files | A real attachment is visible and readable through an available file tool | NOT VERIFIED | Ask for a supported upload or relevant excerpts |
| Create/edit files | A file-writing tool is actually available and succeeds | UNAVAILABLE | Return complete file contents and paths in chat |
| Run code | A code execution tool is available and executes a harmless test | NOT VERIFIED | Static review; label runtime tests NOT RUN |
| Browse public web | Search/open tool is available and succeeds | NOT VERIFIED | State that current web facts are unverified |
| Browser interaction | A browser-control tool is actually available | UNAVAILABLE | Provide user-operated steps |
| GitHub read | GitHub connector is connected and repository read succeeds | NOT VERIFIED | Ask for files or a repository link; use only available public read access |
| GitHub write | Connector confirms write permission and a write is explicitly authorized | UNAVAILABLE | Prepare patch/commit instructions only |
| Persistent project files | Project/file storage is available and the files can be reopened | NOT VERIFIED | Export project state files for user-managed storage |
| Real mobile device | Actual iOS/Android device test evidence exists | NOT VERIFIED | Mark viewport simulation as simulation, not device validation |
| External APIs | Explicit connector/API availability and authorized configuration exist | UNAVAILABLE | Mock external calls or provide integration instructions |

## State definitions

- **AVAILABLE:** directly observed and successfully used in this environment.
- **LIMITED:** available with constraints, quotas, user interaction or restricted scope.
- **UNAVAILABLE:** not exposed or access denied.
- **NOT VERIFIED:** not tested in this environment.

Record tool name only when useful; never include credentials, tokens or private identifiers. A capability detected in one conversation does not automatically carry over to another.
