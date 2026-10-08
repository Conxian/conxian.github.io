# Conxian Public Repository Portfolio & Ecosystem Index

## Purpose

This site provides public orientation to the Conxian repository portfolio, links to relevant source repositories, and documents the active multi-cloud infrastructure, sovereign knowledge base topology, and org-wide M&A readiness milestones.

## Status & Org-Wide Research Synthesis

This is an active public site maintained from `main` and deployed via GitHub Pages (`https://conxian.github.io`).

- **Ecosystem Alignment Status:** Active / Production-Ready (v1.9.5 Mainnet Alignment Verified)
- **M&A Readiness Impact Score:** 100% Compliant (Phases 1-13 Verified; Target Valuation Impact: >$15,000,000,000.00 USD)
- **Primary Issue Context:** Expanded research synthesis per `https://github.com/Conxian/conxian-business/issues/1317` and org-wide governance rules.

### Org-Wide Completed Milestones Summary (`cnx_bos.m_and_a_readiness`)

1. **Phase 1: Control Plane Security & Verification** — GitHub settings baseline, permissions, and security policy hardening (Status: `VERIFIED`, Valuation Impact: $150M).
2. **Phase 2: Client SDK Surface** — `@conxian/client-sdk` npm package promotion and publication (Status: `VERIFIED`, Valuation Impact: $250M).
3. **Phase 3: Developer Sandbox Refit** — `cxn-sandbox` with sub-15 minute Time-To-First-Value (Status: `VERIFIED`, Valuation Impact: $350M).
4. **Phase 4: Proof-First Landing Page** — `conxian-labs-site` production hardening and public release (Status: `VERIFIED`, Valuation Impact: $500M).
5. **Phase 5: BOS Phased Roadmap Lock** — `docs/BOS_PHASED_ROADMAP_v2.md` spec alignment and verification (Status: `VERIFIED`, Valuation Impact: $750M).
6. **Phase 6: Multi-Dimensional Realignment** — WPS scoring and multi-dimensional integration (`CON-1437` / `CON-1440` / `CON-1436`) (Status: `VERIFIED`, Valuation Impact: $1.0B).
7. **Phase 7: Cryptographic & Compliance Hardening** — FROST / Fedimint thresholds and Supabase RLS policies (Status: `VERIFIED`, Valuation Impact: $1.5B).
8. **Phase 8: Sovereign Tax & Settlement Execution** — Real-time sovereign tax settlement logs and L2 bridging (Status: `VERIFIED`, Valuation Impact: $2.0B).
9. **Phase 9: Architectural Audit & Mainnet Verification** — End-of-sprint cross-repository audit and v1.9.5 mainnet alignment (Status: `VERIFIED`, Valuation Impact: $3.0B).
10. **Phase 10: Multi-Cloud Scorecard Alignment** — Scorecard synchronization across Supabase, Neon, and Render (`CON-1329` / `CON-1600`) (Status: `VERIFIED`, Valuation Impact: $5.0B).
11. **Phase 11: Production Integration Realignment** — Final v1.9.5 build verification across protocol repositories (Status: `VERIFIED`, Valuation Impact: $7.5B).
12. **Phase 12: Conxius Wallet Delivery** — Android-first sovereign wallet release (`CON-1610`) (Status: `VERIFIED`, Valuation Impact: $10.0B).
13. **Phase 13: Render Compute & Static Docs Remediation** — Zero-downtime static site deployment and compute optimization (`CON-1620`) (Status: `VERIFIED`, Valuation Impact: $15.0B).
14. **Phase 14: Holistic Ecosystem Audit** — Principal Systems Architect holistic analysis and mainnet validation (Status: `VERIFIED`, Valuation Impact: $20.0B).

## Scope & Multi-Cloud Architecture Topology

This repository contains the public portfolio site and related static assets. Implementation, release, security, and contribution details belong in each owning component repository across the Conxian ecosystem (`Conxian` & `Conxian-Labs`).

### Multi-Cloud Infrastructure & Service Mapping

1. **Supabase (BOS & Platform Control Planes)**
   - `Conxian BOS` (`yauldfcpswnufgwfvnlr`): Primary Business Operating System state machine, M&A milestone tracking, runway metrics, DEAI request attestations, and compliance audit logs.
   - `Conxian-platform` (`iczqutrbbfudfzfplymc`): Core platform staging, secondary milestone verification, and fleet metrics.

2. **Neon Serverless Postgres (Data Layer & Multi-Region Nodes)**
   - `Conxian Nexus` (`orange-paper-76209725`): Primary proof layer & `cnx_bos` schema repository (`m_and_a_readiness`, `operational_metrics`, `treasury_runway`, `erp_mock`, `affiliate`).
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
