# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-05-02

### Added

- Initial launch candidate for `open-source-launch-skill`.
- `SKILL.md` core workflow with a 19-item readiness gate, classification step, and reference map.
- `.cursor/rules/open-source-launch.mdc` and `CURSOR.md` for lightweight Cursor support.
- `AGENTS.md` for Codex-style repo instructions and portable agent usage.
- `skills/open-source-launch/references/positioning.md`, `skills/open-source-launch/references/metadata.md`, `skills/open-source-launch/references/channels.md`, `skills/open-source-launch/references/launch-copy.md`, `skills/open-source-launch/references/failure-modes.md` — full reference set for positioning, public surface, channel selection, channel-specific copy, and failure modes.
- `.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json` for plugin install.
- `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, issue templates, and pull request template.
- `PRIVACY.md` explaining that the skill is Markdown-only and does not collect data.
- `README.md` banner, example output, real `launch-brief-demo` audit, and multi-agent usage guidance for the public launch surface.
- Standard Claude Code plugin skill entrypoint at `skills/open-source-launch/SKILL.md`, with root `SKILL.md` kept as a portable manual entrypoint.
