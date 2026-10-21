# Installation

## Prerequisites

- Microsoft Copilot Studio access in a non-production environment.
- Permission to create a GitHub Copilot harness agent.
- Copilot Credits for Preview/Evaluate.
- Organisation approval for public-web grounding and uploaded documents.

## Configure the agent

1. Create a new GitHub Copilot harness agent.
2. Use the name `UK Company Research Analyst` or an approved neutral name.
3. Copy `agent/description.md` into Description.
4. Copy `agent/instructions.md` into Instructions.
5. Use the environment-default reasoning model.
6. Disable cross-conversation memory.
7. Enable public-web grounding only when policy permits it.
8. Add the entries from `agent/suggested-prompts.json`.
9. Upload all four `SKILL.md` files under `skills/`.
10. Optionally configure the read-only OneDrive and Excel actions documented in `tools-and-connections.md`.

## Validate

- Confirm company identity/listing is required before research.
- Confirm every material time-sensitive claim requires a source and date.
- Confirm facts, opinions, and inference are labelled separately.
- Confirm no investment rating or personalised advice is produced.
- Confirm export requires a reviewed complete draft followed by exact `APPROVE EXPORT`.
- Run every conversation in `evaluations/cases.json` and record results against the acceptance criteria.

Keep the agent unpublished until organisational security, legal, compliance, privacy, data-licensing, accessibility, and model-risk reviews are complete.
