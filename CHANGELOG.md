# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added
- JobRadar24 own detail URL with company verified from page text (JSON-LD has
  no hiring organization name) (#1).
- Cauta.ro company-profile mapping and tolerant employer matching for portals
  that truncate the legal name in JSON-LD (#1).
- Enriched non-personal fields: location, salary, date and expiry date (#1).

### Changed
- Company identity set to PALAS INTERNATIONAL RESORT SRL (CUI `26293850`); config, docs
  and test fixtures rebranded (#1).
- Source identifier is now `mediere.anofm.ro, jobrapid.ro, bebee.com,
  jobica.ro, emprego.com, cauta.ro, jobradar24.ro` (#1).
- Stale-job scope covers all source URL prefixes (#1).

## [1.0.0] - 2026-11-19

### Added
- Python scraper for **PALAS INTERNATIONAL RESORT SRL** (CUI `26293850`), reading jobs
  from ANOFM (`mediere.anofm.ro`) and five other portals.
- Publisher to peviitor v1 API: company upsert, job upload, stale-job delete.
- ANAF company validation with CUIScan fallback and cache.
- Unit, integration, e2e, and consistency tests.
- GitHub Actions workflows and GitHub Pages (`docs/`) with generated `jobs.md`.
- AI documentation under `ai/`.
