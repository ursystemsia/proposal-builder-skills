# Proposal Builder Skills

Two portable agent skills for freelancers who use Upwork or Workana:

- `freelancer-onboarding`: builds a verified, reusable freelancer profile from experience, skills, portfolio evidence, preferences, and constraints.
- `proposal-builder`: evaluates an opportunity and drafts a tailored proposal without inventing credentials or ignoring platform risks.

The skills work together but can be installed separately. They do not require a specific browser, connector, CLI, or model.

## Install

Copy each skill folder into the skill directory supported by your agent.

### Claude Code, project installation

```text
your-project/
└── .claude/
    └── skills/
        ├── freelancer-onboarding/
        └── proposal-builder/
```

### Codex, project installation

Use the project skill directory configured for your environment. In projects that discover `.agents/skills/`:

```text
your-project/
└── .agents/
    └── skills/
        ├── freelancer-onboarding/
        └── proposal-builder/
```

Copy the complete folder, including its `references/` directory.

## First use

Start with onboarding:

```text
Use freelancer-onboarding to create my verified freelancer profile for Upwork and Workana.
```

Review the generated `freelancer-profile.md`. Then provide that profile and a job post:

```text
Use proposal-builder with freelancer-profile.md to evaluate this Upwork opportunity and draft the proposal.
```

The agent should return a verdict, evidence map, draft when appropriate, questions, assumptions, and a platform check. It must not submit the application or contact the client.

## Optional tools

The user may provide profile text, files, portfolio samples, or URLs. The skills may use an already available and authorized browser, connector, or CLI to inspect them. If access fails, the agent must ask for the relevant content or state the limitation. No tool is required for basic use.

## Privacy and platform safety

- Keep private client information out of reusable profiles and public examples.
- Do not store passwords, tokens, cookies, payment details, or identity documents.
- Verify ownership before using portfolio work.
- Review the exact proposal before submission.
- Recheck current Upwork or Workana rules when a proposal depends on contact sharing, links, payments, tests, or access.
- These skills draft and review. They do not submit proposals, buy Connects, send messages, create accounts, or accept contracts.

## Repository layout

```text
proposal-builder-skills/
├── freelancer-onboarding/
│   ├── SKILL.md
│   └── references/profile-schema.md
├── proposal-builder/
│   ├── SKILL.md
│   └── references/
├── examples/
├── LICENSE
└── README.md
```

## License

MIT. See [LICENSE](LICENSE).

