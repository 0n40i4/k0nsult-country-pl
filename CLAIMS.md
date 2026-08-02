# CLAIMS.md — public claim register (k0nsult-country-pl)

Generated from [`k0nsult-tools/docs/CLAIMS-TEMPLATE.md`](https://github.com/0n40i4/k0nsult-tools/blob/master/docs/CLAIMS-TEMPLATE.md)
(OSS-0-06).

| id | statement | class | proof_ref / roadmap_ref | repo_status_ref | verified_at |
|---|---|---|---|---|---|
| `clm-0001` | This repo ships 8 static HTML transparency surfaces (national/state oversight, digital-ministry, authority rankings PL+EN) as `surfaces/ai-truth-*.html`. | DOWOD | `surfaces/` directory listing — 8 files present (`ai-truth-kraj.html`, `ai-truth-panstwo.html`, `ai-truth-prezydent.html`, `ai-truth-min-cyfryzacji.html`, `ai-truth-ranking-jst-kas.html` + `-en`, `ai-truth-ranking-organy.html` + `-en`) | — | 2026-08-02 |
| `clm-0002` | This is the **reference implementation** of the per-country pattern; any EU Member State can instantiate the same structure via `k0nsult-country-template`. | NARRACJA | — (a positioning/design-intent statement; `k0nsult-country-template` exists as a sibling repo but "any Member State can instantiate" is not independently falsifiable from this repo) | — | 2026-08-02 |
| `clm-0003` | `/api/*` calls are the integration boundary; the k0nsult.cloud engine is proprietary and not in this repository. | NARRACJA | — (negative/scope claim: absence of engine code, true by omission — not something this repo's own files can prove) | — | 2026-08-02 |
| `clm-0004` | Whether the surfaces in this repo are served against a **live** `/api/*` backend today (vs. static-only) is undecided at the repo level. | GAP | `OSS-1-03` explicitly leaves the operator to choose between `RESEARCH_LAYER`-equivalent and `CONTROLLED_POC`-equivalent canonical status (WYMAGA_ACK: TAK) — no `x-k0nsult.status` has been written to `publiccode.yml` yet; `generator.config.yml` in `k0nsult-eu-shield` records this repo's status as `null` on purpose | `k0nsult-country-pl#x-k0nsult.status` | 2026-08-02 |
| `clm-0005` | This repo's SBOM (`sbom.json`) is a CycloneDX-lite inventory reproducible from this repo's own tree via `k0nsult-tools`. | DOWOD | `node ../k0nsult-tools/sbom.mjs --root . --out sbom.json --verify` | — | 2026-08-02 |

## Placeholder row (copy for new claims)

| id | statement | class | proof_ref / roadmap_ref | repo_status_ref | verified_at |
|---|---|---|---|---|---|
| `clm-00NN` | *(exact claim text)* | *(DOWOD\|GAP\|NARRACJA)* | *(ref, or "—" if NARRACJA)* | *(optional, or "—")* | *(YYYY-MM-DD)* |
