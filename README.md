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

## Maintainer Guide

1. Add new items at the top of the news list. Give each one a stable id in the form YYYY-MM-DD-short-name, or YYYY-MM-short-name when only the month is confirmed, and an added_on date in the form YYYY-MM-DD.
2. Use status upcoming for future events and published for coverage that has appeared. A date passing does not show that an event took place. Never relabel an upcoming entry as past automatically. Append a dated follow-up recording completion or a correction only when there is evidence, such as a recording, a published program, or confirmation from the organizer.
3. Publish only facts that have been checked against a primary source, such as an organizer email, a calendar invitation, or the published article. When two sources give different dates, show only the month.
4. Add a url only after the link has been opened and checked. Leave it out otherwise.
5. Describe talks and press coverage as events or mentions. Do not describe them as partnerships, endorsements, or adoption.
6. Changes to this page are additive only. Future updates preserve previous records and add dated follow-ups next to them. Do not edit or remove earlier text.
7. Use plain English and full names. Do not use em dashes or en dashes, and do not use promotional language.

Clarification of the guide above: in item 1, "the top of the news list" means the place that keeps news cards in descending order of event or publication date, counting a month-only date as the first day of that month. Insert a new card above the first existing card with an earlier date, or at the end if none is earlier, and leave existing cards in their current order; dated follow-ups stay next to the card they update. On the page, added_on is the rendered "Added YYYY-MM-DD" text, status is the `news-badge` label, and url is the card's source link. Later checks add their own dated notes beside the October 25, 2026 check notes in the hero status line and at the end of the Research section, and those notes stay unchanged. This creates no exception to the additive-only rule in item 6.
