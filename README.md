# cloud-itonami-lei-988400qg33ws7jeiv602

> **Independent third-party archive/analysis. Not affiliated with, endorsed by, or sponsored by KEPCO (Korea Electric Power Corporation).**

Archives the publicly published Legal Notice (법적고지) of **KEPCO (Korea Electric Power Corporation)**, with source-url and retrieval-date
provenance, per ADR-2607110300. Read-only reference/archive repository — not a governed
Advisor/Governor actor. Part of the worldwide-scope extension (batch ASIA-UTIL-1, 2026-07-19).

## Company identity

- **Legal name**: KEPCO (Korea Electric Power Corporation)
- **LEI (ISO 17442)**: [988400QG33WS7JEIV602](https://search.gleif.org/#/record/988400QG33WS7JEIV602) (GLEIF entity-verified, KR)
- **Jurisdiction**: KR
- **Website**: https://www.kepco.co.kr
- **Ticker**: 015760 (KRX)
- **ISIC Rev.5**: 3510

## Contents

- `80-data/public/tos.journal.edn` — EDN quad-log of the archived Legal Notice (법적고지).
- `facts/catalog.edn` — 61 live-checked public-register citations (GLEIF, U.S. SEC EDGAR,
  the issuer's own Legal Notice), each an exact substring of a fetched response body,
  classified `:identity` / `:attribute` / `:definition`. The header records why the Korean
  register of record (RA000657, National Tax Service) cannot be cited per-entity.
- `tools/verify_citations.cljk` — nbb gate: GET every `:cite/url`, require HTTP 2xx and the
  expected substring (`nbb tools/verify_citations.cljk facts/catalog.edn --min 30`).
  Exit 0 = all checked, 1 = drift, 2 = could not answer.
- `NOTICE` — copyright/attribution statement.
- `blueprint.edn` — machine-readable company identity record.

## Design rationale

See ADR-2607110300 and the worldwide-scope extension ledger in `com-junkawasaki/root` (`90-docs/adr/`).
