# Cross-platform one-sentence build benchmarks

Run each benchmark independently on every platform target. All cases begin as NOT RUN until a host-controlled execution produces evidence.

1. **Web:** “Build a polished responsive outdoor photography studio site with a portfolio, service packages, validated booking form and mobile navigation.” Expect complete responsive site and real form behavior, not fake booking.
2. **2D game:** “Create a mobile 2D arena survival game where a pilot dodges drone waves, collects upgrades and survives a boss.” Expect playable loop, collision, upgrades, pause/restart and clear completion states.
3. **3D game:** “Create a stylized 3D island exploration game with third-person movement, collectible artifacts, cliffs, water and a clear objective.” Expect visible scene, camera, movement, collision, objectives and cleanup.
4. **3D workbench:** “Build a browser 3D editor where I can add primitives, select/transform objects, edit materials, undo and export.” Expect add/select/transform/inspect/undo/export.
5. **Touch:** “Create a portrait arcade game with a virtual joystick and two action buttons.” Expect simultaneous touch, touch-cancel/focus-loss handling, usable hit targets and safe areas.
6. **Legacy project:** “Add a settings panel to this existing game without changing movement, scoring or saves.” Expect scoped edits and regression evidence.
7. **Polish pass:** “Make this game feel faster and more satisfying while preserving controls and level progress.” Expect measured/tunable changes without unrelated regression.
8. **Implicit design defaults:** omit exact colors/fonts/layout. Expect coherent defaults without a questionnaire.
9. **Delivery:** every result includes source, run steps, controls, actual tests, known issues and a reproducible artifact or exact host limitation.

## Mid-to-upper-tier scorecard
Review 1–5 with evidence; target 4/5 for: functional completeness; interaction/game feel; visual coherence/art direction; stability/measured performance; responsive/accessibility/input; maintainability/testability. This is a review aid, not certification or an AAA promise. Write NOT MEASURED when evidence is unavailable.

Record exact prompt, host/product/model/version, adapter, tools, expected/actual behavior, tests, evidence and defects. Also test installation, security, schema migration, rollback and cross-platform handoff.
