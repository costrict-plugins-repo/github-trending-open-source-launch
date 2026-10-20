# Cursor Support

This repo includes a Cursor project rule for the same launch-readiness workflow as the canonical skill.

## Use In This Repo

Open this repository in Cursor. The rule is available at:

```text
.cursor/rules/open-source-launch.mdc
```

Ask Cursor to use the open-source-launch rule when auditing or improving a repo launch surface.

## Use In Another Repo

Copy the rule into the target project:

```text
<your-project>/.cursor/rules/open-source-launch.mdc
```

Then ask Cursor:

```text
Use the open-source-launch rule to audit this repo for GitHub launch readiness. Check the README, first-run path, proof/demo, metadata, security surface, launch channels, launch copy, and follow-up plan.
```

## Relationship To Other Agent Surfaces

Cursor supports project rules and native skills. The included `.cursor/rules/open-source-launch.mdc` keeps setup lightweight, while [`skills/open-source-launch/`](./skills/open-source-launch/) is the full reusable workflow and can be copied or referenced as a Cursor skill if you prefer `.cursor/skills/`.

Cursor does not install Claude Code plugins from `.claude-plugin/`. The Cursor rule is a lightweight mirror of the core workflow for Cursor users.

Codex-style agents can use [`AGENTS.md`](./AGENTS.md). Other agents can load [`SKILL.md`](./SKILL.md) directly when they support long-form instruction files.

For the full Claude Code plugin path, use the install commands in [`README.md`](./README.md).
