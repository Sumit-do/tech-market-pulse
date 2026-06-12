# Tech Market Pulse

A MERN-based dashboard that aggregates real-time tech industry signals — layoffs, hiring trends, funding rounds, emerging technologies, and macroeconomic events — and uses AI to surface "what to prepare for" insights for job seekers and recruiters.

## Why

The tech market moves fast. Layoffs, new AI tools, funding shifts, and global events all ripple into hiring decisions — but the signals are scattered across dozens of sources. This project pulls them into one place and connects the dots.

## Features (planned/in-progress)

- [ ] Automated news aggregation every 6 hours (Hacker News, TechCrunch, layoffs.fyi, ArXiv, etc.)
- [ ] AI-driven categorization and trend extraction
- [ ] Daily "what to prepare for" synthesis
- [ ] Skill growth/decay tracking
- [ ] Layoff-to-hiring migration insights
- [ ] Funding & AI investment heatmap
- [ ] Resume gap analysis (personalized skill recommendations)

## Tech Stack

- **Frontend:** React, Tailwind CSS, Recharts
- **Backend:** Node.js, Express
- **Database:** MongoDB
- **AI:** Claude API (categorization + synthesis)
- **Scheduling:** node-cron

## Project Structure

See [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) for a full breakdown.

## Getting Started

\`\`\`bash
# clone
git clone https://github.com/yourusername/tech-market-pulse.git
cd tech-market-pulse

# server setup
cd server
npm install
cp .env.example .env
npm run dev

# client setup
cd ../client
npm install
npm start
\`\`\`

## Environment Variables

See `.env.example` in `/server`. You'll need:
- `MONGODB_URI`
- `CLAUDE_API_KEY` (or your chosen AI provider)
- `NEWSAPI_KEY` (optional)

## Roadmap

See [docs/ROADMAP.md](docs/ROADMAP.md)

## Contributing

This is an early-stage project. Issues and PRs welcome.

## License

MIT
