# README And Positioning Reference

Use this reference when the launch depends on README quality, positioning, proof, examples, or the first 10 seconds of a repo visit.

## Positioning First

Before editing docs, write the launch positioning in plain language:

```text
Project:
Audience:
Pain:
Promise:
Fastest demo:
Why now:
Why this is different:
Proof:
Primary CTA:
```

The promise should fit this pattern:

```text
This helps <specific audience> <achieve specific outcome> without <specific pain/tradeoff>.
```

Good positioning is concrete:

- Bad: "A powerful AI tool for developers."
- Better: "A repo launch assistant that audits your public surface and produces a channel-specific launch checklist before you publish."

If the project is simple, do not inflate it. A small project can still launch well when the audience, use case, proof, and first-run path are obvious.

## README Structure

Write the README like a conversion page, not a landing page.

Recommended order:

1. Name and one-sentence promise.
2. Useful badges only: release/version, CI, license, or status.
3. Screenshot, GIF, terminal output, demo link, or example output above the fold.
4. One-command or one-link first-run path.
5. What it does and who it is for.
6. Quickstart that works from a clean environment.
7. Examples, demo, or before/after.
8. Usage, CLI, API, configuration, or integration reference.
9. Update, uninstall, migration, or rollback instructions when relevant.
10. Validation/testing instructions.
11. Security note.
12. Contributing and license.

Above the fold, the user should know:

- what it is
- who it is for
- why it matters
- how to try it
- what proof exists

## Narrative Pattern

Use a human problem-to-relief story:

```text
You have <project state>. The project works, but <launch risk>.

This helps you <specific launch outcome> before <public moment>.
```

Use direct voice. Skip hype words ("revolutionary," "ultimate," "next-gen") and vague labels ("AI-powered") unless the AI is the point.

## Proof Assets

Good proof includes:

- screenshot or GIF
- hosted demo
- demo repo
- real generated output
- terminal output from install and validation
- before/after comparison
- short video walkthrough
- example project with commits, tests, and docs

Do not fake proof. If a demo is synthetic, say it is a demo. If a report comes from real git history, say so.

Honest, short limitations paired with next steps build trust.

## README Failure Checks

Flag the README when:

- the audience is unclear
- the first command or link is buried
- the proof is missing or vague
- the copy describes features but not the user problem
- the README says "coming soon," "screenshots later," or "not published yet"
- badges, slogans, or installation details appear before the promise
- examples depend on local absolute paths or hidden private context
