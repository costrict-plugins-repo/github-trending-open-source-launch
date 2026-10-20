# Security

This is a portable launch-readiness workflow packaged as Markdown guidance plus lightweight agent metadata. The attack surface is small but real.

## Reporting

Email **hello@omar-khaled.com** instead of opening a public issue.

I commit to acknowledging within 7 days on a best-effort basis. This is a side-maintained project, not a 24/7 service. Allow time for assessment and a fix before public disclosure.

## What Counts as Security for This Skill

- **Prompt injection in reference files** — content that hijacks the skill's behavior, misleads the assistant, or causes it to recommend unsafe actions.
- **Misleading audit guidance** — advice that would cause a launch to fail or expose a maintainer (e.g. recommending a deprecated channel, suggesting a posting pattern that violates a community's rules, or telling users to omit a security disclosure path).
- **Rendering issues that hide content** — markdown that fails to display in such a way that an important warning becomes invisible.

## What Is Not Security

Feature requests, typos, clarifications, and improvements belong in issues or pull requests, not security reports.

## Disclosure Timeline

1. **You report** → I acknowledge within 7 days.
2. **Assessment** → I verify and scope the issue.
3. **Fix** → I prepare and ship a patch.
4. **Patch** → I credit you publicly if you'd like.

I will not sit on a confirmed issue. If a fix takes time, I will say so and add a warning to the README.
