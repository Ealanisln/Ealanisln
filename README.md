# Emmanuel Alanis

**Full Stack Engineer & Tech Lead** | TypeScript, React, Next.js · Node (Hono, Express) · Python/Django · PHP/Symfony

I build and run production systems for real businesses: a Mexican non-bank lender (SOFOM), a Bay Area delivery company, an SF e-commerce site and a SaaS for veterinary clinics. Most of my time goes to shipping features, hardening security, keeping things observable, and writing runbooks other people can execute.

---

## 🚀 What I'm working on (2026)

### Crédito Express — Tech Lead (SOFOM, Mexico)
Loan-origination platform for payroll-deduction lending: credit applications, contract PDF generation, biometric identity verification (national-ID OCR, facial liveness), MFA/OTP, and legally binding document signing. Private repos; ~2,800 commits across 20+ services since Feb 2025.

**Stack:** React 18/19 · Vite · Node 22 · Hono 4 · Drizzle ORM · Python/Django 3.2 · PHP 8.2/Symfony 7 · MySQL 8 · PostgreSQL 15 · AWS (S3, EC2) · Docker · MediaPipe · Vitest · Playwright · PHPUnit/PHPStan

**Highlights:**
- Leading the migration of a Django + PHP backend to a TypeScript API (Hono + Drizzle) against the same databases, verified with shadow tests that replay real requests side by side
- Built a PDF document engine on `pdf-lib` (overlay/stamp, idempotent markers, barcodes, biometric signature stamps) replacing DOCX/reportlab templating
- Facial liveness app with MediaPipe, embedded via iframe in the main SPA; national-ID OCR and verification flows
- Planned and coordinated the production migration from a self-hosted VPS/PaaS to AWS (S3 mirror, DB migration, VPN, staged cutover), executed by the client's ops team from our runbooks
- Security hardening after an intrusion: safe model registry instead of dynamic code execution, host IDS + honeypot, WAF with IP bans, CSP, CORS/authz lockdown, MFA/OTP, PDF sanitization
- Observability: Prometheus/Grafana/Loki/Alertmanager stack, Sentry/GlitchTip across 6 apps, custom health dashboard
- Mentoring a small dev team (1:1s, PR review, requirements refinement with the Scrum/BA side)

### [Ready Set](https://github.com/ReadySet1/ready-set)
On-demand courier and catering delivery platform for the Bay Area (Food Safety and HIPAA certified). Lead developer since May 2025; ~1,400 commits, currently at **v2.7.0**.

**Stack:** Next.js 15.5 · React 19 · TypeScript 5.9 · Prisma 6 · Supabase (Postgres + Auth) · Stripe · Sanity CMS · Twilio · Resend · Mapbox · Cloudinary · Upstash Redis · Sentry-compatible tracking (GlitchTip) · Jest 30 · Playwright

**Highlights:**
- Driver app: GPS tracking, shift management, delivery state machine, idempotent shift starts
- Catering integrations (ezCater, CaterValley) and a partner API with authenticated endpoints
- Delivery pricing calculator, role-based access control, admin task boards
- Security sweeps (auth on all API routes, path-traversal removal, weekly `pnpm audit` + CodeQL)
- CI/CD: release-please versioning, multi-arch Docker images on GHCR, self-hosted on Dokploy, daily `pg_dump` backups with retention

### [Destino SF](https://github.com/ReadySet1/destino-sf)
E-commerce and catering platform for a San Francisco specialty food business. ~900 commits since March 2025.

**Stack:** Next.js 15.5 · React 19 · TypeScript 5.9 · Prisma 6 · Supabase · Square (payments + catalog) · Shippo · Resend + React Email · Google Maps · Mixpanel · Upstash Redis · Sentry · Jest 30 · Playwright + axe-core · Lighthouse CI

**Highlights:**
- Square as source of truth: catalog/inventory sync, webhooks, cron queues, payment processing
- Shippo shipping and database-backed delivery zones for catering
- Accessibility and performance gates in CI (axe, Lighthouse, bundle-size baseline)
- Weekly DB backups and security audits that auto-open tracking issues
- Diagnosed and fixed a production outage caused by a cron job disconnecting the shared Prisma client

### [Vetify](https://github.com/Ealanisln/vetify)
Multi-tenant SaaS for veterinary clinics: scheduling, medical records, billing. ~850 commits, currently at **v1.11**.

**Stack:** Next.js 15.5 · React 19 · Prisma 6 · Kinde Auth · Stripe + Square · FullCalendar · Sentry · Playwright

**Highlights:** subscription billing in local currency (MXN/CLP/COP/USD), trial lifecycle emails, tenant onboarding, PWA install flow, weekly E2E smoke suite.

---

## 💻 Tech Stack

### Frontend
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/-Tailwind_CSS-06B6D4?style=flat-square&logo=tailwind-css&logoColor=white)

### Backend & Database
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Hono](https://img.shields.io/badge/-Hono-E36002?style=flat-square&logo=hono&logoColor=white)
![Express](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white)
![Django](https://img.shields.io/badge/-Django-092E20?style=flat-square&logo=django&logoColor=white)
![Symfony](https://img.shields.io/badge/-Symfony-000000?style=flat-square&logo=symfony&logoColor=white)
![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Drizzle](https://img.shields.io/badge/-Drizzle-C5F74F?style=flat-square&logo=drizzle&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Supabase](https://img.shields.io/badge/-Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)

### Integrations & Services
![Stripe](https://img.shields.io/badge/-Stripe-008CDD?style=flat-square&logo=stripe&logoColor=white)
![Square](https://img.shields.io/badge/-Square-000000?style=flat-square&logo=square&logoColor=white)
![Twilio](https://img.shields.io/badge/-Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)
![Resend](https://img.shields.io/badge/-Resend-000000?style=flat-square&logo=resend&logoColor=white)
![Google Maps](https://img.shields.io/badge/-Google_Maps-4285F4?style=flat-square&logo=google-maps&logoColor=white)
![Sentry](https://img.shields.io/badge/-Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)

### Infra, Testing & DevOps
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Grafana](https://img.shields.io/badge/-Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Playwright](https://img.shields.io/badge/-Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/-Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Jest](https://img.shields.io/badge/-Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![pnpm](https://img.shields.io/badge/-pnpm-F69220?style=flat-square&logo=pnpm&logoColor=white)

---

## 🛠 Core Expertise

- **Full stack TypeScript:** Next.js App Router (Server Components, Server Actions), React 18/19 SPAs with Vite, Node APIs with Hono and Express, Zod validation end to end
- **Legacy modernization:** porting Django and PHP services to TypeScript against live databases, with shadow testing and behavior-parity gates instead of big-bang rewrites
- **Payments and commerce:** Stripe subscriptions and multi-currency billing, Square payments and catalog sync, Shippo shipping, order lifecycles with webhooks and queues
- **Identity and documents:** biometric liveness (MediaPipe), national-ID OCR, MFA/OTP over SMS and WhatsApp, PDF generation and digital signing
- **Security:** authz lockdowns, CSP, WAF and IDS, credential externalization, dependency audits and CodeQL in CI, incident response with commit-level timelines
- **Operations:** AWS migrations, Docker self-hosting (Coolify, Dokploy), Prometheus/Grafana/Loki, Sentry/GlitchTip, automated DB backups with retention, disaster-recovery plans
- **Quality:** Jest, Vitest, PHPUnit, Playwright (including accessibility and visual checks), PHPStan, coverage thresholds enforced in CI, release-please and Conventional Commits

---

## 📈 How I work

- **Runbooks as a deliverable:** when someone else runs production, the numbered steps, idempotent scripts, verification criteria and rollback plan are the product
- **Conventional Commits, CHANGELOGs and semver** across every repo I touch
- **Tests before push, CI as the gate:** lint, typecheck, unit, E2E, security audit, build checks
- **Observability first:** every app reports errors with fingerprints and has a health endpoint before it ships
- **Small team leadership:** dailies, 1:1s, PR reviews, written agreements, and requirement refinement before code starts

---

## 📫 Let's Connect

- **Email:** emmanuel@alanis.dev
- **Website:** [www.alanis.dev](https://www.alanis.dev)
- **Location:** Mexico · open to remote work

**Open to:** full-time positions, contract work, and interesting collaborations in financial services, logistics, e-commerce and SaaS.

---

<div align="center">
  <i>Building production systems that solve real business problems.</i>
</div>
