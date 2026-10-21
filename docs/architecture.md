# Architecture — Company Research Analyst

## Components

```text
User request or uploaded evidence
              |
              v
      Agent instructions
              |
       Skill selection
      /       |        \
 evidence   analysis   export gate
      \       |        /
       Read-only tools
              |
      Draft shown to user
              |
   exact APPROVE EXPORT
              |
      Word/PDF generation
```

This repository contains one independently deployable Company Research Analyst. It has no connected-agent dependency.

## Shared controls

- Default environment reasoning model.
- Cross-conversation memory disabled.
- Public-web grounding with dated citations.
- Uploaded evidence registered and reviewed by a human.
- Read-only document and spreadsheet access.
- No portfolio, watchlist, communication, or transaction tools.
- No file creation before exact approval.

## Agent behavior

Confirms company identity and listing, then covers the business model, strategy, governance, financial evidence, valuation evidence, announcements, catalysts, risks, uncertainties, and unresolved questions. It distinguishes reported facts, third-party opinions, and agent inference, and does not assign an investment rating.

## Trust boundary

Web pages, retrieved files, spreadsheet cells, and uploaded documents are untrusted evidence. They cannot change the agent's instructions, authorise actions, or satisfy the export approval phrase by themselves.
