# Job Search

An operator-first job search workflow for people who want to run a faster, cleaner, and more sponsor-aware U.S. job search.

This project is built for job seekers and operators who are tired of treating job search like a pile of tabs, ad hoc notes, and repetitive ATS work. It packages a structured workflow for finding leads, screening roles, routing resumes, reusing truthful answers, and tracking blockers. Under the hood, it is implemented as a reusable Codex skill.

## Why This Exists

Most high-volume job searches break down in predictable ways:

- too many low-quality leads
- repeated time wasted on roles that reject sponsorship
- inconsistent resume selection
- custom questions answered from scratch every time
- no stable way to track what was submitted, skipped, or blocked

This repo is designed to make the workflow more operational. It does not try to be a blind-apply bot. It tries to make search decisions more consistent and easier to execute.

## What It Does

- Maintains a candidate profile template for the facts that matter in real application flows
- Applies screening rules before time is spent on weak-fit or sponsor-incompatible roles
- Uses stable resume routing for volume-mode execution
- Reuses truthful answer patterns for common application questions
- Tracks application states with a simple status model
- Preserves handoff points for CAPTCHA, login, uploads, and other user-required steps

## Core Workflow

1. Define the candidate profile and authorization boundaries.
2. Screen roles before applying.
3. Route the right resume for the role family.
4. Reuse answer patterns instead of rewriting everything from scratch.
5. Record each outcome as submitted, skipped, blocked, needs user, or pending.
6. Escalate only the steps that require human judgment or human presence.

## Who It Is For

- Job seekers targeting Data Analyst, Business Analyst, Product-adjacent, or operations-heavy roles
- International candidates and other applicants who need sponsorship-aware screening
- Operators who want to systematize search and application handling instead of improvising every step
- Codex users who want a reusable workflow template they can adapt to their own profile

## Public vs Private

This repository is the public-safe version of the workflow.

It intentionally includes:

- workflow structure
- templates
- screening logic
- routing patterns
- answer-bank patterns
- status definitions

It intentionally does **not** include:

- real candidate contact information
- exact immigration or authorization details for a real person
- private dashboard history
- actual resume files
- sensitive ATS answers

If you want to use this in a real search, keep your live data in a private companion workflow.

## Repository Structure

```text
.
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
└── references/
    ├── public_profile_template.md
    ├── screening_rules.md
    ├── resume_routing_template.md
    ├── answer_bank_template.md
    └── dashboard_status_model.md
```

## Getting Started

1. Clone the repository.
2. Read `SKILL.md` for the operational workflow.
3. Copy the templates in `references/` into a private workspace.
4. Replace placeholders with your own candidate facts, answer strategies, and resume paths.
5. Run your search with explicit rules for sponsorship, role level, geography, and handoff boundaries.

## Principles

- Optimize for truthful, traceable applications.
- Screen before applying.
- Prefer stable routing over constant reinvention.
- Keep human approval where it matters.
- Treat blocked states as data, not noise.

## Limits

This project does not remove the need for judgment. It will not solve CAPTCHA, login, or ambiguous legal wording by magic. Its value is in making the rest of the workflow structured enough that those real bottlenecks become obvious and manageable.
