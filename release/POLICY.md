# Version, release, certification and package distribution

The current release is 0.2.0-alpha. Core, modules and all six platform adapters are versioned independently, but are aligned for this alpha milestone. GitHub is the official source; the unified GitHub Release is the primary six-platform download route.

## One-sentence product contract
Each shipped platform entry point must include the One-Sentence Build Mode. A sentence is treated as a complete creative brief; non-blocking details are inferred; implementation produces a complete runnable first version/playable vertical slice where host tools permit. The target is polished independent web/game quality, not an AAA guarantee.

## Mandatory ZIP rule
Every distributable adapter must have its own matching ZIP and SHA-256 sidecar. Each package contains its manifest, install/use instructions and every file listed by its manifest. A full-source ZIP is also generated. Archives must pass unzip validation; a missing manifest, required file, archive or checksum is a distribution failure.

## Release and certification
All six adapters remain Experimental / NOT CERTIFIED until actual host installation, capability detection, benchmark, project handoff, security, regression and delivery tests pass independently. A generated ZIP proves package integrity only—not native import, runtime compatibility, quality score or certification.

L1-L2 manual/instruction-led capabilities remain Experimental. L3-L4 may qualify for certification but are not automatic passes. Revalidate at least every 90 days and after major host/tool changes or severe defects. Suspend certification for confirmed severe security/data-integrity issues.

Public Stable releases, external uploads and deployment require user approval. Do not claim AAA quality, platform compatibility or runtime success without direct evidence.
