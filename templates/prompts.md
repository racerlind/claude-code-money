# Prompts for Claude Code

Copy-paste prompts for the routes in the README. Start Claude Code in the project folder, switch to Plan Mode with Shift+Tab for the first message, and fill in everything in `<angle brackets>`.

---

## Client ticket (freelance builds)

```text
Read CLAUDE.md, the codebase and this ticket:

<paste the client's task here>

1. List every file this touches and why.
2. Propose a step-by-step plan. Don't edit anything until I approve.
3. After I approve: make the change in small steps, run the tests after each one.
4. Done = tests pass and I can see it working on localhost.
5. Finish with a short summary I can send to the client: what changed, how to check it.
```

## Scope a new job before you quote

```text
Here is a job post from a client:

<paste the job post>

Read it like a senior developer. Tell me:
- what they actually need (the real problem behind the request)
- what's unclear and which 3 questions I should ask before quoting
- the work broken into tasks, with a rough time for each
- the risks that could make this take twice as long
Don't write any code.
```

## Automation for a business (retainers)

```text
Read CLAUDE.md. I'm building an automation for <business type>:
<describe the workflow, e.g. "new website form leads → CRM → SMS reply">

1. Propose the simplest setup that works and costs little to run each month.
2. List every outside service and API key it needs, and where each key will live (.env only).
3. Build it with a dry-run mode first, so nothing real is sent while we test.
4. Write a one-page README the business owner can follow if something breaks.
```

## MVP (micro-SaaS)

```text
I'm building a small paid tool for <who> that solves <one problem>.

Build an MVP with:
- sign-in
- the one core feature: <describe it>
- a Stripe subscription with a free trial
- usage limits for free vs. paid users

Write tests first. Show me the plan and the folder structure before you write code.
Keep it simple: no features beyond this list.
```

## Landing page + waitlist (validate before you build)

```text
Make a one-page landing site for <product idea> aimed at <who>.
- headline that names the problem, one line on how it's solved
- 3 short benefit blocks
- an email waitlist form that saves to <service or a simple database>
- fast, mobile-first, no stock-photo clichés
Then tell me how to deploy it for free.
```

## Review before you deliver

```text
Review all changes on this branch as a strict senior reviewer:
- bugs and edge cases
- security problems (secrets, input validation, auth)
- anything that touches data it shouldn't
- code I'd be embarrassed to show the client
List problems by severity. Don't fix anything yet.
```

## Turn repeat work into a product (templates and skills)

```text
Look at the last <3> client projects in <folders>.
Find the parts I keep rebuilding every time.
Propose a reusable starter kit: folder structure, what's configurable,
and a README a buyer could follow in 10 minutes.
```
