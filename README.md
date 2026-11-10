# Condor OTC: Case Study

> Cross-border payments and exchange platform. I built the financial integrations and the tooling the international desk runs on.

**The current version of this case study is on my site: [nahuelsoria.com/en/proyectos/condor-otc](https://nahuelsoria.com/en/proyectos/condor-otc).**

This repository is a public case study of work I led. It contains no proprietary code or confidential data, only an overview of the product, my role, and the engineering approach.

## Overview

Condor OTC moves and converts value across currencies, rails and providers for cross-border operations, and gives the desk the tooling to run it day to day.

## My role

CTO and technical lead.

## What I built

- Financial provider integrations for payments and exchange, each isolated behind a common internal interface so a provider can be added or swapped without touching core logic.
- Multi-rail, multi-currency flows across several corridors, including instant local rails and USD, EU and UK payment methods.
- Beneficiary verification for regulated corridors, with explicit match and mismatch handling.
- Compliance endorsement gating on regulated rails, fail-closed where the regulation requires it.
- Revenue and business-metrics tooling: accurate fee, margin and volume reporting for the desk.
- Internal desk tooling the operations team uses every day.

## Engineering approach

- Integration-heavy architecture, every provider behind a common internal interface.
- Correctness first on anything that touches money. Fees, netting and settlement are reconciled against real provider behaviour before shipping.
- Operational tooling built for speed and correctness under real desk workload.

## Stack

`TypeScript`, `Next.js`, `Node.js`, `PostgreSQL / Firebase`, payment and exchange provider APIs, `Vercel`.

## Outcomes

Live in production, supporting real international operations across multiple currency corridors.

---

Built and led by [Nahuel Soria](https://nahuelsoria.com/en) · [GitHub](https://github.com/nahuelsoria) · [LinkedIn](https://www.linkedin.com/in/nahuelsoria/)
