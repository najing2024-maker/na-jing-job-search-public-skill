---
name: na-jing-job-search-public
description: Use when running a public-safe U.S. job search workflow for Data Analyst, Business Analyst, and adjacent Product or operations roles, especially when screening for sponsorship conflicts, routing resumes consistently, reusing truthful answer patterns, and tracking applications without exposing private candidate data.
---

# Na Jing Job Search Public

## Overview

Use this skill as a public-safe template for a U.S. job search system focused on analytics and business roles. It preserves the operating workflow, screening heuristics, answer patterns, and tracking structure while removing candidate-specific private information.

## Workflow

1. Read `references/public_profile_template.md` before storing or requesting candidate facts.
2. Read `references/screening_rules.md` before searching or deciding whether to apply.
3. Read `references/resume_routing_template.md` before selecting a resume or stable route.
4. Read `references/answer_bank_template.md` before drafting or reusing custom answers.
5. Read `references/dashboard_status_model.md` before updating counts or classifying outcomes.

## Safe Operating Rules

- Prioritize Data Analyst and Business Analyst roles first. Treat Product roles as secondary unless they overlap heavily with analytics or operations.
- Skip roles that explicitly reject sponsorship, require unrestricted U.S. work authorization, require citizenship or clearance, or are clearly senior, staff, or management level.
- Use stable resume routing by role family. In volume mode, prefer one default resume per target lane.
- Count a role as submitted only after an explicit confirmation state is observed.
- Record every touched role as `Submitted`, `Skipped`, `Blocked`, `Needs user`, or `Pending`.

## Privacy Boundary

- Do not include real email addresses, phone numbers, street addresses, immigration documents, or resume binaries in the public version.
- Replace candidate-specific text with templates or placeholders.
- Keep real answer banks, exact compensation expectations, and live dashboard rows in a private companion workflow instead of this public skill.

## References

- `references/public_profile_template.md`: candidate profile placeholder fields and storage guidance.
- `references/screening_rules.md`: reusable role-screening rules for U.S. analytics and BA searches.
- `references/resume_routing_template.md`: stable routing pattern for volume-mode resume selection.
- `references/answer_bank_template.md`: truthful reusable answer patterns with placeholders.
- `references/dashboard_status_model.md`: status definitions, count rules, and blocker categories.
