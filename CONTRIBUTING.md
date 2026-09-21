# Contributing to Conxian Web Site

Thank you for your interest in contributing to the Conxian ecosystem public portfolio site.

## Principles & Guidelines

1. **Self-Contained & Lightweight:**
   - Avoid external heavy dependencies or CDN imports.
   - Maintain the utility-first CSS structure in `css/common.css`.

2. **Security & Public/Private Boundaries:**
   - Never commit sensitive secrets, `.env` files, or internal operational details.
   - Maintain strict separation between public portfolio references and private operational code.

3. **Workflow & Pull Requests:**
   - Create a feature branch for your changes.
   - Verify local site rendering by serving locally:
     ```bash
     python3 -m http.server 8000
     ```
   - Ensure changes pass visual and static validation.
   - Open a clear, descriptive Pull Request targeting `main`.

4. **Security Disclosures:**
   - Refer to [SECURITY.md](SECURITY.md) for reporting security concerns or sensitive data leaks.
