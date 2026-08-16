# Conxian Public Repository Portfolio

## Purpose

This site provides public orientation to the Conxian repository portfolio and links to relevant source repositories.

## Status

This is an active public site maintained from `main` and deployed via GitHub Pages.

## Scope & Repository Policy

This repository contains the public portfolio site and related static assets. Implementation, release, security, and contribution details belong in each owning component repository.

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
