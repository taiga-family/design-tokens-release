# design-tokens-release

Release pipeline for the npm package
**[@taiga-ui/design-tokens](https://www.npmjs.com/package/@taiga-ui/design-tokens)**.

This repository contains no sources. The package is built in the internal Taiga UI CI; on every release the CI pushes
the built package snapshot into [`package/`](./package) and tags it `v<version>`. The
[publish workflow](.github/workflows/publish.yml) then publishes `package/` to the public npm registry via **trusted
publishing (OIDC)** — no npm tokens are stored anywhere, and npm provenance attestations are generated automatically.

Commit history = history of published versions.
