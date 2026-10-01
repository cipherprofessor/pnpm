---
"@pnpm/napi": minor
---

`install()` accepts a `readPackageHookChecksum` option. The checksum is recorded as the lockfile's `pnpmfileChecksum`. While it stays the same, installs with a `readPackageHook` reuse the lockfile. Without it, every install with a hook resolves all dependencies again.
