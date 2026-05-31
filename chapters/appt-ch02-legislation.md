# [Appt] Ch 2: Legislation

## Core Idea
Every country has its own accessibility legislation, but most laws ultimately point to the same technical standard: WCAG. Knowing which law applies (by region and by org type) tells you which WCAG level and success criteria are legally required.

## Frameworks Introduced
- **The Legislation Map** — match jurisdiction + entity type to the governing law:
  - **Global — UN Convention on the Rights of Persons with Disabilities (CRPD)**: signed by most countries; promotes/protects/ensures human rights of 1.3B people with disabilities.
  - **Europe — WAD + EAA → EN 301 549**: the **Web Accessibility Directive (WAD)** covers governments; the **European Accessibility Act (EAA)** covers businesses. Both reference **EN 301 549** (which has a software/mobile-app chapter). v3.2.1 maps to **44 success criteria of WCAG 2.1**. Benefits 80M+ Europeans.
  - **United States — Section 508 + ADA**: **Section 508** requires *federal* governments to make mobile apps accessible. The **ADA** covers all other entities (public, private, nonprofit) and demands equal access to goods, services, information, communication. Both refer to WCAG.

## Key Concepts
- **EN 301 549** — the European accessibility standard; includes a chapter specifically on software/mobile apps; defers to WCAG success criteria.
- **WAD vs EAA** — government vs business scope in Europe.
- **Section 508 vs ADA** — federal government vs everyone-else scope in the US.
- **CRPD** — the international human-rights treaty underpinning national laws.

## Mental Models
- **All roads lead to WCAG** — whatever the law, the testable standard is almost always WCAG.
- **Scope = jurisdiction × entity type** — identify both to find your obligation.
- **Civil-rights framing** — these are rights laws, not optional guidelines (cf. [Giving a Damn] bh-ch01).

## Key Takeaways
1. Identify your governing law by region (UN/EU/US) and entity type (gov vs business).
2. In Europe, target the 44 WCAG 2.1 criteria referenced by EN 301 549 v3.2.1.
3. In the US, Section 508 = federal apps; ADA = everyone else.
4. Compliance ultimately means meeting WCAG (typically A + AA).

## Connects To
- **appt-ch03–ch06**: the WCAG criteria these laws enforce.
- **[Giving a Damn] bh-ch01**: ADA/ACA/DDA as civil-rights laws; non-US orgs still at risk if they sell to US customers.
- **[Playbook] esdc-ch01**: the Accessible Canada Act (2019) as the Canadian equivalent.
