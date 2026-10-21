# UK Company Research Analyst — Copilot Studio Sample

MIT-licensed reference agent for evidence-led research on UK-listed companies using Microsoft Copilot Studio's GitHub Copilot harness.

The agent confirms the company and listing, researches attributable public information, separates facts/opinions/inference, and produces a structured investment-committee-style report without assigning an investment rating.

> **POC — Public Information Only. Not investment advice; no suitability assessment or trade execution.**

## Included

- Complete agent definition under `agent/`.
- Four uploadable skills under `skills/`.
- Read-only tool and governance guidance under `docs/`.
- Evaluation cases and acceptance criteria under `evaluations/`.
- Power Platform solution packaging guidance under `solution/`.

## Quick install

1. Create a new Copilot Studio agent using the GitHub Copilot harness.
2. Copy `agent/description.md` and `agent/instructions.md` into the agent.
3. Apply `agent/settings.json` as a configuration checklist.
4. Upload every `skills/*/SKILL.md` file.
5. Configure only the read-only tools described in `docs/tools-and-connections.md`.
6. Keep the agent in Draft, run `evaluations/cases.json`, and verify `evaluations/acceptance-criteria.md`.

See [Installation](docs/installation.md) for the full procedure.

## Safety boundary

The agent does not provide personalised advice, assign a rating, update a watchlist or portfolio, communicate externally, or execute transactions. It generates Word/PDF output only after displaying the complete draft and receiving the exact phrase `APPROVE EXPORT`.

## Licence

Released under the [MIT License](LICENSE). Microsoft services and third-party data remain subject to their own terms and licences.
