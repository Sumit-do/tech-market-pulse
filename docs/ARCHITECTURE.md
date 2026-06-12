# Architecture

## Data Flow

1. **Fetch Layer** (`server/services/fetchers/`) — runs every 6 hours via cron, pulls raw articles from sources, dumps into `raw_articles` collection.
2. **Analysis Layer** (`server/services/ai/`) — processes unprocessed articles, extracts categories/skills/companies/sentiment.
3. **Aggregation Layer** (`server/services/aggregator.js`) — computes trend deltas, correlations, daily synthesis.
4. **API Layer** (`server/routes/`, `server/controllers/`) — exposes processed insights to frontend.
5. **Frontend** (`client/src/`) — dashboard visualizations.

## Collections

- `raw_articles` — unprocessed news
- `insights` — AI-processed daily summaries
- `users` — (future) for personalization

## Notes

This structure is intentionally loose at the early stage — file/folder names may change as features solidify.
