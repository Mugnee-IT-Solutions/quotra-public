# Quotra — LED Display Quotation & Estimation

**Quotra** is a professional, field-ready solution for teams who sell and specify LED display projects. It streamlines quoting from first conversation to a polished, branded client document—so your sales process stays consistent, fast, and credible.

<div align="center">

<img src="./screenshots/01-splash-brand.jpeg" width="260" alt="Quotra — branded splash screen" />

*Polished first impression — consistent brand from the moment the app opens.*

</div>

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

Below is the product experience in **workflow order** — from the guided home screen, through pricing controls, to the final quotation ready to save or share.

### Guided start — six-step workflow & live totals

The home experience shows where you are in the process, keeps key numbers visible, and lets users jump to any step when needed.

<p align="center">
  <img src="./screenshots/02-home-six-step-workflow.jpeg" width="40%" alt="Quotra — six-step quotation workflow and live totals" />
</p>

### Commercial controls — “At a glance” + pricing & payment

Teams can tune frames, installation, VAT, and discounts while the running total stays transparent for faster decisions on-site.

<p align="center">
  <img src="./screenshots/03-pricing-and-at-a-glance.jpeg" width="40%" alt="Quotra — at-a-glance summary and pricing options" />
</p>

### Final quotation — review, PDF, save & share (offline-friendly)

The last step consolidates the technical breakdown and totals, with clear actions to **save** or **share** — including reassurance that PDF creation works on-device when connectivity is limited.

<p align="center">
  <img src="./screenshots/04-summary-save-and-share.jpeg" width="40%" alt="Quotra — quotation summary with save and share" />
</p>

**Gallery index**

| # | File | What it highlights |
|---|------|--------------------|
| 1 | `screenshots/01-splash-brand.jpeg` | Brand-forward splash (also shown at the top of this page) |
| 2 | `screenshots/02-home-six-step-workflow.jpeg` | Six-step navigation and live grand total / payable |
| 3 | `screenshots/03-pricing-and-at-a-glance.jpeg` | Running summary plus VAT, discounts, and estimate modes |
| 4 | `screenshots/04-summary-save-and-share.jpeg` | Final review, PDF tab, save/share, Step 6 of 6 |

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
