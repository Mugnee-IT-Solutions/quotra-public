# Quotra — LED Display Quotation & Estimation

**Quotra** is a professional, field-ready solution for teams who sell and specify LED display projects. It streamlines quoting from first conversation to a polished, branded client document—so your sales process stays consistent, fast, and credible.

---

## Overview

Businesses that sell LED screens often juggle product options, pricing tiers, taxes, discounts, and installation details across spreadsheets, messages, and ad-hoc documents. That slows deals down and increases the risk of inconsistent numbers or outdated prices.

**Quotra** addresses this by giving estimation and sales teams a single, guided workflow: configure the display and commercial terms, see clear totals and summaries, and produce a professional PDF your clients can trust. The experience is designed to work **even when connectivity is unreliable**, so quotations can be prepared on-site or while traveling without losing momentum.

---

## Key Features

- **Guided quotation workflow** — Step-by-step flow from client and project details through product selection and commercial terms.
- **Consistent pricing logic** — Structured handling of display technologies, configurations, tiers, VAT, discounts, and related line items so quotes stay aligned with your rules.
- **Branded PDF output** — Client-ready documents that reflect your brand and present the quotation clearly.
- **Offline-first reliability** — Core quoting and PDF generation work without a constant internet connection; optional connectivity supports staying up to date when available.
- **Optional catalog refresh** — When online, pricing and catalog data can be refreshed so field teams are not stuck on stale numbers.
- **Secure-by-design posture** — Sensitive implementation details and integrations are kept private (see **Source code notice** below).

---

## Industry & Use Case

**Industry:** Pro AV, digital signage, LED display sales, and systems integration.

**Typical use cases:**

- Sales engineers preparing quotations during client visits or trade events  
- Deal desks standardizing LED display estimates across regions or partners  
- Organizations that need **repeatable, auditable** quotes instead of one-off spreadsheets  

---

## System Workflow

1. **Capture context** — Enter client and project information relevant to the quotation.  
2. **Configure the display** — Select display type, sizing, technology, and related options according to your catalog and rules.  
3. **Apply commercial terms** — Set taxes, discounts, payment or warranty choices, and any add-ons your process includes.  
4. **Review the summary** — Confirm totals, structure, and narrative consistency before export.  
5. **Generate and share** — Produce a branded PDF for the customer; optional background steps may run when connectivity allows, without blocking local success.  

---

## Tech Stack

This product is delivered as a **native Android application**, built for reliability on commercial devices used in the field.

| Area | Technology |
|------|------------|
| Platform | Android (modern API levels) |
| Language | Kotlin |
| User interface | Jetpack Compose, Material Design3 |
| Architecture | Structured layers for catalog, domain logic, export, and presentation |
| Data & serialization | Type-safe models and efficient JSON handling |
| Local persistence | Android DataStore for preferences and cached catalog state |
| Networking | Industry-standard HTTP client for optional online sync |
| Documents | PDF generation tailored for quotation layouts and annexes |
| Build & delivery | Gradle-based Android toolchain (debug, test, and release pipelines) |

---

## Screenshots

Add your product imagery under the `screenshots/` folder and reference the files below for a polished GitHub landing page.

**Suggested filenames:**

| File | What to show |
|------|----------------|
| `./screenshots/01-dashboard-or-home.png` | Entry point or main overview |
| `./screenshots/02-quotation-wizard-step.png` | Mid-flow configuration screen |
| `./screenshots/03-summary-review.png` | Totals and review before export |
| `./screenshots/04-pdf-export-or-share.png` | Export, share, or success state |
| `./screenshots/05-sample-pdf-first-page.png` | Representative first page of a generated PDF (sanitized) |

**Placeholder layout (replace with your assets):**

<p align="center">
  <img src="./screenshots/01-dashboard-or-home.png" width="32%" alt="Quotra — main experience" />
  <img src="./screenshots/02-quotation-wizard-step.png" width="32%" alt="Quotra — configuration step" />
  <img src="./screenshots/03-summary-review.png" width="32%" alt="Quotra — summary review" />
</p>

<p align="center">
  <img src="./screenshots/04-pdf-export-or-share.png" width="32%" alt="Quotra — export and share" />
  <img src="./screenshots/05-sample-pdf-first-page.png" width="32%" alt="Sample branded PDF output" />
</p>

---

## Architecture (high level)

At a conceptual level, **Quotra** separates concerns so the product stays maintainable and safe to evolve:

- **Presentation** — The guided user experience and state that sales teams interact with.  
- **Domain** — Business rules for pricing, eligibility, and quotation structure—the “source of truth” for how numbers are computed.  
- **Catalog & data** — Bundled defaults combined with optional refreshed data, merged in a controlled way for predictable results.  
- **Export** — Document generation and optional non-blocking integration hooks, designed so a successful local export is never held hostage by network conditions.  

No implementation code is published in this repository; the description above reflects how the system is organized for **clarity and governance**, not for replication.

---

## Source code notice

The **full source code, internal integrations, and deployment assets** for this solution are **private**. This protects client confidentiality, commercial terms, security configurations, and intellectual property.

If you are evaluating a similar build for your organization, we are happy to discuss scope, timelines, and an appropriate delivery model under NDA where required.

---

## Company

**Mugnee IT Solution**  
Website: [https://mugneeit.com](https://mugneeit.com)

---

## Get in touch

If you need a **custom quotation tool**, **mobile-first sales application**, or **integrated document workflow** for AV, signage, or complex configurable products, contact **Mugnee IT Solution**. We design solutions that balance **usability for sales teams**, **strictness for finance and operations**, and **professional presentation** for your customers.

**[Visit mugneeit.com](https://mugneeit.com)** to start a conversation about a solution tailored to your business.
