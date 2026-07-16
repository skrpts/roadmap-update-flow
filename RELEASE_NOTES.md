# Release Notes

## v1.1.23
GH#845 — republish with American English (en-US) content, completing the source-only GH#805 flip that never reached the Hub. Copy only — no functional or behaviour change.

## v1.1.22
GH#753 — supply allocate-resources via `bindings: sprint_plan { from_step: "Progress Tracking" }` and re-pin to v1.0.3, fixing the previously-dangling {{steps.Sprint Planning.output}} ref. Also declare per-step `output: {name,type}` (GH#745). Canonical scan clean.

## v1.1.21
GH#645 Row 3b — migrate to K-037 dep-referenced schema. Strip 8 inline shared-content files and declare 8 hub-shared deps (UUID id + slug name + version + checksum from `gen-dep-checksums.mjs`). Closes pre-Step-3 inline-vendoring for this bundle.

## v1.1.20
Wave 2: re-signed with canonical engine signing pipeline.

## v1.1.19
Tags migrated inline into manifest (GH#586). tags.yaml retired.

## v1.1.18
Bundle re-signed with canonical engine signing pipeline (Wave 2 migration).

## v1.1.17
Signature fix — RELEASE_NOTES.md now included in integrity checksum.

## v1.1.16
Initial catalog release with full structural and content-quality validation. All scanner checks pass.
