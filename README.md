# k0nsult-country-pl

The **Poland member-state layer** of the K0NSULT open commons — transparency and
oversight surfaces at the national level (state/president/ministry, authority and
JST-KAS rankings, PL + EN). This is the **reference implementation** of the
per-country pattern; any EU Member State can instantiate the same structure
(see `k0nsult-country-template`).

> **Doctrine:** `claim ≤ proof`; only agents are scored, never natural persons.
> Public-authority contacts on these pages are institutional registry data.

## Engine stays hidden
`/api/*` calls are the integration boundary; the k0nsult.cloud engine is proprietary
and **not** in this repository.

## Supply chain
`sbom.json` via [`k0nsult-tools`](../k0nsult-tools):
`node ../k0nsult-tools/sbom.mjs --root . --out sbom.json`

CI (`verify.yml`) fails the build if `sbom.json` is not byte-for-byte re-derivable
from the tree (`--verify`). To stop that failure at commit time instead of at CI
time, enable the shipped hook once per clone:
```
git config core.hooksPath .githooks
```
`.githooks/pre-commit` then regenerates and re-stages `sbom.json` automatically
before every commit (no-op, non-blocking warning if `../k0nsult-tools` isn't
cloned as a sibling).

## License
Apache-2.0 (patent grant, Section 3). See `LICENSE` and `NOTICE`.
