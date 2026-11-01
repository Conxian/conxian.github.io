# Conxian Public Repository Portfolio & Ecosystem Index

## Purpose

This site provides public orientation to the Conxian repository portfolio, links to relevant source repositories, and documents the active multi-cloud infrastructure, sovereign knowledge base topology, standards-alignment framework, and evidence-based valuation model.

## Status & Org-Wide Research Synthesis

This is an active public site maintained from `main` and deployed via GitHub Pages (`https://conxian.github.io`).

- **Ecosystem Alignment Status:** Active development. Per-repository release and CI status is authoritative (see the portfolio table and each repository's own README); this site is a static index, not a production status board.
- **Standards Alignment:** Components are *designed against* ISO 20022, ISO/IEC 27001, ISO/IEC 42001, ISO/IEC 25010, and ISO/IEC 20000-1 as reference frameworks. **Formal certification under these standards is not held.** These are alignment targets and internal design references, not accredited certificates.
- **Valuation:** The business is pre-revenue. The evidence-based range and the explicit criteria that would change it live in `conxian-business/docs/MNA_READINESS_VALUATION_2026_10_31.md`. Milestone figures are aspirational targets, not realized enterprise value.
- **Primary Issue Context:** System-wide valuation model refactoring, standards-adherence review, and KB research update per `https://github.com/Conxian/conxian-business/issues/1317`.

---

## Valuation: Speculative Milestones vs. Operational Reality

Legacy documentation recorded additive milestone target impacts in the $15B–$20B USD range. Milestones do not compound additively without underlying financial traction and cash flow.

Enterprise value is therefore evaluated only against operational evidence: measured costs, recognized revenue, and verified usage. At present:

- **Recognized revenue:** none (pre-revenue).
- **Measured operating cost:** ~$21/month (GitHub Code Quality licenses $20 + storage ~$1.3; GitHub Actions free on public repositories; Render and Neon on free tiers).
- **Paying customers:** 0. The first-revenue path is tracked in `conxian-business#1591`.

Where a figure cannot be supported by current evidence it is recorded as a target, not a realized value. See the M&A readiness and valuation framework documents in `conxian-business` for the full methodology.

---

## Standards Alignment Matrix

The table below records how each framework is *used as a design reference*. It is not a certification record.

| Standard | Domain / Scope | How it is used | Status |
|---|---|---|---|
| **ISO 20022** | Financial messaging | Rust middleware translating ISO 20022 MX message families (pacs, camt, pain) at the gateway boundary. | Design alignment |
| **ISO/IEC 27001** | Information security management | Secret management, pinned GitHub Actions SHAs, `CODEOWNERS`, row-level security on data stores. | Design alignment |
| **ISO/IEC 42001** | AI system governance | Agent budget boundaries, agent decision logging, auditable execution bounds. | Design alignment |
| **ISO/IEC 25010** | Software quality (SQuaRE) | Modular architecture, unit/integration test coverage, documented time-to-first-value. | Design alignment |
| **ISO/IEC 20000-1** | Service management | CI/CD pipelines, health checks, documented incident and change controls. | Design alignment |

Formal certification would require an accredited third-party audit; none has been completed.

---

## Deployment & Measured Usage

### Multi-Cloud Infrastructure & Service Mapping

1. **Supabase (BOS & Platform control planes)**
   - `Conxian BOS` (`yauldfcpswnufgwfvnlr`): business-operating-system state machine, milestone tracking, runway metrics, request attestations, compliance audit logs.
   - `Conxian-platform` (`iczqutrbbfudfzfplymc`): platform staging, secondary milestone verification, fleet metrics.

2. **Neon Serverless Postgres (data layer & multi-region nodes)**
   - `Conxian Nexus` (`orange-paper-76209725`): proof layer & `cnx_bos` schema repository.
   - `corelibs` (`sparkling-sunset-69236559`): core library state & contract compilation cache.
   - `Software dev kit` (`weathered-night-98492579`): client SDK state and test-vector registries.
   - `Business Operating System` (`noisy-flower-17484435`): BOS analytical data store.
   - `market` (`small-math-44741750`): market depth and settlement logs.
   - `Gateway` (`noisy-cloud-41146057`): ISO 20022 banking bridge state.

3. **Render (compute & service deployment)**
   - `My Workspace` (`tea-d4ufhh8gjchc73c80mu0`): web services, static documentation pipelines, cron workers.

### Measured Usage (current)

- **Paying customer accounts:** 0.
- **Treasury:** no treasury balance is reported here; the operating cost baseline is ~$21/month (measured). Do not treat any previously published treasury or customer figures as current — they were not evidence-backed and have been removed.
- **Runtime qualification:** the gateway's production deployment is tracked in `conxian-gateway#466`; source and CI do not establish production operation.

---

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
