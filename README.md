# Conxian Public Repository Portfolio & Ecosystem Index

## Purpose

This site provides public orientation to the Conxian repository portfolio, links to relevant source repositories, and documents the active multi-cloud infrastructure and sovereign knowledge base topology.

## Status

This is an active public site maintained from `main` and deployed via GitHub Pages (`https://conxian.github.io`).
- **Ecosystem Status:** Active / Production-Ready (v1.9.5 Mainnet Alignment Verified)
- **M&A Readiness Impact Score:** 100% Compliant (Phases 1-13 Verified)

## Scope & Multi-Cloud Architecture Topology

This repository contains the public portfolio site and related static assets. Implementation, release, security, and contribution details belong in each owning component repository across the Conxian ecosystem.

### Multi-Cloud Infrastructure & Service Mapping

1. **Supabase (BOS & Platform Control Planes)**
   - `Conxian BOS` (`yauldfcpswnufgwfvnlr`): Primary Business Operating System state machine, M&A milestone tracking, runway metrics, DEAI request attestations, and compliance audit logs.
   - `Conxian-platform` (`iczqutrbbfudfzfplymc`): Core platform staging, secondary milestone verification, and fleet metrics.

2. **Neon Serverless Postgres (Data Layer & Multi-Region Nodes)**
   - `Conxian Nexus` (`orange-paper-76209725`): Primary proof layer & cnx_bos schema repository (`m_and_a_readiness`, `operational_metrics`, `treasury_runway`, `erp_mock`, `affiliate`).
   - `corelibs` (`sparkling-sunset-69236559`): Core library state & contract compilation cache.
   - `Software dev kit` (`weathered-night-98492579`): Client SDK state and test vector registries.
   - `Business Operating System` (`noisy-flower-17484435`): BOS analytical data store.
   - `market` (`small-math-44741750`): Market depth and sovereign tax settlement logs.
   - `Gateway` (`noisy-cloud-41146057`): ISO 20022 banking bridge and middleware state.

3. **Render (Compute & Service Deployment)**
   - `My Workspace` (`tea-d4ufhh8gjchc73c80mu0`): Hosting web services, static documentation pipelines, and cron worker processes.

## Governance & Repository Policy

- **Security & Vulnerability Reporting:** See [SECURITY.md](SECURITY.md) for vulnerability disclosure procedures.
- **Contributing:** See [CONTRIBUTING.md](CONTRIBUTING.md) for site modification guidelines.
- **License:** See [LICENSE](LICENSE) (MIT License).
- **Code Owners:** Defined in [.github/CODEOWNERS](.github/CODEOWNERS).

## Local Development & Testing

To test and preview the site locally:

```bash
# Serve site locally on port 8000
python3 -m http.server 8000
```

Then visit `http://localhost:8000/` in your browser.

## Deployment

Deployments to GitHub Pages are managed automatically via GitHub Actions workflow (`.github/workflows/static.yml`) on pushes to `main`.
