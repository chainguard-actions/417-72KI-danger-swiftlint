<!-- markdownlint-disable -->

# Hardening Report: 417-72KI--danger-swiftlint/v6.3

> This file was generated automatically by the hardening agent.

**Policy SHA:** `d636be7e43ef829af6e853da6b3c7566db9f72fe`

**Test Policy SHA:** `843adf9e4b8f85d0c08b27b9d0b09dd094b54702`

**Harden Agent Version:** `2`

Action **417-72KI--danger-swiftlint/v6.3** was hardened automatically. 1 finding(s) were identified and resolved across 1 iteration(s).

## Findings Fixed

### unpinned-uses (severity: high)

The Docker action's runs.image uses a mutable tag instead of a SHA digest: `image: 'docker://41772ki/danger-swiftlint:6.3'`. Pin it as docker://41772ki/danger-swiftlint@sha256:<digest> # 6.3.

Locations:

- `action.yml:10`

## Iteration Notes

### Iteration 1

**Fixes applied:** unpinned-uses

**Notes:**

Pinned runs.image to docker://41772ki/danger-swiftlint:6.3@sha256:cb813baec3083dc3eb56b7444d86fff2b3eea97751147a7ca7a578584e60e791 (docker:// scheme and tag kept inline).

