# Portable project state

Maintain: `project.json` (ID/name/type/schema/Core/module versions/enabled modules/status/targets/constraints); `PROJECT_CONTEXT.md` (goals and approved decisions); `ARCHITECTURE.md` (stack, boundaries, data flow, interfaces, budgets, rollback); `TASKS.json`; `DEVELOPMENT_LOG.md` (no secrets); `CHANGELOG.md`; `TEST_REPORT.json`; `KNOWN_ISSUES.md`; `HANDOFF.md`.

Project files are the cross-platform source of truth; chat memory is supplementary. Use explicit `schema_version`; migrations must be tested and must not silently discard fields. Suggested project types: web, 2d-game, 3d-game, 3d-workbench, mixed, other.

Example:
```json
{"schema_version":"1.0.0","project_id":"example","name":"Example","project_type":"web","core_version":"0.1.0-alpha","module_versions":{},"modules":{"web":true},"status":"planning","target_platforms":[],"constraints":[]}
```
