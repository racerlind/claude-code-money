# CLAUDE.md

<!-- Put this file in the root of a client project. Claude Code reads it at the start of every session.
     Replace everything in <angle brackets>, delete what you don't need. -->

## Project
- Client: <business name>
- What it does: <one sentence, e.g. "booking site for a dental clinic">
- Stack: <e.g. Next.js, Postgres, Vercel>

## Goal of the current job
<One sentence a client would sign off on, e.g. "Every website lead lands in the CRM and gets a text reply in under 5 minutes.">

## Rules
- Plan first. Show me the plan and the files you'll touch before editing anything.
- Never touch live customer data, production databases or billing without asking me first.
- Secrets live in `.env`. Never write keys, passwords or tokens in code, logs or commit messages.
- Small changes. One feature or fix per commit, with a clear message.
- Every change comes with a test, or a written reason why it can't have one.
- Add one line per change to `CHANGELOG.md` in plain English the client can read.
- Don't add new dependencies without telling me why.
- If something is unclear, ask. Don't guess business rules.

## Commands
- Install: `<npm install>`
- Run locally: `<npm run dev>`
- Tests: `<npm test>`
- Lint: `<npm run lint>`

## Done when
- [ ] <measurable result 1, e.g. "10 test leads flow end to end">
- [ ] <measurable result 2, e.g. "the owner gets a weekly email report">
- [ ] All tests pass and I've run it myself on localhost
- [ ] `CHANGELOG.md` is updated
