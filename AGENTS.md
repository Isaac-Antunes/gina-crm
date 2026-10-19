# Agent Instructions & Repository Guidelines (`AGENTS.md`)

## 🎯 Primary Objective
Maintain and polish **Gina CRM (`gina-crm`)**—the static showcase and visual brand repository companion to [`gina-training-lab`](https://github.com/Isaac-Antunes/gina-training-lab)—to meet top-tier engineering, security, and technical documentation standards in clear, professional English.

---

## 🔒 Security & Static-Site Invariants (CRITICAL)
1. **Pure Static Architecture:**
   - This repository is published via GitHub Pages as pure static HTML5 and CSS.
   - Do **not** introduce runtime JavaScript bundles, tracking pixels, cookies, external form endpoints, or backend credentials.
2. **Zero Secrets or Real Customer Data:**
   - Never commit API keys, tokens, `.env` files, Salesforce org URLs, or real customer PII. All examples and visual plates must use 100% synthetic data.
3. **Cross-Repository Consistency:**
   - Keep architectural claims (10-stage deterministic precedence, `1.5x` rhythm boundary, `3.0x` dormancy boundary, top-third RFV competition ranking, 99% Apex coverage across 17 tests, and 47 local evaluation challenges) strictly aligned with the canonical implementation in [`gina-training-lab`](https://github.com/Isaac-Antunes/gina-training-lab).

---

## 📂 Repository Hygiene
- **Root Directory:** Keep only static entrypoints (`index.html`, `404.html`, `robots.txt`, `sitemap.xml`, `.nojekyll`), `LICENSE`, and top-level markdown documentation (`README.md`, `SECURITY.md`, `AGENTS.md`).
- **Assets:** Keep README banners inside `docs/`, Behance case-study plates inside `behance/`, and site styles/SVGs inside `assets/`.
- **Localization:** Write all markdown documentation, commit messages, and pull request descriptions in clear, publication-grade technical English.
