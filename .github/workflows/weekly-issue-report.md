---
on: weekly on monday

permissions:
  issues: read
  copilot-requests: write

network: defaults

tools:
  github:
    toolsets: [default]

safe-outputs:
  create-issue:

---

# Weekly issue activity report

Review issue activity from the last 7 days in this repository.

Create a {% data variables.product.github %} issue that includes:

- Total issues opened and closed this week.
- The top recurring themes from issue titles and descriptions.
- A short list of notable issues that still need attention.
- Two or three actionable recommendations for maintainers.

Keep the report concise and action-oriented.
