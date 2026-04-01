Your task is to create this week's AI agent research deliverables and save them into this repository.

Read `AGENTS.md` first and follow it.

## Objective
Research important new information from the past 7 days about AI agents in general.
Codex is only one supporting tool in scope, not the sole subject.

## Sources
Research broadly across public sources when available and useful, including:
- official docs
- official changelogs and release notes
- official blogs and announcements
- research papers
- repositories
- developer forums
- credible news coverage
- social platforms such as X when they add useful signal

Prefer primary sources for factual claims.

## Deliverables
Determine today's date in Asia/Tokyo and create a dated directory:
- `reports/YYYY/YYYY-MM-DD/`

Write these files:
1. `reports/YYYY/YYYY-MM-DD/summary.md`
2. `reports/YYYY/YYYY-MM-DD/signals.json`
3. `reports/latest/summary.md`
4. `reports/latest/signals.json`
5. update `reports/index.md`

## Requirements for summary.md
Write in Japanese.
Include these sections:
- タイトル
- 作成日
- 概要
- 今週の重要トピック
- 学習への示唆
- 業務効率化への示唆
- 開発・PoCへの示唆
- 来週試すこと
- 参考ソース

For each major topic, include:
- 何が新しいか
- なぜ重要か
- 学習面の価値
- 業務効率化への示唆
- 開発/PoCへの示唆
- 信頼度

Limit the report to the highest-signal items.

## Requirements for signals.json
Create a JSON array. Each item must use this schema:
{
  "title": "",
  "date": "YYYY-MM-DD",
  "source_type": "official|technical|news|social|paper",
  "theme": [],
  "summary": "",
  "learning_relevance": 1,
  "productivity_relevance": 1,
  "development_relevance": 1,
  "novelty": 1,
  "urgency": 1,
  "recommended_action": "",
  "confidence": "high|medium|low",
  "sources": []
}

## Requirements for reports/index.md
Append or refresh a compact chronological index with links to each dated report folder.
Keep newest first.

## Important
- Save the files directly into the repository.
- Keep formatting clean and readable.
- Do not leave placeholders.
- If an older index exists, update it rather than duplicating lines.
