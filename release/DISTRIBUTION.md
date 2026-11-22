# Package distribution contract

## One package, one matching ZIP
For every `packages/<platform>/` directory:
1. Include a `PACKAGE_MANIFEST.json` with package ID, version and required file list.
2. Include the One-Sentence Build Mode in the actual entrypoint shipped to that platform (Skill, system prompt or host instructions).
3. Validate all manifest-listed files.
4. Generate a matching ZIP and SHA-256 sidecar.
5. Validate ZIP integrity and publish the download index.
6. Generate the full source bundle with Core, modules, benchmarks, docs, adapters and release workflows.

Every platform gets an independent package. The full-source archive does not replace platform ZIPs.

## Six-platform GitHub Release
The primary delivery is one GitHub Release containing the six main platform ZIPs and their SHA-256 sidecars. The Release workflow must run only after the package-generation workflow succeeds, read versions and archive paths from manifests, validate every checksum/ZIP, and never overwrite an existing immutable release.

## Truthful statuses
- Workflow not completed: BUILD PENDING.
- ZIP generated and read back from GitHub: GENERATED / VALIDATED.
- Missing file/checksum or invalid archive: FAILED.
- Host installation, actual tool execution and certification: separate evidence; never inferred from packaging.
