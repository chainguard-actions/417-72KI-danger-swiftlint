<!-- markdownlint-disable -->

# Hardening Report: 417-72KI--danger-swiftlint/v6.4

> This file was generated automatically by the hardening agent.

**Policy SHA:** `d636be7e43ef829af6e853da6b3c7566db9f72fe`

**Test Policy SHA:** `843adf9e4b8f85d0c08b27b9d0b09dd094b54702`

**Harden Agent Version:** `2`

Action **417-72KI--danger-swiftlint/v6.4** was hardened automatically. 1 finding(s) were identified and resolved across 1 iteration(s).

## Findings Fixed

### unpinned-uses (severity: high)

The Docker action's runs.image uses a mutable tag instead of a SHA digest: `image: 'docker://41772ki/danger-swiftlint:6.4'`. Pin it to a digest, e.g. docker://41772ki/danger-swiftlint@sha256:<digest> # 6.4.

Locations:

- `action.yml:10`

## Iteration Notes

### Iteration 1

**Fixes applied:** unpinned-uses

**Notes:**

Pinned runs.image to docker://41772ki/danger-swiftlint:6.4@sha256:c23bb7c31f726d4d3795bdcdb952e922d460fb3097bc5f7b38854e00f3e7c9c9

