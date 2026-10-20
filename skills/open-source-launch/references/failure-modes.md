# Failure Modes And Verdict Reference

Use this reference when producing the final readiness report, reviewing a launch plan, or checking whether the project is accidentally repeating common launch mistakes.

## Full Verdict Format

Items without evidence default to `Not verified`, not `Pass`. An unverified check is a gap to investigate, not a hidden pass.

| Check | Verdict | Evidence |
|-------|---------|----------|
| Positioning | Pass / Needs work / Not verified | Quote from README hero or landing page |
| Audience and CTA | Pass / Needs work / Not verified | Quoted line naming the persona and outcome |
| First-run path documented | Pass / Needs work / Not verified | One-command or one-link path quoted from README |
| First-run path tested | Pass / Fail / Not verified | Command run end-to-end in a clean environment with output captured |
| README itself | Pass / Needs work / Not verified | File check: hero, install, proof, license/contributing/security pointers all present |
| Examples / demo / proof | Pass / Needs work / Not verified | Runnable example + observed output, OR linked screenshot/GIF |
| Project metadata | Pass / Needs work / Not applicable | Manifest fields verified (name, version, license, description, keywords) |
| Repo metadata | Pass / Needs work / Not applicable | GitHub description, topics, linked site, social preview confirmed |
| Release metadata | Pass / Needs work / Not applicable | Tag, release notes, version match across files |
| Distribution status | Pass / Needs work / Not verified | Install path is live, or pending/private status is explicit with fallback |
| Update / removal path | Pass / Needs work / Not applicable | Quoted section in docs covering upgrade, uninstall, or migration |
| Automated checks | Pass / Fail / Not applicable | CI run URL or local command output |
| Manual QA | Pass / Fail / Not applicable | Smoke-test transcript or QA notes |
| No secrets / private paths | Pass / Needs work | Grep result for tokens, keys, local paths — none found |
| No stale or placeholder content | Pass / Needs work | Grep result for TODO/FIXME/coming soon/lorem — none found |
| Launch copy is channel-specific | Pass / Needs work | One sentence quoted from each channel showing differentiation |
| Community-health files | Pass / Needs work / Not applicable | LICENSE / CHANGELOG / CONTRIBUTING / SECURITY presence, plus funding/sponsorship when relevant |
| Release dry-run | Pass / Fail / Not applicable | Output of npm publish --dry-run / python -m build / cargo publish --dry-run / gh release create --draft |
| Channel plan | Pass / Needs work | Channel selection rationale documented |
| Post-launch response plan | Pass / Needs work | Documented SLA, triage path, or rollback steps |

```text
Verdict: Ready / Not Ready / Code-ready but account-blocked

Code blockers:
- ...

Account/platform blockers:
- ...

Launch blockers:
- ...

Next action:
- ...
```

Never hide uncertainty. If a check was not run, mark `Not verified` and explain why.

## Common Failure Modes

Watch for:

- README does not explain who the project is for
- README documents a command, link, import, or demo path that does not work
- release artifact omits required executables, docs, templates, examples, assets, or data
- public artifact includes private launch notes
- package, archive, container, app, model, dataset, or docs output differs from working tree expectations
- first run works once but update, migration, redeploy, or refresh overwrites user edits
- tests pass but the documented user path fails
- GitHub badges point to a repo that does not exist yet
- README presents marketplace, registry, package, or app-store install commands as live while approval or publishing is still pending
- demo uses local absolute paths
- a similar project could confuse users searching for yours
- launch copy says "coming soon," "not published yet," or "screenshots later"
- launch posts use the same generic text in every community
- launch asks for stars instead of feedback or usage
- maintainer disappears after posting
- early feedback is not converted into docs or issues

## Source-Informed Standards

This gate is intentionally focused on first-time-stranger clarity, trust, and time-to-value. It complements — rather than replaces — broader OSS standards like opensource.guide (community/governance), GitHub Community Standards (file presence), and OpenSSF Scorecard (supply-chain security). If your project needs those layers, run them in addition to this gate.

Use these public standards as references when useful:

- GitHub README docs and repository best practices: `https://docs.github.com/en/repositories`
- Open Source Guides for starting projects, finding users, building community, and measuring health: `https://opensource.guide/`
- OpenSSF Best Practices for security and trust basics: `https://best.openssf.org/`
- Hacker News Show HN and community guidelines: `https://news.ycombinator.com/showhn.html` and `https://news.ycombinator.com/newsguidelines.html`
- Product Hunt launch guidance for launch assets, timing, and launch-day response: `https://www.producthunt.com/launch`

Quote only benchmarks you verified directly in this session.

## Final Quality Bar

Optimize for trust, clarity, usefulness, and memory — not just shipping.

A strong open-source launch makes a stranger think:

1. I understand what this does.
2. I know whether it is for me.
3. I can try it immediately.
4. The maintainer checked the boring details.
5. The demo is real enough to trust.
6. I know how to update, remove, contribute, or report a problem.
7. I would star this because I may need it later or want others to find it.

That is the bar.
