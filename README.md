# Awesome-Sales-Quotation-Proposal-Management

# Awesome Sales Quotation & Proposal Management

> A curated list of top Sales Quotation and Proposal Management platforms — both SaaS/Hosted commercial solutions and open-source alternatives for creating, sending, and tracking quotes and proposals that close deals.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [PandaDoc](#pandadoc)
  - [Proposify](#proposify)
  - [Qwilr](#qwilr)
  - [DealHub](#dealhub)
  - [Better Proposals](#better-proposals)
  - [Conga Composer](#conga-composer)
- [Open-Source Software](#-open-source-software)
  - [SwiftCPQ](#swiftcpq)
  - [Oreko](#oreko)
  - [Quote and Sign](#quote-and-sign)
  - [Core OSS](#core-oss)
  - [PactPop](#pactpop)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Sales Quotation and Proposal Management platforms. These are not open-source but are included as reference points for feature comparison.

### PandaDoc
**Type:** Proposal and contract management with e-signature  
PandaDoc provides proposal creation with custom templates, reusable content blocks, and a drag-and-drop editor. Features include real-time collaboration, approval chains, and alerts when recipients open or complete agreements. Integrates with payment processors for faster collection. ESIGN, UETA, and HIPAA compliant, SOC 2 certified [citation:8]. **Note:** The open-source alternative ecosystem for PandaDoc is limited—available tools like DocuSeal and OpenSign cover e-signature but lack PandaDoc's proposal analytics and interactive pricing tables [citation:8].

### Proposify
**Type:** Proposal software with design focus  
Proposify provides proposal creation with strong design templates, team collaboration, and tracking. It is often compared alongside Better Proposals and PandaDoc for sales teams wanting polished, branded proposals with approval workflows.

### Qwilr
**Type:** Interactive web-based proposals  
Qwilr turns proposals into interactive web pages rather than static PDFs, with embedded pricing tables, video, and acceptance tracking. Suited for sales teams wanting a modern, engaging proposal experience.

### DealHub
**Type:** CPQ with proposal generation  
DealHub provides guided quote configuration, adaptive pricebooks, and automated document generation for contracts and proposals. It supports every sales motion (new business, renewals, expansions) with native integrations into Salesforce, Dynamics, and HubSpot.

### Better Proposals
**Type:** Affordable proposal software  
Better Proposals focuses on proposal creation with strong design and basic tracking, positioned as an affordable alternative for freelancers and small teams. It includes e-signature and template libraries [citation:8].

### Conga Composer
**Type:** Template-based document generation for Salesforce  
Conga Composer merges data from Salesforce into Word, Excel, PowerPoint, and HTML templates for quotes, proposals, and contracts. Release 8 added a Template Builder with drag-and-drop field insertion. Suited for Salesforce organizations needing high-volume, data-driven document generation.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Sales Quotation and Proposal Management tools. The open-source ecosystem is **limited and fragmented**—most projects are early-stage, niche-focused, or cover only part of the proposal workflow (e-signature, invoicing, or quoting without full proposal tracking).

### SwiftCPQ
**Stack:** Vue.js / AGPL-3.0 | **License:** AGPL-3.0  
SwiftCPQ is an open-source proposal and quote generator designed for ICT consultants, developers, and Managed Service Providers (MSPs), positioned as an accessible alternative to ConnectWise CPQ, Kaseya Quote Manager, and Scalepad Quoter [citation:6][citation:2]. Features include an intuitive editor, version history, product catalogue, flexible recurrence pricing (upfront/monthly/annual), pricing tools (margins and discounts), and PDF templates. **Roadmapped but not yet implemented:** e-signature, web proposal view, approval workflow, REST API, and client portal [citation:6]. **Critical caveat:** The default branch has had no work since January 2025, and signatures/web proposal view remain on the roadmap—the project may be abandoned [citation:1][citation:12].  
**Best for:** MSPs and ICT consultants wanting a self-hosted CPQ foundation, accepting that e-signature and client-facing proposal views are not yet available.

### Oreko
**Stack:** TypeScript / Next.js / PostgreSQL / Stripe / AGPL-3.0 | **License:** AGPL-3.0  
Oreko is a self-hosted visual quote and invoice builder for freelancers, agencies, and small businesses, positioned as the open alternative to Bonsai and Bloom [citation:9][citation:4]. Features include a visual block-based quote builder, one-click quote-to-invoice conversion, client management with lifetime value tracking, contracts with e-signature (E-SIGN, UETA), Stripe payment integration, PDF generation, email notifications, dashboard analytics (revenue trends, quote conversion rates), and milestone payments. Deploys via Docker with PostgreSQL and Prisma [citation:9].  
**Best for:** Freelancers and small agencies wanting a self-hosted, AGPL-licensed quote and invoice platform with Stripe payments and e-signature built in.

### Quote and Sign
**Stack:** TypeScript / Cloudflare / AGPL-3.0 | **License:** AGPL-3.0  
Quote and Sign is an open-source proposal and quote platform for freelancers, studios, and small agencies, with a focus on **interactive, client-facing proposals** [citation:3][citation:13]. Key differentiator: clients receive a link (not a PDF), can toggle optional items and adjust quantities within limits, watch the total update, and accept by typing their name—all on their phone. Both parties receive a signed PDF plus a record page with a SHA-256 fingerprint proving what was agreed, when, and by whom. Includes seven templates, 16 currencies, flat pricing (no per-user seats), and runs on a free Cloudflare account. Business accounts can countersign and receive signed webhooks for CRM automation [citation:13].  
**Best for:** Freelancers wanting interactive, phone-friendly proposals with cryptographic acceptance records, deployable on free Cloudflare infrastructure.

### Core OSS
**Stack:** Next.js / Supabase / Tailwind / TypeScript | **License:** Open Source (per repository)  
Core OSS is a minimalist, extensible open-source CRM built with Next.js and Supabase, with a built-in **Offer Builder** for creating proposals with service line items, discounts, and terms [citation:5]. Features include a **Public Offer View** with shareable offer pages and email-gated acceptance, dashboard KPIs and offer history charts, and 5 core entities (Organizations, Contacts, Projects, Offers, Services). Designed to be extended with Claude Code. Setup requires Supabase configuration and environment variables [citation:5].  
**Best for:** Developers wanting a lightweight CRM foundation with built-in proposal/offer creation and public acceptance pages, extendable with AI assistance.

### PactPop
**Stack:** Next.js / Drizzle / PostgreSQL / PayPal / Open Source | **License:** Open Source (per project)  
PactPop is an open-source workspace for freelancers and small agencies that tracks client promises from the first message to payment confirmation, with **eight AI agents** handling intake, scope, pricing, proposal, operations, finance, proof, and payment [citation:11]. Key features include ScopeWatch (catches scope creep and prices change orders), ProofFlow (checks delivery against acceptance criteria), TrustGate (server-side permission checks on every agent tool call, with money actions having locked floors), and PayPal integration for real invoices and payment status. Amounts are computed in code (integer minor units), not by the model [citation:11]. **Note:** This is a Devpost hackathon project; production maturity should be evaluated carefully.  
**Best for:** Freelancers wanting a comprehensive promise-tracking workspace with AI agents and PayPal integration, accepting that the project is early-stage.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Quote Builder | E-Signature | Client Portal | Self-Hosted | Best For |
|----------|---------|-------|---------------|-------------|---------------|-------------|----------|
| **PandaDoc** | Proprietary | Cloud | ✅ Templates | ✅ | ✅ | ❌ | Full proposal + contract suite |
| **Proposify** | Proprietary | Cloud | ✅ Design-focused | ✅ | ✅ | ❌ | Polished branded proposals |
| **Qwilr** | Proprietary | Cloud | ✅ Interactive web | ✅ | ✅ | ❌ | Interactive web proposals |
| **SwiftCPQ** | AGPL-3.0 | Vue.js | ✅ CPQ-focused | (Roadmap) | (Roadmap) | ✅ | MSP CPQ foundation |
| **Oreko** | AGPL-3.0 | Next.js/Postgres | ✅ Visual block | ✅ | ✅ | ✅ | Freelancer quote + invoice |
| **Quote and Sign** | AGPL-3.0 | Cloudflare | ✅ Interactive | ✅ SHA-256 record | ✅ | ✅ | Phone-friendly proposals |
| **Core OSS** | Open Source | Next.js/Supabase | ✅ Offer Builder | (Email-gated) | ✅ Public view | ✅ | CRM + offer acceptance |
| **PactPop** | Open Source | Next.js/Postgres | ✅ AI-assisted | (PayPal records) | ✅ | ✅ | Promise tracking + AI agents |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Sales Quotation or Proposal Management tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem for **dedicated proposal management** is **very limited and fragmented**. Many available projects are early-stage or cover only part of the workflow: **SwiftCPQ** focuses on CPQ but may be abandoned [citation:1], **Oreko** combines quotes with invoicing, **Quote and Sign** excels at interactive client acceptance but not full proposal building, and **Core OSS** embeds offers within a CRM. No mature open-source project yet replicates PandaDoc or Proposify's full breadth of proposal analytics, content libraries, and team approval workflows. For teams needing a production-grade proposal platform today, commercial tools remain the practical choice.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
