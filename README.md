# TaskCoins.io — Full Product Specification

**Document for: Development Team**
**Date: 2026-03-08**
**Version: 1.0**

---

## 1. Platform Overview

TaskCoins is a micro-task platform where advertisers pay workers ("Chillers") to distribute content across social media. The platform is powered by its own ERC-20 token — TaskCoins — which serves as the sole payment currency.

**Business Model:** Advertisers fund campaigns in TaskCoins → Chillers complete tasks → Platform takes 20% cut off-chain → Chillers receive 80%.

**Revenue comes from the platform fee, NOT from selling tokens.**

---

## 2. Token Specs

| Parameter | Value |
|-----------|-------|
| Token Name | TaskCoins |
| Token Symbol | TASK (or TBC by founder) |
| Network | Ethereum (ERC-20) |
| Total Supply | ~590,000,000 (mirrors SOL circulating supply) |
| On-chain Tax | NONE — clean ERC-20, zero transfer fees |
| Platform Fee | 20% taken off-chain by backend before distributing to workers |
| Launch | Uniswap V2/V3 on Day 1 |
| CEX Target | MEXC or LBank within 1 week of launch |

**Important:** The token contract has NO special mechanics — standard ERC-20 only. The 20% cut is a platform-level operation, not a token-level tax. This keeps the token CEX-friendly and doesn't penalize holders/traders.

---

## 3. Account Types

### 3.1 Advertiser Account

An advertiser is any person or company that wants content distributed across social media.

**Features:**
- Sign up with email + password OR wallet connect (MetaMask, WalletConnect)
- Dashboard: create campaigns, fund wallet, track task completion, view analytics
- Deposit TaskCoins from external wallet to platform balance
- Create campaigns: define task type, platform target, content to post, reward per task, number of tasks
- View proof submissions from Chillers (screenshots, links)
- Approve or reject proof submissions
- Campaign analytics: how many posts live, estimated reach, engagement proof
- Withdraw unused TaskCoins back to wallet

### 3.2 Chiller Account

A Chiller is a worker who completes tasks and earns TaskCoins.

**Features:**
- Sign up with email + password OR wallet connect
- Dashboard: browse available tasks, track earnings, view level progress
- Task board: filter by platform (X, Reddit, CMC, Binance Square, YouTube, Telegram), reward amount, difficulty
- Submit proof: upload screenshot + paste post link
- Earnings wallet: view balance, withdraw TaskCoins to external wallet
- Profile: show level, reputation score, tasks completed, platforms active on
- Referral link: invite friends, earn 5% of their earnings

---

## 4. Chiller Level System

Chillers progress through levels based on tasks completed. Higher levels unlock higher-paying tasks.

| Level | Name | Tasks Required | Perks |
|-------|------|---------------|-------|
| 1 | Bronze | 0 | Access to basic tasks only |
| 2 | Silver | 50 | Access to medium-tier tasks |
| 3 | Gold | 200 | Access to premium tasks + priority queue |
| 4 | Diamond | 500 | Access to VIP tasks + direct advertiser offers |
| 5 | Legend | 1,000+ | Featured on leaderboard + highest-paying tasks |

**Level benefits:**
- Higher level = access to better-paying tasks
- Advertisers can target specific levels (e.g., "Gold+ only" for quality campaigns)
- Level displayed on public profile

---

## 5. Reputation Score

Every Chiller has a reputation score (0-100) based on:

| Factor | Weight |
|--------|--------|
| Task approval rate (% of submissions approved by advertisers) | 40% |
| Tasks completed | 25% |
| Account age | 10% |
| Consistency (tasks per week streak) | 15% |
| Flags/reports against account | 10% (penalty) |

**Impact:**
- Score below 50 = restricted from premium tasks
- Score below 30 = account review / temporary suspension
- Score above 80 = "Trusted Chiller" badge visible to advertisers

---

## 6. Task System

### 6.1 Task Categories

| Category | Platform | What the Chiller does |
|----------|----------|----------------------|
| Post on X | X (Twitter) | Copy-paste provided text + image, post from their account |
| Post on Reddit | Reddit | Post in specified subreddit with provided content |
| Post on CMC | CoinMarketCap Community | Post in specified coin's community page |
| Post on Binance Square | Binance Square | Post provided content on Binance Square |
| YouTube Comment | YouTube | Comment on specified video with provided text |
| Telegram Share | Telegram | Share post in specified Telegram groups |
| Follow/Like/Retweet | Multiple | Engagement tasks (lower reward) |

### 6.2 Task Lifecycle

```
Advertiser creates campaign
    → Tasks appear on task board
        → Chiller claims a task
            → Chiller posts content on their account
                → Chiller submits proof (screenshot + link)
                    → System auto-verifies OR advertiser manually approves
                        → TaskCoins released to Chiller (80% of task reward)
                        → Platform keeps 20%
```

### 6.3 Anti-Cheat System

- **Screenshot verification:** AI checks that screenshot matches the required platform and content
- **Link verification:** System visits the submitted URL to confirm the post is live and matches the content
- **Duplicate detection:** Same screenshot or link cannot be submitted twice
- **Account age check:** Chiller's social accounts must be older than 30 days
- **Rate limiting:** Max tasks per chiller per hour to prevent bot farming
- **Flag system:** Advertisers can flag suspicious submissions → triggers manual review

---

## 7. Staking

Chillers can stake TaskCoins on the platform to unlock benefits.

| Stake Amount | Benefit |
|-------------|---------|
| 1,000 TASK | Access to premium task queue |
| 5,000 TASK | 5% bonus on all task earnings |
| 10,000 TASK | 10% bonus + early access to new campaigns |
| 50,000 TASK | VIP status + direct advertiser matching |

**Purpose:** Reduces sell pressure by locking tokens, rewards committed community members.

---

## 8. Referral Program

- Every Chiller gets a unique referral link
- When a referred user signs up and completes their first task, the referrer earns a bonus
- Ongoing: referrer earns **5% of the referred Chiller's earnings** (paid by platform from its 20% cut, NOT from the Chiller's 80%)
- Referral dashboard: track invites, active referrals, total earnings from referrals

---

## 9. Leaderboard

Public page showing top-performing Chillers.

**Rankings by:**
- Most tasks completed (weekly / monthly / all-time)
- Most TaskCoins earned (weekly / monthly / all-time)
- Highest reputation score
- Most referrals

**Display:** Username, avatar, level badge, tasks completed, reputation score, platforms active on.

**Purpose:** Creates competition. People grind harder when they see others earning.

---

## 10. Pages

### 10.1 Landing Page (Home)
- Hero section: "Complete Tasks. Earn TaskCoins."
- How it works (3 steps): Sign up → Complete tasks → Earn crypto
- Live stats: total tasks completed, total TaskCoins distributed, active Chillers
- CTA: "Start Earning" / "Launch a Campaign"

### 10.2 University Page
Educational hub with courses and guides.

**Courses:**
- How to grow your X (Twitter) account from 0 to 10K
- How to grow your Reddit karma and authority
- How to build a YouTube channel
- How to maximize earnings on TaskCoins
- Crypto basics for beginners
- How to use MetaMask and manage your wallet

**Format:** Video lessons + text guides, organized by difficulty (Beginner / Intermediate / Advanced). Free for all registered users.

### 10.3 Services Page
Premium B2B services offered by the TaskCoins team.

| Service | Description |
|---------|-------------|
| **PR Writing** | Professional crypto press release writing for projects |
| **YouTuber Promotion** | Get your project featured by crypto YouTubers |
| **Distribution on Outlets** | Get your news published on major crypto news outlets |
| **dApp Creation** | Smart contract development + frontend for Web3 projects |
| **Token Launch** | ERC-20/BEP-20 token creation + Uniswap listing assistance |
| **NFT Development** | NFT collection creation, minting page, marketplace listing |
| **Smart Contract Audit** | Security audit for existing smart contracts |
| **Web3 Consulting** | Advisory on tokenomics, go-to-market, community building |

Each service has its own card with description, starting price (in TaskCoins or USD), and "Request Quote" button.

### 10.4 Blog Page
Daily articles and updates.

**Content types:**
- TaskCoins token news and updates
- Partnership announcements
- Platform feature releases
- Crypto industry news
- Community highlights and top Chiller spotlights

**Format:** Standard blog layout with categories, search, featured posts.

### 10.5 Whitepaper Page
Full tokenomics and platform documentation.

**Sections:**
- Abstract / Executive Summary
- Problem Statement (why micro-task platforms need crypto)
- Solution (TaskCoins platform + token)
- Token Utility
- Supply: ~590,000,000 TASK
- Allocation breakdown (team, liquidity, treasury, community, airdrop)
- Platform fee model (20% off-chain cut)
- Burn mechanism (5% of platform's 20% cut burned quarterly)
- Staking model
- Governance roadmap
- Team
- Legal disclaimer

### 10.6 Roadmap Page
Visual timeline of milestones.

**Suggested phases:**

| Phase | Timeline | Milestones |
|-------|----------|-----------|
| Phase 1 — Launch | Month 1 | Token deploy, Uniswap listing, platform beta, first 300 Chillers onboarded |
| Phase 2 — Growth | Month 2-3 | CEX listing (MEXC/LBank), University launch, 1,000 Chillers, anti-cheat v1 |
| Phase 3 — Scale | Month 4-6 | Mobile app (PWA), Services marketplace live, staking launch, 5,000 Chillers |
| Phase 4 — Expand | Month 6-12 | Multi-language support, advertiser API, governance voting, 20,000 Chillers |
| Phase 5 — Ecosystem | Year 2 | Mobile native app, additional CEX listings, DAO governance, 100,000 Chillers |

### 10.7 Advertiser Marketplace
Browse Chiller profiles before creating campaigns.

- Filter by: platform expertise, level, reputation score, follower count
- Premium Chillers can set higher task rates
- Direct hire: advertisers can offer tasks directly to specific Chillers

### 10.8 Proof Gallery
Public wall of completed task proof.

- Shows recent completed tasks with screenshots and links
- Builds trust for new advertisers considering the platform
- Filter by platform, campaign type, date

---

## 11. Burn Mechanism

- Every quarter, the platform burns **5% of the 20% it collected** in platform fees
- Example: Platform collected 1,000,000 TASK in Q1 fees → burns 50,000 TASK
- Burn transactions are public on-chain and announced on the blog
- **Purpose:** Decreasing supply over time → deflationary pressure → rewards long-term holders

---

## 12. Advertiser Bonus (Early Growth)

To attract initial advertisers:
- Pay for a 1,000 TASK campaign → get 1,050 TASK in distribution (5% bonus)
- Platform subsidizes the extra from treasury
- Limited to first 6 months or first $X in campaign volume
- Announced as a "Launch Promotion" to create urgency

---

## 13. Multi-Language Support

Priority languages for micro-task markets:

| Language | Market |
|----------|--------|
| English | Global |
| Arabic | MENA region |
| Spanish | Latin America |
| Turkish | Turkey (huge crypto adoption) |
| Indonesian | Southeast Asia |
| Russian | CIS countries |
| Portuguese | Brazil |

Full UI translation + University courses in top 3 languages minimum at launch.

---

## 14. Mobile App

- **Phase 1:** Progressive Web App (PWA) — works on any phone browser, installable
- **Phase 2:** Native apps (iOS + Android) when user base justifies the investment
- Chillers will primarily use the platform from mobile — the UI must be mobile-first

---

## 15. Advertiser Analytics Dashboard

| Metric | Description |
|--------|-------------|
| Tasks completed | How many of the campaign tasks were finished |
| Tasks pending | Awaiting Chiller action |
| Tasks in review | Proof submitted, awaiting verification |
| Posts live | Confirmed live posts with links |
| Estimated reach | Sum of Chiller follower counts who posted |
| Spend | Total TaskCoins spent on this campaign |
| Cost per post | Average TASK per completed task |

---

## 16. Technical Architecture (Recommendation)

| Layer | Suggested Stack |
|-------|----------------|
| Frontend | Next.js + Tailwind CSS (mobile-first) |
| Backend | Node.js API (Express or Next.js API routes) |
| Database | PostgreSQL (Supabase or self-hosted) |
| Auth | Email/password + Web3 wallet (MetaMask, WalletConnect) via RainbowKit or wagmi |
| Token interaction | ethers.js or viem for deposit/withdraw |
| Image storage | Supabase Storage or AWS S3 |
| Hosting | Vercel (frontend) + Railway or AWS (backend) |
| Anti-cheat | Custom AI screenshot verification + URL scraping |

---

## 17. Payment Flow (Detailed)

### Advertiser Deposits
```
Advertiser connects wallet (MetaMask)
    → Sends TASK tokens to platform deposit contract
        → Platform credits their internal balance
            → Advertiser creates campaign from internal balance
```

### Chiller Withdrawal
```
Chiller requests withdrawal from internal balance
    → Platform deducts amount from internal balance
        → Platform smart contract sends TASK to Chiller's wallet
            → Transaction confirmed on-chain
```

### Platform Cut (Off-Chain)
```
Advertiser funds campaign: 1,000 TASK
    → Backend splits: 800 TASK → task pool | 200 TASK → platform treasury
        → Each completed task pays from the 800 pool
            → Platform treasury accumulates the 200
                → Quarterly: 5% of treasury burned
```

---

## 18. Token Allocation (Suggested — Founder to Confirm)

| Allocation | % | Tokens | Notes |
|-----------|---|--------|-------|
| Uniswap Liquidity | 30% | 177,000,000 | Paired with ETH at launch |
| Platform Treasury | 25% | 147,500,000 | For operations, advertiser bonuses, burns |
| Team | 15% | 88,500,000 | 12-month vesting (required for CEX) |
| Community Airdrop | 10% | 59,000,000 | First 300 army + early users |
| Marketing | 10% | 59,000,000 | Listings, influencers, promotions |
| Staking Rewards | 10% | 59,000,000 | Distributed to stakers over 24 months |

**Founder must confirm these numbers before token deployment.**

---

## 19. CEX Listing Checklist (MEXC / LBank)

| Requirement | Status |
|-------------|--------|
| Clean ERC-20 contract (no tax) | ✅ Planned |
| Token deployed on mainnet | ⬜ Pending |
| Uniswap liquidity live | ⬜ Pending |
| CoinGecko / CoinMarketCap listing application | ⬜ Pending |
| Whitepaper published | ⬜ Pending |
| Team KYC (some exchanges require it) | ⬜ Check with exchange |
| Listing fee budget | ⬜ Founder to confirm |
| Minimum trading volume on Uniswap | ⬜ Need organic volume first |
| Smart contract audit (even basic) | ⬜ Recommended |

---

## 20. Summary — All Pages

| # | Page | Priority |
|---|------|----------|
| 1 | Landing Page (Home) | P0 — Must have |
| 2 | Sign Up / Login (Advertiser + Chiller) | P0 |
| 3 | Advertiser Dashboard | P0 |
| 4 | Chiller Dashboard | P0 |
| 5 | Task Board | P0 |
| 6 | Wallet (Deposit / Withdraw) | P0 |
| 7 | Whitepaper | P0 |
| 8 | Roadmap | P0 |
| 9 | Blog | P1 — Important |
| 10 | University | P1 |
| 11 | Services | P1 |
| 12 | Leaderboard | P1 |
| 13 | Referral Dashboard | P1 |
| 14 | Advertiser Marketplace | P2 — Nice to have at launch |
| 15 | Proof Gallery | P2 |
| 16 | Staking Page | P2 |
| 17 | Admin Panel (internal) | P0 |

---

## 21. Go-To-Market: Three-Front Strategy

TaskCoins launches on three simultaneous fronts. All three feed each other — none works alone.

### Front 1: Chillers (Supply Side — Grow the Workforce)

**Goal:** Recruit and retain thousands of active Chillers who complete tasks daily.

| Channel | Tactic |
|---------|--------|
| **YouTubers** | Partner with 3-5 mid-tier crypto YouTubers (50K-200K subs) to show themselves earning TaskCoins live on camera — "I earned X TaskCoins in 1 hour" |
| **Referral Program** | Every Chiller recruits more Chillers — 5% of referred earnings incentivizes organic growth |
| **University** | Free courses on growing social accounts attract people who want to earn more per task |
| **Micro-task communities** | Target existing SEOSprint, Picoworkers, Microworkers users — they already understand the model |
| **Developing markets** | Focus on regions where $5-10/day is meaningful income — Southeast Asia, MENA, Latin America, CIS |
| **Kira Army** | The original 300 army members are Day 1 Chillers — already trained, already engaged |

### Front 2: Token (Volume + Liquidity — Fuel the Economy)

**Goal:** Drive buy pressure, trading volume, and token visibility to support the platform economy.

| Channel | Tactic |
|---------|--------|
| **PR on major outlets** | CoinDesk, CoinTelegraph, Bitcoin Magazine — same outlets and relationships used for Pepeto |
| **Bitcoinomist coverage** | Our own media outlet publishes TaskCoins news on Day 1 and ongoing |
| **CEX listings** | MEXC or LBank within Week 2 — makes the token accessible to non-DeFi users |
| **CMC + CoinGecko** | Listing applications submitted on Day 1 — visibility to millions of crypto users |
| **Burn mechanism** | 5% quarterly burn of platform fees creates deflationary narrative for holders |
| **Staking** | Locks supply, reduces sell pressure, rewards committed community |
| **Kira distribution** | Kira auto-generates content about TaskCoins and distributes across X, Reddit, CMC, Binance Square |

### Front 3: Advertisers (Demand Side — Bring the Money)

**Goal:** Attract advertisers who buy TaskCoins to fund campaigns. This is the most critical front — without advertisers, there are no tasks and no earnings.

| Target | Why they need TaskCoins |
|--------|----------------------|
| **Crypto projects launching tokens** | They need distribution — 300 people posting about their launch in 24 hours |
| **NFT projects** | Need buzz and social proof before mint |
| **CEXs promoting new listings** | Want community awareness for newly listed tokens |
| **DeFi protocols** | Need user awareness for new features or chain expansions |
| **Web3 gaming** | Need player acquisition and social buzz |
| **Pepeto network** | Every project we know from Pepeto's journey is a potential advertiser — warm leads from Day 1 |

**Sales pitch:** "Pay 10,000 TaskCoins → get 300 real people posting about your project across X, Reddit, CMC, Binance Square within 24 hours. Verified proof for every post."

### Front 4: Investors (Buy Pressure — Fuel the Price)

**Goal:** Attract direct investors to the token using FOMO marketing and the "next 100x" narrative. Because TaskCoins has real utility, this is 10x easier than a pure meme coin.

**Why investors buy TaskCoins over random launches:**

| What investors see | Why it matters |
|-------------------|---------------|
| Platform is LIVE | Not a whitepaper promise — taskcoins.io is working today |
| Users are earning | Real people completing real tasks = proof of demand |
| Advertisers are paying | Buy pressure comes from business revenue, not just speculation |
| 20% platform fee | This is a real business with real revenue — not "we'll figure it out" |
| Quarterly burns | Supply decreases over time — deflationary by design |
| CEX listings | MEXC/LBank = accessibility for retail investors |
| Pepeto team | Proven track record of launching and scaling a crypto project |

**FOMO Marketing Angles:**

- "TaskCoins is the next 100x — real platform, real revenue, real users earning daily"
- "This is what [100x coin] looked like at $1M market cap before it exploded"
- "The platform takes 20% of every transaction — imagine what happens when 100K users are on it"
- "You're not buying a meme — you're buying equity in a working business"
- "While other coins have zero utility, TaskCoins powers an entire economy of 300+ active workers"
- "Life-changing opportunity — utility tokens with live products are the ones that survive and 100x"

**Investor channels:**

| Channel | Tactic |
|---------|--------|
| **Crypto Twitter / X** | Paid KOLs (Key Opinion Leaders) posting "next 100x" threads with platform screenshots |
| **Telegram caller groups** | Get TaskCoins called in 5-10 active caller channels |
| **YouTube investors** | Different angle than Chiller YouTubers — these focus on "why TASK token will 100x" not "how to earn" |
| **CoinDesk / CoinTelegraph PRs** | Investor-focused articles: "TaskCoins raises $X in first week" / "New utility token powers micro-task economy" |
| **Dex trending** | Push for DEXTools / DEXScreener trending on launch day — investors watch these |
| **CMC / CoinGecko** | Fast-tracked listing = visibility to millions of investors daily |

**Why utility kills meme coins for investor confidence:**

Most meme coins pump and dump because there's no reason to hold. TaskCoins has built-in buy pressure:
- Every advertiser MUST buy TaskCoins to run campaigns
- Every quarter, tokens get burned
- Staking locks supply
- As the platform grows, demand for the token grows with it

This means even after the initial FOMO wave, there's sustained demand. That's what turns a pump into a long-term hold.

### The Flywheel (All 4 Fronts)

```
More Chillers → stronger offer for advertisers ("we have 5,000 active posters")
    → More advertisers → more buy pressure on token + more tasks available
        → More token volume → more PR coverage → attracts more Chillers + advertisers
            → Rising price → FOMO investors pile in → more liquidity + volume
                → More PR coverage about the price action → more Chillers + advertisers + investors
                    → Cycle repeats, each loop bigger than the last
```

### Launch Sequence (Week 1-2)

| Day | Action |
|-----|--------|
| Day 1 | Token deploy + Uniswap liquidity live |
| Day 1 | Bitcoinomist PR published (own outlet — instant) |
| Day 1 | CMC + CoinGecko listing applications submitted |
| Days 1-3 | 3-5 YouTuber videos go live (showing platform + earning) |
| Days 3-5 | CoinDesk / CoinTelegraph PR published (timed after initial volume builds) |
| Week 2 | MEXC or LBank listing goes live |
| Week 2 | Second wave PRs on listing day (new news cycle, new momentum) |

Every step feeds the next. YouTuber volume strengthens the CEX application. CEX listing creates a second PR cycle. Second PR cycle brings new users. New users = more tasks = more volume. The loop never stops.

---

## 22. Competitive Advantage

| Factor | TaskCoins | Galxe / Layer3 / Zealy |
|--------|-----------|----------------------|
| **Model** | Get paid to post content on YOUR accounts | Complete Web3 quests (bridge, swap, mint) |
| **Payment** | Native token with real utility | Points or random airdrops |
| **Media** | Own media outlet (Bitcoinomist) feeding content | No media arm |
| **Distribution** | Kira auto-generates platform-ready content | Manual content creation |
| **Team** | Pepeto launch experience, outlet relationships | Varies |
| **Advertiser value** | Real social posts from real accounts with proof | Quest completions (less visible marketing) |

---

**End of Specification**

*This document contains all features planned for TaskCoins.io v1. The dev should build P0 items first, then P1, then P2. The four-front GTM strategy (Chillers + Token + Advertisers + Investors) runs in parallel with development.*
