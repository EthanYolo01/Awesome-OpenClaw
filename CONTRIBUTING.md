# Contributing to Awesome OpenClaw

Thank you for helping make this list better! This document explains how to contribute, what we accept, and what we don't.

## Our Philosophy

**Opinionated over exhaustive.** We'd rather have 500 well-described, genuinely useful entries than 5,000 bare links. Every entry you add should answer three questions: *What is it? Who is it for? Why does it matter here?*

## Ways to Contribute

- **Add a resource** — A skill, tool, article, paper, video, or service you've actually used
- **Improve a description** — Make an existing entry more accurate or useful
- **Fix a broken link** — See a dead URL? Open an issue or submit a fix
- **Flag a security issue** — See a malicious skill listed? Open an issue with the `security` label immediately
- **Report outdated content** — The ecosystem moves fast; flag stale entries

## What We Accept

✅ **Accepted:**
- Skills, plugins, and MCP servers with meaningful adoption or a clear niche
- Tools you have personally used and found genuinely useful
- Articles, tutorials, or videos that teach something not covered elsewhere
- Papers directly relevant to the OpenClaw architecture or security model
- Alternative implementations with a clear differentiating use case

❌ **Not accepted:**
- Your own project submitted the day it was created (exceptions: clear technical novelty)
- AI-generated or SEO-stuffed articles with no original insight
- Paid products without a free tier unless they're genuinely industry-leading
- Duplicate entries (search before submitting)
- Skills not available on ClawHub or a public repo
- Anything that failed the [Skill Vetting Checklist](README.md#skill-vetting-checklist)

## Submission Process

### For Small Changes (Fixing a link, improving a description)

1. Fork the repo
2. Make your edit in `README.md`
3. Submit a PR with a brief description of what you changed and why

### For New Entries

1. Fork the repo
2. Add your entry to the appropriate section in `README.md`
3. Follow the format (see below)
4. Submit a PR using the [Add Resource PR template](.github/PULL_REQUEST_TEMPLATE.md)

### For New Sections

Open an issue first to discuss. New sections require at least 5 quality entries and a clear reason the content doesn't fit existing sections.

## Format Guidelines

### Table Entries (most sections)

```markdown
| [Tool Name](https://link) | What it does in one sentence | When to use it / key differentiator |
```

**Good:**
```markdown
| [ClawRouter](https://github.com/community/clawrouter) | Intelligent LLM routing — sends cheap tasks to cheap models | Users report 40–60% cost reduction; essential for high-volume deployments |
```

**Bad:**
```markdown
| [ClawRouter](https://github.com/community/clawrouter) | LLM router | Good tool |
```

### List Entries (tutorials, articles)

```markdown
- [Title](https://link) — One sentence describing what you'll learn and why it's worth reading
```

## Quality Bar for Each Section

| Section | Minimum Bar |
|---|---|
| Must-Have Skills | 100+ installs on ClawHub; personally tested by contributor |
| Developer Tooling | Open source preferred; clear documentation |
| Security | Extra scrutiny — must not introduce false security confidence |
| Alternatives | Must have a clear stated use case differentiator |
| Tutorials | Must teach something not covered in the official docs |
| Papers | Must be on arXiv or a peer-reviewed venue |

## Security Contributions

Security is our highest-priority section. If you're submitting security content:

- **Malicious skills:** Open an issue with label `security` immediately. Do not include the malicious skill in a PR.
- **CVEs:** Open an issue with label `security`. Provide the CVE number, affected versions, severity, and mitigation.
- **Security tools:** Describe the specific threat model the tool addresses. Vague "security tool" entries are rejected.

## Code of Conduct

All contributors are expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md). Be kind. Focus on the content, not the person.

## Questions?

Open an issue with the `question` label, email the maintainer at **kalayolo86@gmail.com**, or ask in the [OpenClaw Discord](https://discord.gg/openclaw) `#awesome-openclaw` channel.
