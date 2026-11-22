# Engineering standards

## Roles
Project Manager: scope, milestones, risks, approvals, delivery. Architect: stack, boundaries, interfaces, migrations. Web Engineer: HTML/CSS/JS/TS, responsive UI, accessibility. Game Engineer: gameplay, scenes, maps, camera, input. Physics Engineer: rigid bodies, collision, vehicle/character/environment physics, numerical stability. Technical Artist: procedural geometry, materials, lighting, effects, LOD, budgets. QA: acceptance criteria, automation, regression, visual/performance tests and truthful reports.

## Quality priority
P0 data safety/correctness; P1 stability/usability; P2 performance; P3 polish/noncritical features. Never sacrifice P0/P1 for P2/P3. Degrade distant detail, shadow resolution, post-processing, particles and decorative features first. Never silently degrade core input, collision, saves or critical interactions.

Measure FPS, memory, draw calls, polygon counts, texture sizes, startup and asset size; report NOT MEASURED when not measured. Mobile checks include touch, orientation, safe areas, soft keyboard, focus loss and real-device limits.

## Security
Never request chat-pasted passwords/tokens. Inject secrets securely; do not commit them. Confirm destructive/remote/paid operations. Record third-party versions, origins and licenses; produce SBOM. Review external scripts/assets. Stop on suspected data corruption or severe security issue.

## Tests
PASS=executed and passed; FAIL=executed and failed; PARTIAL=incomplete; NOT RUN=not executed; MANUAL=requires user/real host/device. Separate static, unit, integration, end-to-end and physical-device testing. Report environment, versions, commands, counts, failures, unverified items and evidence. Max three repair attempts per root cause.
