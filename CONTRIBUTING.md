# Contributing

Thank you for helping `open-source-launch` stay useful and honest.

This repo is different from most open-source projects: there is no app code to compile, no test suite to run, and no build artifact to ship. Contribution means improving the workflow's judgment, breadth, accuracy, or agent-facing packaging.

## What Contribution Looks Like

**Add a readiness check.** If you have seen a launch fail because the skill missed a signal, add it to `skills/open-source-launch/references/failure-modes.md` or to the readiness gate in `SKILL.md`. Bring receipts: the repo, what went wrong, what check would have caught it.

**Add or improve a reference section.** Catch vague guidance, add concrete examples, remove advice that did not survive contact with real launches. Prefer prose with examples over more bullets.

**Report a launch failure mode the skill missed.** Open an issue with: the project, what went wrong, why this skill missed it, what check would catch it next time. The issue is the contribution; a fix can follow.

**Submit a real audit example.** Run this skill on a public repo (your own, with permission, or one that publicly invites feedback). Include the original state, the verdict, and what changed.

## Expectations

**Response time:** issues and PRs get read weekly. This is a side-maintained project, not an on-call service.

**Scope:** keep contributions focused on launch clarity, evidence, and accuracy. Avoid debates about taste, tone, or community philosophy unless they directly affect whether a stranger trusts and tries the project.

**Taste:** the skill optimizes for usefulness, trust, and memory — not stars, not hype, not speed. If your contribution helps a maintainer launch with confidence that strangers will understand and use the project, it belongs here.

## Before You Contribute

Read `SKILL.md` and the relevant reference file. The best contributions understand the operating principle: launch quality is evidence, not confidence.

If you are unsure whether an idea fits, open an issue first instead of a PR.
