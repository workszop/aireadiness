# AI readiness assessment

Self-assessment of an organisation's readiness to adopt AI. Live at https://ready.warsztaty-ai.com/

- 32 questions in 6 areas: strategy and leadership, policies and compliance, data, people and skills, tools and infrastructure, deployment and financing.
- Polish and English (`questions.pl.js`, `questions.en.js`, plain-text question lists wrapped in a template literal). One line per question: `question|best option|...|worst option`, sections start with `#`.
- Scoring: each answer is normalised to 0-1 (top option 1, bottom option 0). Area score is the mean of its questions, overall score is the mean of all questions.
- Results include per-area recommendations, CSV/JSON export and a shareable link that encodes the answers in the URL hash.
- Single `index.html`, no build step. Progress is kept in localStorage. Works when opened directly from disk.
- Styled with the Quantica Lab website design system (`qweb`): Satoshi + Geist Mono, ink-navy hero and panels, quantica pink as the only primary, bento cells, pill buttons. Logos in `assets/`.
