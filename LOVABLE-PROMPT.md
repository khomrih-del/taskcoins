# TaskCoins.io — Lovable Build Prompt

Build a full-stack micro-task crypto platform called **TaskCoins** at taskcoins.io. The platform connects advertisers who need social media distribution with workers ("Chillers") who get paid in TaskCoins (ERC-20 token) to post content on their personal accounts.

---

## Tech Stack

- **Frontend:** React + Tailwind CSS (mobile-first, responsive)
- **Backend:** Supabase (auth, database, storage, edge functions)
- **Wallet:** RainbowKit + wagmi for MetaMask/WalletConnect integration
- **Charts:** Recharts for analytics dashboards

---

## Color Scheme & Branding

- Primary: Electric blue `#388EFF`
- Secondary: Green `#09CE84` (success/earnings)
- Warning: Orange `#FFA01E`
- Danger: Red `#FC564E`
- Background: Dark mode by default `#0A0E17` with card backgrounds `#111827`
- Text: White `#FFFFFF` primary, gray `#9CA3AF` secondary
- Font: Inter for body, Satoshi for headings
- Style: Clean, modern, crypto-native feel like dYdX or Blur — not playful, not corporate

---

## Two Account Types

### 1. Advertiser Account
- Signs up with email/password OR wallet connect
- Dashboard shows: active campaigns, total spend, tasks completed, tasks pending, posts live
- Can create campaigns: pick platform (X, Reddit, CMC, Binance Square, YouTube, Telegram), write content for Chillers to post, upload image, set reward per task, set number of tasks needed
- Can review proof submissions (screenshot + link) from Chillers — approve or reject each
- Can deposit TaskCoins from external wallet to platform balance
- Can withdraw unused TaskCoins back to wallet
- Analytics page: campaign performance, cost per post, estimated reach

### 2. Chiller Account
- Signs up with email/password OR wallet connect
- Dashboard shows: available balance, total earned, tasks completed, current level, reputation score, referral earnings
- Task board: browse available tasks filtered by platform, reward amount, difficulty
- Task flow: claim task → post content on their account → submit proof (upload screenshot + paste link) → wait for approval → earn TaskCoins
- Wallet page: view balance, request withdrawal (subject to warming rules — see below)
- Profile page: level badge, reputation score, platforms active on, tasks completed count
- Referral page: unique referral link, list of referrals, earnings from referrals
- Staking page: stake TaskCoins to unlock premium task tiers

---

## Pages to Build

### 1. Landing Page (Home)
- Hero section: "Complete Tasks. Earn TaskCoins." with CTA buttons "Start Earning" and "Launch a Campaign"
- Animated counter showing live stats: total tasks completed, total TaskCoins distributed, active Chillers (use placeholder numbers for now: 12,847 tasks / 2,450,000 TASK distributed / 1,234 Chillers)
- How it works section (3 steps with icons): Sign Up → Complete Tasks → Earn Crypto
- For Advertisers section: "Get 300 real people posting about your project in 24 hours" with campaign pricing preview
- For Chillers section: "Earn crypto by posting on social media — no investment needed" with earning examples
- Testimonials section (placeholder): 3 cards with avatar, name, quote, amount earned
- Partners/press logos bar (placeholder): CoinDesk, CoinTelegraph, CoinMarketCap logos area
- Footer: links to all pages, social icons, legal links

### 2. Sign Up / Login Page
- Toggle between Advertiser and Chiller account type
- Email + password form
- "Connect Wallet" button (MetaMask/WalletConnect via RainbowKit)
- "Sign up with Google" option
- Referral code field (optional, pre-filled if they came from a referral link)
- Terms of service checkbox

### 3. Advertiser Dashboard
- Sidebar navigation: Dashboard, Create Campaign, My Campaigns, Review Proofs, Analytics, Wallet, Settings
- Dashboard cards: Total Spend, Active Campaigns, Tasks Completed, Posts Live, Estimated Reach
- Recent campaign activity feed
- Quick action button: "Create New Campaign"

### 4. Create Campaign Page (Advertiser)
- Step-by-step wizard:
  - Step 1: Choose platform(s) — X, Reddit, CMC Community, Binance Square, YouTube, Telegram (multi-select with icons)
  - Step 2: Write content — text editor for the post content + image upload + optional link to include
  - Step 3: Set requirements — minimum Chiller level, minimum reputation score, specific instructions
  - Step 4: Set budget — reward per task (in TASK tokens), number of tasks, total campaign cost calculated automatically (includes 20% platform fee shown transparently: "800 TASK to workers + 200 TASK platform fee = 1,000 TASK total")
  - Step 5: Review & Launch — summary of everything, "Launch Campaign" button
- Campaign must deduct from advertiser's platform balance

### 5. Chiller Dashboard
- Sidebar navigation: Dashboard, Task Board, My Tasks, Wallet, Staking, Leaderboard, Referrals, University, Profile, Settings
- Dashboard cards: Available Balance, Total Earned (all time), Tasks Completed, Current Level (with progress bar to next level), Reputation Score (circular gauge)
- "Available Tasks" preview showing top 5 highest-paying tasks
- Earnings chart (line chart, last 30 days)
- Level progress section showing current perks and what they unlock at next level

### 6. Task Board (Chiller)
- Grid/list view toggle
- Filter sidebar: Platform (X, Reddit, CMC, Binance Square, YouTube, Telegram), Reward range (slider), Difficulty, Sort by (newest, highest reward, ending soon)
- Each task card shows: Platform icon, advertiser name, task title, reward amount (TASK), time remaining, difficulty badge, required level
- Click a task → Task Detail page: full instructions, content to post, image to use, submit proof form (screenshot upload + link input), "Claim Task" button
- After claiming: timer starts (24 hours to complete), task moves to "My Tasks"

### 7. My Tasks (Chiller)
- Tabs: Active (claimed, in progress), Submitted (awaiting review), Approved (completed, paid), Rejected (with reason)
- Each card shows task details + status badge + reward amount
- For active tasks: "Submit Proof" button
- For rejected tasks: "Resubmit" option if allowed

### 8. Wallet Page (Both account types)
- Balance display: large number with TASK token icon
- Two tabs: Deposit and Withdraw
- Deposit: "Connect Wallet" → enter amount → approve transaction → confirm
- Withdraw: enter amount → destination wallet address → request withdrawal
- **Withdrawal warming rules displayed clearly:**
  - New accounts (0-30 days): "Withdrawals unlock after 30 days of activity"
  - Warmed accounts (30-60 days): "You can withdraw once per month, minimum 500 TASK"
  - Trusted accounts (60+ days, reputation 70+): "Bi-weekly withdrawals, minimum 200 TASK"
  - VIP accounts (Diamond+, reputation 90+): "Weekly withdrawals, minimum 100 TASK"
- Progress bar showing how close they are to next withdrawal tier
- Transaction history table: date, type (earned/withdrawn/staked/deposited), amount, status
- Banner: "TaskCoins is designed for long-term growth. The longer you hold, the more your earnings are worth."

### 9. Staking Page (Chiller)
- Current staking status: amount staked, tier unlocked, benefits active
- Staking tiers displayed as cards:
  - 1,000 TASK → "Access premium tasks"
  - 5,000 TASK → "5% bonus on all earnings"
  - 10,000 TASK → "10% bonus + early access to campaigns"
  - 50,000 TASK → "VIP status + direct advertiser offers"
- "Stake" input with amount field and "Stake Now" button
- "Unstake" option with 7-day cooldown period displayed
- Staking history table

### 10. Leaderboard Page
- Time filter tabs: This Week, This Month, All Time
- Ranking table: Rank, Avatar, Username, Level Badge, Tasks Completed, TaskCoins Earned, Reputation Score, Platforms
- Top 3 highlighted with gold/silver/bronze styling
- "Your Rank" sticky bar at bottom showing the logged-in user's position
- Separate tabs for: Most Tasks, Most Earned, Best Reputation, Most Referrals

### 11. Referral Page (Chiller)
- Unique referral link with copy button
- Share buttons: X, Telegram, WhatsApp, Email
- Stats: Total Referrals, Active Referrals, Total Referral Earnings
- Referral list table: Username, Sign-up Date, Tasks Completed, Your Earnings from Them
- Explainer: "Earn 5% of everything your referrals earn — forever. Paid from the platform fee, not from their earnings."

### 12. University Page
- Course grid with cards: thumbnail, title, difficulty badge (Beginner/Intermediate/Advanced), lesson count, estimated time
- Courses (placeholder content, will be filled later):
  - "How to Grow Your X (Twitter) Account from 0 to 10K"
  - "Reddit Karma Building: The Complete Guide"
  - "YouTube Channel Growth for Beginners"
  - "Maximize Your TaskCoins Earnings"
  - "Crypto Basics: Wallets, Tokens, and DeFi"
  - "How to Use MetaMask Like a Pro"
- Click course → Course page with video embed area + text content + "Mark as Complete" button
- Progress tracking: courses completed shown on profile

### 13. Services Page
- Service cards in a grid:
  - **PR Writing** — "Professional crypto press releases for your project" — Starting at 5,000 TASK
  - **YouTuber Promotion** — "Get featured by crypto YouTubers with 50K-200K subscribers" — Starting at 10,000 TASK
  - **Distribution on Outlets** — "Get published on CoinDesk, CoinTelegraph, and major outlets" — Starting at 25,000 TASK
  - **dApp Creation** — "Smart contract + frontend development for your Web3 project" — Starting at 50,000 TASK
  - **Token Launch** — "ERC-20/BEP-20 creation + Uniswap listing assistance" — Starting at 30,000 TASK
  - **NFT Development** — "Collection creation, minting page, marketplace listing" — Starting at 20,000 TASK
  - **Smart Contract Audit** — "Security audit for your existing contracts" — Starting at 15,000 TASK
  - **Web3 Consulting** — "Tokenomics, GTM strategy, community building advisory" — Starting at 10,000 TASK
- Each card has "Request Quote" button → opens a form modal: name, email, project URL, budget, description, submit

### 14. Blog Page
- Standard blog layout: featured post hero at top, grid of recent posts below
- Categories: News, Updates, Partnerships, Guides, Community
- Each post card: featured image, title, excerpt, date, category badge, read time
- Individual blog post page: hero image, title, date, author, content area, share buttons, related posts
- Placeholder: 3 dummy blog posts about TaskCoins launch

### 15. Whitepaper Page
- Clean, document-style layout (like a real whitepaper reading experience)
- Table of contents sidebar (sticky on desktop):
  1. Abstract
  2. Problem Statement
  3. The TaskCoins Solution
  4. Platform Architecture
  5. Token Utility
  6. Tokenomics (supply: 590,000,000 TASK)
  7. Allocation (pie chart: 30% Liquidity, 25% Treasury, 15% Team, 10% Airdrop, 10% Marketing, 10% Staking)
  8. Platform Fee Model (20% off-chain cut — diagram)
  9. Burn Mechanism (5% quarterly burn)
  10. Staking Model
  11. Governance Roadmap
  12. Team
  13. Legal Disclaimer
- "Download PDF" button in header
- Placeholder text for each section — will be filled with real content later

### 16. Roadmap Page
- Vertical timeline design (alternating left/right on desktop, single column on mobile)
- Phases with status indicators (completed = green, in progress = blue pulse, upcoming = gray):
  - Phase 1 — Launch (Month 1): Token deploy, Uniswap listing, Platform beta, First 300 Chillers
  - Phase 2 — Growth (Month 2-3): CEX listing, University launch, 1,000 Chillers, Anti-cheat v1
  - Phase 3 — Scale (Month 4-6): Mobile PWA, Services marketplace, Staking launch, 5,000 Chillers
  - Phase 4 — Expand (Month 6-12): Multi-language, Advertiser API, Governance voting, 20,000 Chillers
  - Phase 5 — Ecosystem (Year 2): Native mobile app, Additional CEX listings, DAO governance, 100,000 Chillers

### 17. Proof Gallery Page
- Public page (no login required) showing recent completed tasks
- Masonry grid of proof cards: screenshot thumbnail, platform icon, task type, Chiller username, date
- Filter by platform: All, X, Reddit, CMC, Binance Square, YouTube, Telegram
- Purpose: shows potential advertisers that tasks are REAL and verified

### 18. Advertiser Marketplace Page
- Browse Chiller profiles before creating targeted campaigns
- Filter: platform expertise, level, reputation score, follower count range
- Chiller cards: avatar, username, level badge, reputation score, platforms (icons), tasks completed, "Hire Directly" button
- "Hire Directly" → creates a private task offer to that specific Chiller

### 19. Admin Panel (Internal — Not Public)
- Accessible only by admin accounts
- User management: view all users, ban/suspend, adjust levels manually
- Campaign management: view all campaigns, pause/remove if needed
- Task moderation: review flagged proofs, resolve disputes
- Financial overview: total platform fees collected, treasury balance, burn history
- Analytics: daily active users, tasks per day, new signups chart, revenue chart
- Content management: blog post editor, university course editor

---

## Key UI Components

### Navigation (Header)
- Logo (left)
- Menu items: Home, Task Board, University, Services, Blog, Whitepaper, Roadmap
- Right side: "Connect Wallet" button (if not logged in) OR wallet address + balance (if connected)
- User avatar dropdown: Dashboard, Profile, Settings, Logout
- Mobile: hamburger menu

### Task Card Component
```
┌─────────────────────────────────┐
│ [X icon]  Post about ProjectX   │
│                                 │
│ Reward: 150 TASK                │
│ Level required: Silver+         │
│ Time remaining: 18h 32m        │
│                                 │
│ [████████░░] 67/100 completed   │
│                                 │
│ [Claim Task]                    │
└─────────────────────────────────┘
```

### Level Badge Component
- Bronze: copper colored badge
- Silver: silver metallic badge
- Gold: gold metallic badge
- Diamond: blue diamond badge with subtle sparkle
- Legend: purple/rainbow gradient badge with glow effect

### Reputation Gauge
- Circular progress indicator (0-100)
- Color: red (0-30) → orange (31-50) → yellow (51-70) → green (71-90) → blue glow (91-100)
- Number displayed in center

---

## Database Tables (Supabase)

### users
- id, email, wallet_address, account_type (advertiser/chiller), display_name, avatar_url, level (1-5), reputation_score (0-100), total_earned, total_spent, tasks_completed, referral_code, referred_by, account_created_at, last_active_at, is_banned

### campaigns
- id, advertiser_id (FK users), title, description, content_text, content_image_url, platforms (array), reward_per_task, total_tasks, tasks_completed, tasks_remaining, min_chiller_level, min_reputation, status (active/paused/completed/expired), created_at, expires_at

### tasks
- id, campaign_id (FK campaigns), chiller_id (FK users), status (available/claimed/submitted/approved/rejected), proof_screenshot_url, proof_link, claimed_at, submitted_at, reviewed_at, rejection_reason

### wallets
- id, user_id (FK users), balance, total_deposited, total_withdrawn, total_earned, total_spent, total_staked, withdrawal_tier (new/warmed/trusted/vip), first_task_completed_at

### transactions
- id, user_id (FK users), type (deposit/withdrawal/earned/spent/staked/unstaked/referral_bonus/platform_fee), amount, status (pending/completed/failed), tx_hash (for on-chain), created_at

### stakes
- id, user_id (FK users), amount, tier_unlocked, staked_at, unstake_requested_at, unstake_available_at

### referrals
- id, referrer_id (FK users), referred_id (FK users), total_earned_from_referral, created_at

### blog_posts
- id, title, slug, excerpt, content, featured_image_url, category, author, published_at, is_published

### courses
- id, title, description, difficulty, thumbnail_url, lessons_count, estimated_minutes, content, order_index

### service_requests
- id, user_id (FK users), service_type, name, email, project_url, budget, description, status (new/in_progress/completed), created_at

---

## Important Business Logic

1. **20% Platform Fee:** When advertiser creates campaign for 1,000 TASK, show breakdown: "800 TASK to workers + 200 TASK platform fee." Deduct full 1,000 from advertiser balance. Workers receive from the 800 pool only.

2. **Withdrawal Warming:** New accounts cannot withdraw for 30 days. Show countdown timer and progress bar. After 30 days, unlock based on reputation tier.

3. **Referral System:** 5% of referred user's earnings credited to referrer. Paid from platform's 20% cut, NOT deducted from the worker's earnings. Calculate and credit in real-time when referred user's task is approved.

4. **Level Progression:** Bronze (0 tasks) → Silver (50) → Gold (200) → Diamond (500) → Legend (1000). Show progress bar with tasks remaining to next level.

5. **Staking Lock:** When user stakes, tokens are locked. Unstaking has 7-day cooldown. During cooldown, benefits remain active but tokens cannot be withdrawn.

6. **Task Claiming:** Chiller can only have 3 active (claimed but not submitted) tasks at a time. 24-hour deadline to submit proof after claiming. Auto-release uncompleted tasks back to the pool.

---

## Mobile Responsiveness

- Mobile-first design — most Chillers will use phones
- Bottom navigation bar on mobile (Home, Tasks, Wallet, Profile)
- Task cards stack vertically on mobile
- Swipe gestures for task approval (advertiser reviewing proofs)
- All forms optimized for mobile input
- Camera access for screenshot upload on mobile

---

## Placeholder Data

Pre-populate with realistic demo data so the platform looks alive:
- 5 sample campaigns across different platforms
- 20 sample task submissions with proof screenshots (placeholder images)
- 10 sample Chiller profiles at various levels
- 3 sample blog posts about TaskCoins
- Leaderboard with 50 sample users
- Transaction history with 30 sample entries

---

Build everything listed above. Make it production-ready, mobile-first, dark mode by default. The platform should feel like a premium crypto product — clean, fast, trustworthy.
