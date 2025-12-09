# webflow-kingdom
Gamified social network for webflow professionals

**Webflow Kingdom** is a gamified social network and marketplace for Webflow professionals. It connects **pre-vetted teams** of complementary skills (designers, Webflow developers, marketing specialists, growth engineers) with high-value projects and retainers, prioritizing **smart team–project matching** and **Web3-powered Solana transactions** from day one.

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Market Opportunity](#market-opportunity)
- [Customers](#customers)
- [Core Features](#core-features)
- [Team Building](#team-building)
- [Team Trading](#team-trading)
- [Getting Started](#getting-started)
- [Tech Stack](#tech-stack)
- [Development Plan](#development-plan)
- [Demo](#demo)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About the Project

**The Problem**: Complex Webflow projects and ongoing retainers frequently **overrun budgets and miss deadlines** because clients assume one person can “do everything,” while the work actually requires a coordinated group of specialists. Misaligned expectations, ad‑hoc communication, and fragile payment flows lead to scope creep, stalled projects, and eroded trust on both sides.

**Webflow Kingdom Solution**: Start with **matching and money**. Project briefs are structured and scored, then matched to **pre‑vetted teams** whose skills, history, and cohesion fit the work. Engagements are locked in through **on‑chain Solana transactions** (escrow, milestones, payouts) and **Web3‑verified deliverables**, so expectations, ownership, and payment terms are clear from the outset. Around this, Kingdom layers gamified progression, team‑building tools, and an algorithmic cohesion and team‑trading system.

## 🎯 Customers

| Customer Type | Needs | Kingdom Value |
|---------------|-------|---------------|
| Growth‑stage startups | Reliable Webflow + marketing execution on retainers | Curated squads matched to briefs + on‑chain escrow |
| Mid‑market SaaS | Complex Webflow apps, CRO, experiments | Specialist teams with proven history |
| E‑commerce & DTC | High‑converting storefronts and landing pages | Design/dev/marketing teams tied to performance milestones |
| Marketing agencies | Webflow capacity without full‑time hires | White‑label teams + simple Solana-powered payouts |
| Webflow agencies | Overflow and specialist gaps | Augmentation squads with verified track records |

## 📊 Market Opportunity

| Reality today | Webflow Kingdom offers |
|--------------|------------------------|
| Generic freelancer marketplaces | Niche focus: Webflow ecosystems and adjacent growth work |
| Manual, guess‑based matching | Structured briefs + team scoring + matching logic |
| Fragile off‑platform payments | On‑chain Solana escrow, milestones, and payouts |
| No verified team history | Web3‑anchored deliverable and review records |
| Static, misaligned teams | Cohesion scoring + optional team trading over time |

## ✨ Core Features

### Project–Team Matching (First‑class)

- **Structured project briefs**: Budget, timeline, vertical, Webflow complexity, integrations, marketing goals.
- **Team capability profiles**: Skills, past niches, tech depth, price bands, preferred engagement models.
- **Matching engine**:
  - Scores fit between projects and teams.
  - Surfaces 3–5 best‑fit teams instead of a raw marketplace list.
  - Considers cohesion and past performance, not just individual skills.
- **Pre‑engagement lobby**:
  - Shortlisted teams can ask clarifying questions.
  - Clients can compare offers with standardized terms.

### Web3 Transactions (From Day 1)

- **Solana escrow**:
  - Client funds milestones into a Solana program-controlled escrow.
  - Funds only release when deliverables are verified.
- **Milestone payments**:
  - Each milestone has an on‑chain reference and amount.
  - Partial payouts possible if scope evolves but both sides agree.
- **Web3‑verified deliverables**:
  - Hashes of key artifacts (Figma exports, Webflow cloneable IDs, docs) stored on-chain or anchored.
  - Review events (approved/rejected) signed and associated with both client and team.
- **Reputation layer**:
  - Teams build an immutable record of completed work and resolution history.
  - Clients also accumulate a reputation score for clarity, fairness, and timely approvals.

## 👑 Team Kingdom (Social + Marketplace)

- **Team profiles**: “Level 7 Webflow Squad” with clear role breakdown (design, dev, growth, ops).
- **Gamification**: XP for completed milestones, badges for categories (SaaS, e‑com, launches, migrations).
- **Portfolio showcases**: Link to live Webflow builds plus on‑chain verification of who delivered what.
- **Kingdom feed**: New briefs, matched opportunities, milestone wins, and notable launches.

## 👥 Team Building

### Online Cohesion Exercises

- **Forge Bonds**: Regular, anonymous feedback rounds on communication, reliability, strategy, collaboration.
- **Skill Sync**: Lightweight exercises to clarify who owns which part of the stack and where each member is strongest.
- **Kingdom Calls**: Live video working sessions for deep dives on architecture, timelines, and scope.
- **Chemistry Score**: Aggregated cohesion metric that factors into team–project matching.

### Networking Hub – Building Moats

- **Building Moats spaces**: Topic or skill‑based rooms (e.g., “SaaS dashboards”, “CMS monsters”, “animations”).
- **Virtual meetups**: Group sessions, teardown nights, and brief reviews.
- **Local chapters**: Optional in‑person meetups coordinated per city or region.
- **Mentorship ladder**: Senior squads helping newer teams reach enterprise‑level delivery.

## 🔄 Team Trading System

- **Private feedback engine**:
  - Teammates rate each other across several dimensions after projects.
  - Data stays private to the algorithm; only aggregate signals surface.
- **Cohesion‑aware trading**:
  - When fit repeatedly scores low, the system can suggest alternative teams.
  - Freelancers can opt in to a “transfer window” where they join squads with better chemistry.
- **Safeguarded transitions**:
  - In‑flight project transitions must respect escrow and milestones.
  - On‑chain history keeps movement transparent while preserving reputation.

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- npm, pnpm, or yarn
- Supabase project
- Solana wallet (e.g., Phantom) for test transactions

### Installation

git clone https://github.com/YOUR_USERNAME/webflow-kingdom.git
cd webflow-kingdom
npm install
cp .env.example .env.local
npm run dev

text

### Environment Variables

NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SOLANA_RPC_URL=https://api.mainnet-beta.solana.com
SOLANA_PROGRAM_ID=your_solana_program_id
OPENAI_API_KEY=your_openai_key # if using AI-assisted matching/copy

text

## 🛠️ Tech Stack

| Layer        | Technology             | Purpose                                  |
|-------------|------------------------|------------------------------------------|
| Frontend    | Next.js + React + TS   | App shell, profiles, matching UI         |
| Styling     | Tailwind + shadcn/ui   | Kingdom-themed interface                 |
| Backend     | Next.js API + Supabase | Auth, data models, matching logic        |
| Web3        | Solana + @solana/web3.js + Anchor | Escrow, milestones, reputation   |
| Video       | Daily.co               | Kingdom Calls team sessions              |
| Realtime    | Supabase Realtime      | Chats, notifications, live lobbies       |
| Analysis    | Custom scoring + LLMs  | Fit scoring, recommendations             |
| Database    | Supabase Postgres      | Users, teams, projects, feedback         |
| Hosting     | Vercel                 | Deployment and edge functions            |

## 🗺️ Development Plan

**Phase 1 – Matching & Web3 Core (highest priority)**  
- Implement project brief model and team capability profiles.  
- Build first version of the matching engine (rule‑based + scoring).  
- Implement Solana escrow program, basic milestone contract, and client–team funding flow.  
- Minimal UI for: create brief → get matched teams → accept → escrow funded.

**Phase 2 – Team Profiles & Reputation**  
- Team and user profile pages with role breakdowns and histories.  
- Integrate Web3‑verified deliverable hashes and milestone approval events.  
- Basic reputation scores for teams and clients surfaced in matching.

**Phase 3 – Team Building & Cohesion**  
- Launch Forge Bonds, Skill Sync, Chemistry Score.  
- Add Kingdom Calls and Building Moats spaces.  
- Begin feeding cohesion metrics back into the matching engine.

**Phase 4 – Team Trading & Advanced Matching**  
- Implement transfer window, trade suggestions, and secure transitions.  
- Enhance scoring model with more history and feedback dimensions.  
- Add filters and controls for clients who prefer new teams vs. veteran squads.

**Phase 5 – Gamification & Tournaments**  
- Leaderboards, badges, and quests.  
- “Tournament briefs” where multiple teams compete on structured challenges.  
- Deeper analytics dashboards for teams to see where they’re winning/lagging.

## 📱 Demo

*(Planned – to be updated once UI is built)*  
- Project–Team Matching flow  
- Solana escrow and milestone approval  
- Team Chemistry dashboard

## 🤝 Contributing

1. Fork the repo  
2. Create a feature branch: `git checkout -b feature/matching-engine`  
3. Commit changes: `git commit -m "feat: add initial project-team matching"`  
4. Push: `git push origin feature/matching-engine`  
5. Open a pull request

## 📄 License

MIT – see `LICENSE`.

## 🙋 Contact

Creator: YOUR_NAME / YOUR_GITHUB_USERNAME  
Issues: open an issue in this repo

---
