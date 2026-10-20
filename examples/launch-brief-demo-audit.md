# Real Audit: Launch Brief Demo

This is a real saved audit from running the `open-source-launch` readiness gate against a small runnable local project named `launch-brief-demo`.

## Verdict

Code-ready but account-blocked.

## Code Blockers

- None found in the documented local path.

## Account/Platform Blockers

- GitHub repository metadata is not verified because `launch-brief-demo` is a local project and `example/launch-brief-demo` is not a real public repository.
- Release metadata is not verified because no `v0.1.0` GitHub tag or release exists.
- The documented repository, homepage, and issue URLs in `package.json` use `https://github.com/example/launch-brief-demo...`; those must be replaced before a real public launch.

## Launch Blockers

- No CI workflow exists under `.github/workflows/`, so automated validation is local-only.
- Launch channel plan and channel-specific copy are not documented yet.
- Security and conduct contact uses `security@example.com`, which is fine for a local demo but would block a real launch.

## What Is Already Working

- README has a plain human hook: small projects need audience, proof, and boring launch details checked before sharing.
- First-run path is visible and copy-pasteable: `node ./bin/launch-brief.js`.
- Proof is immediate: README includes real example output, and the observed command output matches it.
- Project metadata exists in `package.json`: name, version, description, license, author, repository, homepage, bugs, keywords, bin, scripts, and engines.
- Community basics exist: `LICENSE`, `CHANGELOG.md`, `CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`, issue template, and pull request template.

## Gate Evidence

| Check | Verdict | Evidence |
|-------|---------|----------|
| Positioning | Pass | README opens with "Print a tiny launch brief before you share a small open-source repo." |
| Audience and CTA | Pass | README says it is for "maintainers who want a quick reminder of those launch basics." |
| First-run path documented | Pass | README documents `node ./bin/launch-brief.js`. |
| First-run path tested | Pass | Manual QA command passed: `node ./bin/launch-brief.js`. |
| README itself | Pass | README includes quick start, example output, checks, validation, limitations, security, contributing, code of conduct, and license. |
| Examples / demo / proof | Pass | README example output matched the observed CLI output. |
| Project metadata | Pass | `package.json` parsed successfully and includes core npm-style metadata. |
| Repo metadata | Not verified | Local project only; GitHub description, topics, website, and social preview cannot be checked. |
| Release metadata | Not verified | `CHANGELOG.md` has `0.1.0`, but no GitHub tag or release exists. |
| Update / removal path | Not applicable | The demo CLI does not install persistent project state in the documented path. |
| Automated checks | Partial | `npm test` passes locally, but no CI workflow exists. |
| Manual QA | Pass | `node ./bin/launch-brief.js` and `npm test` both passed. |
| No secrets / private paths | Pass | Public files contain no real tokens, passwords, or local absolute paths. |
| No stale or placeholder content | Needs work | `example/launch-brief-demo` URLs and `security@example.com` are demo placeholders and must be replaced before a real public launch. |
| Launch copy is channel-specific | Needs work | No Show HN, Reddit, Product Hunt, social, or maintainer outreach copy exists yet. |
| Community-health files | Pass | LICENSE, CHANGELOG, CONTRIBUTING, SECURITY, CODE_OF_CONDUCT, issue template, and PR template exist. |
| Release dry-run | Not applicable | No package publication was requested for this local demo. |
| Channel plan | Needs work | No channel selection rationale is documented. |
| Post-launch response plan | Needs work | CONTRIBUTING gives PR expectations, but no launch-day issue/comment triage plan exists. |

## Manual QA Transcript

```text
$ node ./bin/launch-brief.js
Launch Brief
Audience: solo maintainers preparing a small open-source repo
Promise: summarize the launch surface before posting
Proof: this command runs without dependencies
Next: verify repo metadata, release tag, and channel copy

$ npm test
> launch-brief-demo@0.1.0 test
> node ./bin/launch-brief.js

Launch Brief
Audience: solo maintainers preparing a small open-source repo
Promise: summarize the launch surface before posting
Proof: this command runs without dependencies
Next: verify repo metadata, release tag, and channel copy
```

## Next Action

If this were a real launch, replace placeholder GitHub/contact URLs, create the public repository, add a small CI workflow, create the `v0.1.0` tag/release, write channel-specific launch copy, then rerun the gate.
