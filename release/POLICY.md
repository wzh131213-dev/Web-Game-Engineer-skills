# Version, release, certification and package distribution

Core, each Module, each Adapter and each installable Skill package have independent versions. Stable, Beta and Experimental are distinct. GitHub is the official source.

## Mandatory ZIP rule

**Every distributable Skill or platform adapter must have its own ZIP archive.** This applies equally to ChatGPT, Claude, Gemini, DeepSeek, Qwen, Doubao and every future platform or standalone Skill package. No platform receives a ZIP-only exception or a folder-only exception.

- Each package lives in its own `packages/<package-id>/` directory.
- Each package must include `PACKAGE_MANIFEST.json`, install/use instructions, the complete files required for that package, its package version and certification status.
- The automated distribution workflow builds one ZIP per package using the name `<package_id>-<package_version>.zip`.
- A SHA-256 sidecar file is generated for every ZIP.
- A full-source ZIP is also generated for the overall product release.
- Every archive is tested with `unzip -t`; manifest-listed files are checked before packaging.
- Generated archives, checksums and a download index are committed under `dist/packages/` on `main`, so they remain visible in the repository rather than existing only as temporary workflow artifacts.
- A package is not considered distributable if its manifest is missing, a required file is missing, ZIP validation fails or its checksum is absent.
- Never claim an archive is ready until the workflow has completed and the actual ZIP and checksum files have been read back from GitHub.

Platform adapter documentation outside `packages/` is design/source documentation, not a completed installable distribution package. Before calling a platform package released, create its independent `packages/<platform>/` directory and manifest; the workflow will then produce its matching ZIP.

## Release and certification

Certification levels: L1 basic guidance; L2 instruction-led/manual execution; L3 main tools work with some manual steps; L4 full workflow tools. L1-L2 remain Experimental. L3-L4 may apply for certification but do not automatically pass.

Each platform independently passes actual installation, capability detection, benchmarks, project handoff, security, regression and delivery tests. Revalidate at least every 90 days and after major host/tool changes or severe defects. Suspend affected certification for confirmed severe security/data-integrity issues.

Build adapters concurrently where possible; isolate failures. Unfinished platforms may receive Experimental packages but must not be called formally compatible. A ZIP archive proves only that a source package was packaged and validated; it does not prove installation, runtime compatibility or certification.

Public Stable releases, deployment and external publication still require user approval. The package ZIP generation workflow only writes package archives and checksums to this repository's `main` branch.
