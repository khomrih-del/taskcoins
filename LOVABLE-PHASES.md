# TaskCoins.io — Lovable Build Phases

Copy-paste each phase to Lovable after the previous one is complete.

---

## Phase 1 — APPROVED BY LOVABLE (In Progress)

Landing page, Navigation, Sign Up/Login, Chiller Dashboard, Task Board, Design System.

**Already sent. Let Lovable build it.**

---

## Phase 2 — Wallet + Advertiser Side

After Phase 1 is complete, send this:

```
Now add these pages to the existing build:

### Wallet Page (Both account types)
- Large balance display with TASK token icon at the top
- Two tabs: Deposit and Withdraw
- Deposit tab: "Connect Wallet" button → enter amount → mock approve transaction → mock confirm
- Withdraw tab: enter amount → destination wallet address field → "Request Withdrawal" button
- Withdrawal warming rules displayed clearly with a progress bar:
  - New accounts (0-30 days): "Withdrawals unlock after 30 days of activity" — show countdown timer
  - Warmed accounts (30-60 days): "You can withdraw once per month, minimum 500 TASK"
  - Trusted accounts (60+ days, reputation 70+): "Bi-weekly withdrawals, minimum 200 TASK"
  - VIP accounts (Diamond+, reputation 90+): "Weekly withdrawals, minimum 100 TASK"
- Banner at top: "TaskCoins is designed for long-term growth. The longer you hold, the more your earnings are worth."
- Transaction history table below: date, type (earned/withdrawn/staked/deposited), amount, status badge (completed=green, pending=yellow, failed=red)
- Pre-populate with 15 sample transactions

### Advertiser Dashboard
- Sidebar navigation: Dashboard, Create Campaign, My Campaigns, Review Proofs, Analytics, Wallet, Settings
- Dashboard cards row: Total Spend (TASK), Active Campaigns, Tasks Completed, Posts Live, Estimated Reach
- Recent campaign activity feed below the cards (list of recent events like "Task #234 approved", "Campaign X completed 80%")
- Quick action button: "Create New Campaign" — prominent blue CTA

### Create Campaign Page (Advertiser)
- Step-by-step wizard with progress bar at top (Step 1 of 5):
  - Step 1 — Choose Platform: Grid of platform cards with icons (X, Reddit, CMC Community, Binance Square, YouTube, Telegram). Multi-select. Each card highlights when selected.
  - Step 2 — Write Content: Text editor for post content (textarea) + image upload drag-and-drop area + optional "Link to include" field
  - Step 3 — Set Requirements: Dropdown for minimum Chiller level (Any, Silver+, Gold+, Diamond+), minimum reputation score slider (0-100), text area for specific instructions
  - Step 4 — Set Budget: Input for "Reward per task" (in TASK), input for "Number of tasks needed", auto-calculated total showing breakdown: "800 TASK to workers + 200 TASK platform fee = 1,000 TASK total" (20% fee shown transparently)
  - Step 5 — Review & Launch: Summary card of all selections, "Launch Campaign" button
- After launch: redirect to My Campaigns page showing the new campaign as "Active"
- Pre-populate with 3 sample campaigns in different states (active, completed, paused)

### My Campaigns Page (Advertiser)
- Table/card list of all campaigns
- Each shows: title, platform icons, status badge (Active/Paused/Completed), progress bar (tasks completed/total), total spend, date created
- Click a campaign → detail view with list of all task submissions, approve/reject buttons for each proof

### Review Proofs Page (Advertiser)
- Queue of submitted proofs awaiting review
- Each proof card shows: Chiller username + avatar, platform icon, screenshot thumbnail (clickable to expand), submitted link (clickable), timestamp
- Two action buttons per card: "Approve" (green) and "Reject" (red, shows text input for rejection reason)
- Filter tabs: All Pending, By Campaign dropdown

### Advertiser Analytics Page
- Cards row: Total Tasks Completed, Total Posts Live, Average Cost Per Post, Estimated Total Reach
- Line chart: campaign performance over time (tasks completed per day)
- Bar chart: performance by platform (X vs Reddit vs CMC etc.)
- Table: top performing Chillers for this advertiser's campaigns

Use the same dark crypto-native design system from Phase 1. Keep everything consistent.
```

---

## Phase 3 — Whitepaper + Roadmap + University

After Phase 2 is complete, send this:

```
Now add these pages:

### Whitepaper Page
- Clean, document-style reading layout on dark background
- Sticky table of contents sidebar on desktop (collapses to dropdown on mobile):
  1. Abstract
  2. Problem Statement
  3. The TaskCoins Solution
  4. Platform Architecture
  5. Token Utility
  6. Tokenomics
  7. Allocation
  8. Platform Fee Model
  9. Burn Mechanism
  10. Staking Model
  11. Governance Roadmap
  12. Team
  13. Legal Disclaimer
- Section 6 — Tokenomics: Display "Total Supply: 590,000,000 TASK" prominently
- Section 7 — Allocation: Animated pie/donut chart showing: Uniswap Liquidity 30%, Platform Treasury 25%, Team 15% (12-month vesting), Community Airdrop 10%, Marketing 10%, Staking Rewards 10%
- Section 8 — Platform Fee: Visual diagram showing the 20% split flow (Advertiser pays 1000 → 800 to workers, 200 to platform)
- Section 9 — Burn: Explain 5% quarterly burn with simple infographic
- "Download PDF" button in the header area
- Add placeholder paragraph text for each section (3-5 sentences each, professional tone)
- Typography: large section headings in Satoshi, body in Inter, generous line height for readability

### Roadmap Page
- Vertical timeline design, alternating left/right on desktop, single column on mobile
- Each phase is a card connected by a vertical line
- Status indicators: completed phases = green dot with checkmark, in progress = blue pulsing dot, upcoming = gray dot
- Phases:
  - Phase 1 — Launch (Month 1) — Status: In Progress
    - Token deploy on Ethereum
    - Uniswap liquidity live
    - Platform beta launch
    - First 300 Chillers onboarded
  - Phase 2 — Growth (Month 2-3) — Status: Upcoming
    - CEX listing (MEXC / LBank)
    - University launch with first courses
    - 1,000 active Chillers
    - Anti-cheat system v1
  - Phase 3 — Scale (Month 4-6) — Status: Upcoming
    - Mobile PWA release
    - Services marketplace live
    - Staking launch
    - 5,000 active Chillers
  - Phase 4 — Expand (Month 6-12) — Status: Upcoming
    - Multi-language support (Arabic, Spanish, Turkish, Indonesian)
    - Advertiser API for programmatic campaign creation
    - Governance voting for token holders
    - 20,000 active Chillers
  - Phase 5 — Ecosystem (Year 2) — Status: Upcoming
    - Native mobile apps (iOS + Android)
    - Additional CEX listings
    - DAO governance
    - 100,000 active Chillers
- Subtle animation: timeline fills in as user scrolls down

### University Page
- Hero: "TaskCoins University — Learn, Grow, Earn More"
- Course grid (3 columns desktop, 1 column mobile)
- Each course card: thumbnail placeholder image, title, difficulty badge (green=Beginner, orange=Intermediate, red=Advanced), lesson count, estimated time, "Start Course" button
- Courses to create:
  1. "How to Grow Your X Account from 0 to 10K" — Beginner — 8 lessons — 45 min
  2. "Reddit Karma Building: The Complete Guide" — Beginner — 6 lessons — 30 min
  3. "YouTube Channel Growth for Beginners" — Intermediate — 10 lessons — 60 min
  4. "Maximize Your TaskCoins Earnings" — Beginner — 5 lessons — 20 min
  5. "Crypto Basics: Wallets, Tokens, and DeFi" — Beginner — 7 lessons — 35 min
  6. "How to Use MetaMask Like a Pro" — Beginner — 4 lessons — 15 min
- Click a course → Course detail page with: course header (title, difficulty, progress bar), lesson list sidebar, content area (placeholder text + video embed placeholder), "Mark as Complete" button per lesson, "Next Lesson" button
- Progress tracking: green checkmarks on completed lessons

Keep the same dark design system. Consistent with everything built so far.
```

---

## Phase 4 — Services + Blog + Leaderboard + Referrals

After Phase 3 is complete, send this:

```
Now add these pages:

### Services Page
- Hero: "Web3 Services — Built by the Team Behind Pepeto"
- Service cards in 2-column grid (1 column on mobile):
  1. PR Writing — "Professional crypto press releases" — icon: document — Starting at 5,000 TASK
  2. YouTuber Promotion — "Get featured by crypto YouTubers (50K-200K subs)" — icon: play button — Starting at 10,000 TASK
  3. Distribution on Outlets — "Get published on CoinDesk, CoinTelegraph, and major outlets" — icon: newspaper — Starting at 25,000 TASK
  4. dApp Creation — "Smart contract + frontend for your Web3 project" — icon: code — Starting at 50,000 TASK
  5. Token Launch — "ERC-20/BEP-20 creation + Uniswap listing" — icon: rocket — Starting at 30,000 TASK
  6. NFT Development — "Collection, minting page, marketplace listing" — icon: image — Starting at 20,000 TASK
  7. Smart Contract Audit — "Security audit for existing contracts" — icon: shield — Starting at 15,000 TASK
  8. Web3 Consulting — "Tokenomics, GTM, community building" — icon: lightbulb — Starting at 10,000 TASK
- Each card has "Request Quote" button → opens modal form: name, email, project URL, budget dropdown, description textarea, "Submit Request" button
- Bottom section: "Why Choose Us?" — 3 cards: "Proven Team" (Pepeto track record), "End-to-End" (from token to marketing), "Results-Driven" (real metrics, not promises)

### Blog Page
- Hero: featured post (large card with image, title, excerpt, date, "Read More")
- Below: grid of posts (3 columns desktop, 1 mobile)
- Category filter bar: All, News, Updates, Partnerships, Guides, Community
- Each post card: featured image placeholder, title, excerpt (2 lines), date, category badge, read time
- Create 3 placeholder blog posts:
  1. "TaskCoins Launches: The Future of Social Media Earning" — News — 5 min read
  2. "How 300 Chillers Earned Their First TaskCoins" — Community — 3 min read
  3. "TaskCoins Tokenomics Explained: Why We Built a Utility Token" — Guides — 7 min read
- Individual blog post page: hero image, title, author avatar + name + date, content area with placeholder paragraphs, share buttons (X, Telegram, copy link), "Related Posts" section at bottom with 2 post cards

### Leaderboard Page
- Hero: "Top Chillers — Compete, Climb, Earn"
- Time filter tabs: This Week, This Month, All Time
- Category tabs: Most Tasks, Most Earned, Best Reputation, Most Referrals
- Rankings table:
  - Columns: Rank (#), Avatar, Username, Level Badge, Tasks Completed, TASK Earned, Reputation Score, Platforms (icons)
  - Top 3 rows highlighted: gold background for #1, silver for #2, bronze for #3
  - Rows 4-50 normal styling
- "Your Rank" sticky bar at bottom of viewport showing logged-in user's position: "You are ranked #47 — complete 12 more tasks to reach #40"
- Pre-populate with 50 sample users with varied levels, scores, and earnings

### Referral Page (Chiller)
- Hero section: "Invite Friends. Earn 5% of Everything They Make — Forever."
- Referral link box: large display of unique link with "Copy" button and share buttons (X, Telegram, WhatsApp, Email)
- Stats cards row: Total Referrals, Active Referrals (completed at least 1 task), Total Referral Earnings (TASK)
- Referral table: Avatar, Username, Signed Up date, Their Tasks Completed, Your Earnings from Them
- Explainer section at bottom: "How it works" — 3 steps with icons:
  1. "Share your link" — They sign up with your code
  2. "They earn" — They complete tasks and get paid
  3. "You earn" — 5% of their earnings credited to you automatically (from platform fee, NOT from their pay)
- Pre-populate with 5 sample referrals

Keep the same design system. All pages consistent.
```

---

## Phase 5 — Staking + Proof Gallery + Marketplace

After Phase 4 is complete, send this:

```
Now add these pages:

### Staking Page (Chiller)
- Hero: "Stake TaskCoins — Unlock Premium Rewards"
- Current status card: amount currently staked, current tier unlocked, active benefits listed
- Staking tiers displayed as 4 horizontal cards (scrollable on mobile):
  - Tier 1: 1,000 TASK → "Access premium tasks" — icon: star
  - Tier 2: 5,000 TASK → "5% bonus on all earnings" — icon: trending up
  - Tier 3: 10,000 TASK → "10% bonus + early access to campaigns" — icon: lightning
  - Tier 4: 50,000 TASK → "VIP status + direct advertiser offers" — icon: crown
  - Current tier highlighted with blue glow border, locked tiers slightly dimmed with lock icon
- Stake section: input field with "Amount to stake" + "Max" button + "Stake Now" blue CTA
- Unstake section: input field + "Request Unstake" button + warning text: "7-day cooldown period. Benefits remain active during cooldown."
- Staking history table: date, action (Staked/Unstaked), amount, status

### Proof Gallery Page (Public — No Login Required)
- Hero: "Real Tasks. Real Posts. Real Proof."
- Filter bar: All Platforms, X, Reddit, CMC, Binance Square, YouTube, Telegram
- Masonry grid of proof cards:
  - Each card: screenshot thumbnail (click to expand in lightbox), platform icon badge in corner, task type label, Chiller username, date completed, "Verified" green badge
  - Hover effect: slight scale up + glow
- "Load More" button at bottom (or infinite scroll)
- Pre-populate with 20 sample proof cards using placeholder screenshots
- Purpose text at top for advertisers: "Every task on TaskCoins is verified with screenshot proof and live links. See what our Chillers deliver."

### Advertiser Marketplace Page
- Hero: "Find the Perfect Chillers for Your Campaign"
- Filter sidebar (left on desktop, top sheet on mobile):
  - Platform expertise: checkboxes (X, Reddit, CMC, etc.)
  - Level: dropdown (Any, Silver+, Gold+, Diamond+)
  - Reputation: range slider (0-100)
  - Follower count: range dropdown (Any, 1K+, 5K+, 10K+, 50K+)
  - Sort by: Most tasks completed, Highest reputation, Newest
- Chiller profile cards grid (3 columns desktop):
  - Avatar, username, level badge
  - Reputation score gauge (small circular)
  - Platform icons they're active on
  - Stats: tasks completed, member since
  - "Hire Directly" blue button
- Click "Hire Directly" → modal: select platform, write task content, set reward, "Send Offer" button
- Pre-populate with 15 sample Chiller profiles at various levels

Keep the same design system.
```

---

## Phase 6 — Backend + Real Wallet Connect + Admin

After Phase 5 is complete, send this:

```
Now connect the backend and add real functionality:

### Supabase Backend
Connect all existing UI to Supabase:

Create these tables:
- users: id, email, wallet_address, account_type (advertiser/chiller), display_name, avatar_url, level (1-5, default 1), reputation_score (0-100, default 50), total_earned (default 0), total_spent (default 0), tasks_completed (default 0), referral_code (unique), referred_by, created_at, last_active_at, is_banned (default false)
- campaigns: id, advertiser_id (FK users), title, description, content_text, content_image_url, platforms (text array), reward_per_task, total_tasks, tasks_completed (default 0), tasks_remaining, min_chiller_level (default 1), min_reputation (default 0), status (active/paused/completed/expired), created_at, expires_at
- tasks: id, campaign_id (FK campaigns), chiller_id (FK users), status (available/claimed/submitted/approved/rejected), proof_screenshot_url, proof_link, claimed_at, submitted_at, reviewed_at, rejection_reason
- wallets: id, user_id (FK users), balance (default 0), total_deposited, total_withdrawn, total_earned, total_spent, total_staked, withdrawal_tier (new/warmed/trusted/vip), first_task_completed_at
- transactions: id, user_id (FK users), type (deposit/withdrawal/earned/spent/staked/unstaked/referral_bonus/platform_fee), amount, status (pending/completed/failed), tx_hash, created_at
- stakes: id, user_id (FK users), amount, tier_unlocked, staked_at, unstake_requested_at, unstake_available_at
- referrals: id, referrer_id (FK users), referred_id (FK users), total_earned_from_referral, created_at
- blog_posts: id, title, slug, excerpt, content, featured_image_url, category, author, published_at, is_published
- service_requests: id, user_id, service_type, name, email, project_url, budget, description, status (new/in_progress/completed), created_at

### Auth
- Enable Supabase Auth with email/password
- Add Google OAuth provider
- On signup: create user record + wallet record + generate unique referral_code
- Account type selection (advertiser/chiller) saved to user profile

### Business Logic (Edge Functions)
- claim_task: Check chiller level >= campaign min_level, reputation >= min_reputation, active tasks < 3. Create task record with status "claimed", set claimed_at, start 24hr timer.
- submit_proof: Upload screenshot to Supabase Storage, save proof_link, update task status to "submitted"
- approve_task: Update task status to "approved", calculate reward, credit 80% to chiller wallet, 20% to platform wallet, increment chiller tasks_completed, check level upgrade
- reject_task: Update task status to "rejected", save rejection_reason, release task back to pool
- create_campaign: Verify advertiser balance >= total cost (reward * tasks * 1.25 for 20% fee), deduct from balance, create campaign
- process_referral: On task approval, if chiller has referred_by, credit 5% of platform's 20% cut to referrer
- check_level_up: After task approval, check tasks_completed thresholds (50=Silver, 200=Gold, 500=Diamond, 1000=Legend), update level

### Wallet Connect (RainbowKit + wagmi)
- Add RainbowKit provider wrapping the app
- Support MetaMask and WalletConnect
- Deposit flow: connect wallet → approve TASK token spend → transfer to platform contract address → credit internal balance
- Withdraw flow: request withdrawal → check warming tier rules → if approved, queue for processing
- Display connected wallet address in header (truncated)
- Show on-chain TASK balance alongside platform balance

### Admin Panel
- Route: /admin (protected, only admin accounts)
- Sidebar: Users, Campaigns, Tasks, Finances, Analytics, Blog, Content
- Users page: searchable table, view profile, ban/unban, adjust level/reputation manually
- Campaigns page: view all, pause/resume/delete campaigns
- Tasks page: view flagged/disputed tasks, override approve/reject
- Finances: total fees collected, treasury balance, burn log, revenue chart (daily/weekly/monthly)
- Analytics: DAU chart, new signups chart, tasks per day chart, revenue per day chart
- Blog editor: create/edit/delete blog posts with rich text editor, image upload, publish/unpublish toggle

Replace all placeholder/mock data with real Supabase queries. All forms should now save to the database. All dashboards should show real data from the database.
```

---

## Done

After all 6 phases, TaskCoins.io is a fully functional platform. Each phase builds on the previous one. Never skip a phase.
