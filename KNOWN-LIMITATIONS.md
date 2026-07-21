# KNOWN LIMITATIONS — read before relying on this

**Status: REFERENCE / EXPERIMENTAL.** This repository ships **content surfaces** (HTML) for a national transparency layer — Poland as the reference instance. It is documentation of a state of affairs, not a live data service.

This file is published deliberately. Doctrine: **claim ≤ proof** — we document where this is
incomplete rather than overclaiming. The commons underwent internal adversarial review rounds
plus an external review (RSpace); findings and fixes are public in the git history.

## Known open weaknesses
- **The pages are a point-in-time snapshot.** Institutional names, competences and statuses
  change; nothing here refreshes itself. Verify against the primary source before relying on it.
- **Not legal advice.** The material is decision-support. Regulatory interpretation (AI Act and
  national implementing law) belongs to qualified counsel and the competent authority.
- **Poland-specific.** Structure is reusable (see `k0nsult-country-template`), but the content
  is not transferable to another Member State without substitution and re-verification.
- **No live API.** The surfaces are static; any dynamic behaviour would require the private engine,
  which is not part of this repository.

## What IS solid
- Apache-2.0 with the explicit patent grant; scoped NOTICE; SBOM with per-file SHA-256,
  re-derivable from a fresh clone.

## How to help
Try to break it and open an issue or PR with a reproducing input. That is exactly how the
limitations above were surfaced.
