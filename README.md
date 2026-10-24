# Documentation Wiki Project

> Custom documentation platform built on MediaWiki base. Solo-developed Bootstrap, CSS, JavaScript, and WCAG 2.1 AA accessibility compliance. Replaced PDF-only distribution with searchable web knowledge hub.

![Status](https://img.shields.io/badge/status-live-brightgreen)
![Accessibility](https://img.shields.io/badge/wcag-2.1%20AA-green)
![Stack](https://img.shields.io/badge/tech-MediaWiki%20%7C%20Bootstrap%20%7C%20JS-blue)

---

## Overview

When static PDFs stopped meeting user needs, I designed and built a fully custom documentation website from scratch. This wasn't a CMS template drop-in — it was a ground-up build using MediaWiki as the base, enhanced with custom Bootstrap styling, JavaScript interactivity, and strict WCAG 2.1 AA accessibility compliance.

The result: a searchable, mobile-responsive knowledge hub that improved information access speed. Owned and maintained solo for 7 years.

**At a glance:**

| Attribute | Detail |
| :--- | :--- |
| **Role** | Sole developer, designer, and maintainer |
| **Duration** | 2019 – Present (7 years active maintenance) |
| **Scope** | Full-stack documentation platform: frontend, backend configuration, accessibility audit |
| **Users** | Internal teams + external customers (public-facing) |
| **Status** | Live and actively maintained |

---

## What's Inside

```
/
├── README.md                     # This file
├── screenshots/
│   ├── homepage.png              # Site overview showing navigation
│   ├── search-interface.png      # Demonstrates improved discoverability
│   ├── mobile-view.png           # Responsive design proof
│   └── accessibility-report.png  # WAVE audit results
├── code-snippets/
│   ├── bootstrap-customization.js # Custom component overrides
│   ├── mediawiki-extensions.php  # Extension configuration
│   ├── custom-templates.php      # Page layout templates
│   └── wcag-accessibility-notes.md # Accessibility implementation details
├── configuration/
│   ├── LocalSettings.php         # MediaWiki core config
│   ├── skin-customization.css    # Theme override stylesheet
│   └── extension-list.txt        # Installed extensions with versions
├── content-migration/
│   ├── pdf-to-wiki-script.py     # Automation for bulk content migration
│   └── migration-log.md          # Documented migration process
├── accessibility/
│   ├── wave-audit-report.html    # Full WCAG validation output
│   ├── keyboard-navigation-test.md # Manual testing procedures
│   └── screen-reader-notes.md    # NVDA/JAWS compatibility notes
└── maintenance/
│   ├── backup-procedure.md       # Disaster recovery steps
│   ├── update-checklist.md       # Quarterly maintenance tasks
│   └── incident-log.md           # Downtime and issue tracking
```

---

## Background

Before this project, documentation distribution followed a broken model:

- **Static PDFs** emailed or posted as download links — no search, limited analytics.
- **Fragmented knowledge** — users couldn't find related topics; cross-references were manual.
- **Accessibility gaps** — PDFs weren't tagged for screen readers; mobile viewing was painful.

The constraint shaping the solution was straightforward: **zero engineering budget, one person with writing skills but self-taught web development knowledge, and a requirement to support both internal and external audiences.** Whatever I built had to be maintainable by one person without a dedicated IT team.

---

## Approach

Four technical decisions drove the architecture.

**1. MediaWiki over commercial CMS.**
Chose MediaWiki because it was open-source, familiar to technical writers, and required no licensing fees. The cost: steep learning curve for customization; required reading source code to understand extension hooks. 

**2. Bootstrap for responsive design.**
Selected Bootstrap for mobile-first grid system and pre-built components (navbars, accordions, modals). Avoided heavy frameworks (React, Vue) that would require build toolchains.

**3. Accessibility as requirement, not afterthought.**
Implemented WCAG 2.1 AA: semantic HTML, ARIA labels, keyboard navigation, color contrast compliance. Ran WAVE audits after every major change.

**4. Minimal plugin ecosystem.**
Installed only essential extensions (SyntaxHighlight, BatchUpload, etc.). Avoided bloating with unnecessary plugins that would break on MediaWiki updates.

---

## Outcome

- Complemented **PDF-only distribution model** with searchable web platform serving 40,000 monthly unique visitors.
- Achieved **WCAG 2.1 AA compliance** verified through automated (WAVE) and manual (screen reader) testing.
- Cut **information access time** from 5-10 minutes (PDF navigation) to under 60 seconds (search-based lookup).
- Enabled **self-service knowledge discovery** through faceted search and cross-referenced article links.
- Maintained platform for **7 years** with zero downtime incidents outside scheduled maintenance windows.

---

## Notes & Limitations

**Solo-maintained architecture.** All code, configuration, and content decisions were made by one person without formal software engineering training. Some patterns reflect pragmatic compromises rather than textbook best practices.

**MediaWiki version constraints.** Built on MediaWiki 1.43 LTS; upgrading to newer versions would require refactoring custom extensions and skin code. Migration path documented but not yet tested in production.

**No CI/CD pipeline.** Deployments were manual FTP/SFTP uploads with pre-deployment checklist. Modern pipelines (GitHub Actions, Jenkins) would improve reliability but were outside project scope.

**Browser support limitations.** Tested on Chromium and Gecko-based browsers. Older browsers may experience degraded functionality but remain functional.

---

## Accessibility Verification

### Automated Testing

| Tool | Result | Score |
| :--- | :--- | :--- |
| WAVE | Passed | 0 errors, 5 warnings (low severity) |
| axe DevTools | Passed | 0 violations |
| Lighthouse Accessibility | Passed | 100/100 |

### Manual Testing

| Test | Method | Result |
| :--- | :--- | :--- |
| Keyboard navigation | Tab through all interactive elements | Pass |
| Screen reader (NVDA) | Read full page with NVDA | Pass |
| Screen reader (VoiceOver) | Read full page with VoiceOver | Pass |
| High contrast mode | Windows High Contrast Mode | Pass |
| Zoom to 200% | Browser zoom without horizontal scroll | Pass |

---

## Related Projects

- [Portfolio and case study](https://tech-robert-pro.github.io)
- [Documentation templates](https://github.com/tech-robert-pro/documentation-templates)
- [Terminology management](https://github.com/tech-robert-pro/terminology-management)
- [LLM automation tools](https://github.com/tech-robert-pro/llm-tool-examples)
- [Hardware manual samples](https://github.com/tech-robert-pro/hardware-manual-samples)

---

## License

© 2026 Robert. All rights reserved.

Shared for portfolio and reference purposes. Custom skin code, JavaScript enhancements, and accessibility implementation are my original work. MediaWiki core and third-party extensions are subject to their respective licenses (GPLv2, MIT, etc.). Not licensed for commercial redistribution.

---

<!--
MAINTENANCE
Last reviewed: October 2026
Review cadence: Quarterly (security patches) + Annual (full audit)
Contact: tech.robert@protonmail.com
-->
