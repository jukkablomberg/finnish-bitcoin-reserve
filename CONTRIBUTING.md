# Contributing to *Finland's Path to a Sovereign Bitcoin Reserve*

Thank you for considering a contribution. This is an open policy document, and the goal is to make it the most accurate, useful, and forkable artifact possible.

## What we accept

- **Factual corrections** — Wrong dates, broken citations, outdated figures. Open an issue or PR with the source.
- **New data points** — Sovereign reserve moves, new parliamentary filings, central bank statements, ECB releases. Provide a primary source.
- **Counter-arguments** — Serious objections that should be addressed in the *Counter-Arguments and Replies* section. Open an issue with the `counter-argument` label. We'll evaluate, and if the objection is substantive and well-formed, we'll add it with a reply.
- **Translations** — Finnish (priority), Swedish, Norwegian, Estonian, Danish, German. Submit as a new folder (e.g. `sv/`, `no/`) with an accompanying note about the translator's background. We do not accept machine-translated PRs without human review.
- **Forks for other jurisdictions** — You are explicitly welcome to fork this for Sweden, Norway, Estonia, or any country. Please link back to the original.
- **Improvements to the GitHub Actions PDF build** — Better typography, cover-page design, citation formatting.

## What we do not accept

- **Ideological PRs** — This whitepaper takes a policy position: that Finland should establish a sovereign Bitcoin reserve. Pull requests asking the document to argue the opposite will be closed. The right venue for that is a separate document.
- **Promotional content** — No links to exchanges, custody providers, or other commercial services in the body of the whitepaper. Vendors mentioned in custody-architecture examples (e.g. BitGo, Coinbase Custody, Anchorage) are named for illustration, not endorsement.
- **Machine-translated PRs without disclosure** — If you used AI to translate, please say so in the PR description and have a native speaker review.
- **Off-scope tangents** — This document is about Finland's sovereign reserve specifically. PRs that broaden the scope to "all of Europe" or "all crypto" will be redirected to forks.

## How to propose a change

### Small corrections (typos, broken links, factual edits)
Open a pull request directly. If you've never used GitHub before:
1. Click the file you want to edit
2. Click the pencil icon (top-right of the file view)
3. Make your edit
4. Scroll to the bottom and click "Propose changes"

### Larger changes (new sections, restructuring, translations)
Open an issue first describing what you want to do. This avoids you doing significant work that ends up not fitting the document.

### New data
If you add a row to a CSV in `/data/`, please include:
- The primary source (link to a press release, central bank statement, or official filing)
- The date the data point was confirmed
- Your name in the PR description so credit can be given in the `acknowledgements.md` (forthcoming)

## Style

- **Voice**: Operator-credible. Sober. Not promotional, not academic. Write as if briefing a senior civil servant who has no ideological prior on the topic.
- **Length**: Make your point and stop. The full document is targeted at 10-12 pages.
- **Footnotes vs. inline links**: Inline links for primary sources. Footnotes for context or methodology.
- **Numbers**: Always cite the source and date. Bitcoin prices, BTC holdings, and FX figures move fast. Stale numbers undermine credibility.

## Review and merge

The author (Jukka Blomberg) reviews and merges PRs. Response time target: 7 days. If you don't hear back in 14 days, please ping the issue.

## Conduct

See [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md). In short: be useful, be civil, be honest about your interests and affiliations.

## Acknowledgements

Contributors will be acknowledged in a forthcoming `acknowledgements.md` and, for substantial contributions, in the whitepaper itself in a "with thanks to" footnote on the title page.
