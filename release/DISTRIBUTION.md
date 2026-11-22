# Package distribution contract

This is the mandatory distribution rule for every installable Skill and platform adapter in this repository.

## One package, one matching ZIP

For every `packages/<package-id>/` directory:

1. Include a `PACKAGE_MANIFEST.json` with `package_id`, `package_version` and a `files` array.
2. Include every file listed by the manifest, plus the installation guide and required assets.
3. The workflow creates `dist/packages/<package_id>-<package_version>.zip`.
4. The workflow validates the ZIP archive and creates a matching `.zip.sha256` checksum file.
5. The download index is written to `dist/packages/INDEX.md`.
6. The full product source is also packaged as `web-game-engineer-full-<release>.zip` with its SHA-256.

This applies to all platform adapters equally. Future platforms must be added as independent package directories, not hidden inside another platform's ZIP. One combined full-source ZIP does not replace each individual package ZIP.

## Build trigger

The GitHub Actions workflow runs when package sources or the release version change on main, and can also be started manually. It validates all package manifests and listed files before producing archives. It commits generated ZIPs and checksums to `dist/packages/` on main.

## Release truthfulness

- Workflow not yet completed: ZIP status is BUILD PENDING.
- Workflow completed and archive read back from GitHub: ZIP status is GENERATED / VALIDATED.
- Missing checksum or failed archive test: distribution FAILED.
- A generated ZIP does not mean the target AI host installed it or passed compatibility tests.
- Native Skill import support must be independently confirmed for each host.
