# System Reminder: package-updater-skip-update

- Source: inline

## Summary

PackageManagerAutoUpdater skips update when current version is at or above maxVersion.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | 2.1.47 | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
PackageManagerAutoUpdater: current version ${EXPR_1: '2.1.47'} is already at or above maxVersion ${EXPR_2}, skipping update
