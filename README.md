# Auditable Agents Ecosystem

Source for <https://auditable-agents.github.io>, the front door for an open-source ecosystem
that makes the actions of AI agents accountable.

## What the Ecosystem Covers

The components span the lifecycle of a single agent action:

| Stage | Component | Role |
|---|---|---|
| Before deployment | [agent-audit](https://github.com/HeadyZhang/agent-audit) | Static scanning of agent code and MCP configurations against the OWASP Agentic Top 10 |
| At execution | [Aegis](https://github.com/Justin0504/Aegis) | Policy enforcement before a tool call commits, with signed, hash-chained records |
| After the commit | [auditable](https://github.com/yzhao062/auditable) | Capture, replay, and rollback of a committed action |
| Across the field | [awesome-auditable-ai](https://github.com/yzhao062/awesome-auditable-ai) | Curated index of papers, tools, datasets, and standards |

The [Auditable Agents](https://arxiv.org/abs/2604.05485) framework supplies the shared model:
five auditability dimensions, the detect / enforce / recover classes, and the Auditability
Card disclosure format.

## Current State

Stated plainly, because tooling meant to make other systems inspectable should be inspectable
itself: every repository is effectively maintained by one developer, the components carry four
different licenses, and there is no shared release process or published governance model yet.
Building the contributor base and the governance layer is what this organization exists to do.

## Contributing

Issues and pull requests go to the individual component repositories. For a security problem,
use the repository's private security advisory rather than a public issue.

## Editing This Page

The site is a single self-contained `index.html` with no build step and no external
dependencies. Edit it and push to `main`; GitHub Pages serves it directly.

## License

Page content is CC0-1.0. Each component keeps its own license as listed above.
