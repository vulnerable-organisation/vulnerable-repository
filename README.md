# Claimable Dependency Demo

This repo intentionally references a **nonexistent** scoped package:
`@example-business/utils@1.0.0`.

- `.npmrc` -> `registry=https://registry.npmjs.org/`
- CI runs `npm ci`
- `npm view @example-business/utils --registry https://registry.npmjs.org/` returns 404

This is a safe demonstration of **Dependency Confusion / Package Namespace Hijacking**.
