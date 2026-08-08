# Dashboard Status Model

## Allowed Statuses

- `Submitted`: explicit confirmation was observed.
- `Skipped`: role violated rules or was not worth pursuing.
- `Blocked`: agent could not proceed safely due to technical or policy friction.
- `Needs user`: the user must act before progress can continue.
- `Pending`: role remains viable for later action.

## Count Rules

- Count only confirmed submissions.
- Do not count saved jobs, application drafts, or “apply started” states as submitted.
- Keep totals aligned between job pool rows and dashboard rollups.

## Common Blockers

- CAPTCHA
- Resume upload control failure
- Workday or enterprise ATS account gate
- Broken or removed job posting
- Sponsorship wording conflict
- Custom materials not yet prepared
