Build a complete crypto micro-task platform called TaskCoins. This is a platform where advertisers pay workers ("Chillers") in a crypto token called TASK to post content on their social media accounts. Build EVERY page listed below in full. Do NOT skip any page. Do NOT defer anything to "future iterations." Build it all now.

Design: Dark mode crypto-native aesthetic like dYdX or Blur. Background #0A0E17, card backgrounds #111827 with subtle glass-morphism (backdrop-blur, border border-white/10). Primary accent #388EFF (electric blue). Success green #09CE84. Warning orange #FFA01E. Danger red #FC564E. Text white #FFFFFF primary, #9CA3AF secondary. Font: Satoshi for headings (bold, clean), Inter for body text. Subtle blue glow on primary CTA buttons. Rounded corners on all cards (16px). Mobile-first responsive design — most users will be on phones.

Tech: React + TypeScript + Tailwind CSS + Supabase (auth + database + storage) + shadcn/ui components. Use React Router for navigation.

---

PAGE 1: LANDING PAGE (route: /)

Top navigation bar (sticky, dark, blur background):
- Left: TaskCoins logo (text logo "TaskCoins" in Satoshi bold white, with a small blue coin icon next to it)
- Center menu links: Home, Task Board, University, Services, Blog, Whitepaper, Roadmap
- Right: "Connect Wallet" button (blue outline) and "Sign Up" button (blue filled)
- Mobile: hamburger menu

Hero section (full viewport height, centered):
- Large heading: "Complete Tasks. Earn TaskCoins." in Satoshi bold, 56px desktop / 36px mobile
- Subheading: "Get paid in crypto to post on social media. Join 1,200+ Chillers earning daily." in Inter, #9CA3AF, 20px
- Two CTA buttons side by side: "Start Earning" (blue filled, large) and "Launch a Campaign" (blue outline, large)
- Below buttons: three animated stat counters in a row: "12,847 Tasks Completed" | "2,450,000 TASK Distributed" | "1,234 Active Chillers" — numbers should have a counting-up animation on page load
- Background: subtle gradient from #0A0E17 to #111827, optional subtle grid pattern or floating particle effect

How It Works section:
- Section heading: "How It Works" centered
- Three cards in a row (stacked on mobile), each with:
  - Card 1: Icon (user-plus), number "1", title "Sign Up", description "Create your free account as a Chiller or Advertiser. Connect your wallet or use email."
  - Card 2: Icon (clipboard-check), number "2", title "Complete Tasks", description "Browse available tasks, post content on your social media accounts, and submit proof."
  - Card 3: Icon (coins), number "3", title "Earn Crypto", description "Get paid in TaskCoins for every approved task. Hold for 100x or withdraw to your wallet."
- Cards have glass-morphism styling with blue icon accents

For Advertisers section:
- Left side: heading "Get 300 Real People Posting About Your Project in 24 Hours", description paragraph explaining how advertisers create campaigns, set rewards, and get verified proof of every post. Mention platforms: X, Reddit, CoinMarketCap, Binance Square, YouTube, Telegram.
- Right side: mockup card showing a sample campaign: "Promote $TOKEN Launch on X" — 150 TASK per post — 67/100 tasks completed — progress bar
- CTA button: "Launch a Campaign"

For Chillers section:
- Right side: heading "Earn Crypto by Posting on Social Media — No Investment Needed", description explaining how Chillers browse tasks, post from their own accounts, submit screenshots as proof, and earn TaskCoins.
- Left side: mockup card showing earnings dashboard preview: balance "12,450 TASK", level "Gold", tasks completed "234", reputation "87/100"
- CTA button: "Start Earning"

Trusted By section:
- Horizontal logo bar with placeholder gray logos: "CoinDesk", "CoinTelegraph", "CoinMarketCap", "Uniswap", "MEXC" — use text placeholders styled as logos in gray

Testimonials section:
- Three testimonial cards in a row:
  - Card 1: Avatar placeholder, "Ahmed K.", "Gold Chiller", "I've earned over 50,000 TASK in my first month. This platform changed my life.", 5 stars
  - Card 2: Avatar placeholder, "Sarah M.", "Advertiser", "We got 280 verified posts about our token launch in under 12 hours. Insane ROI.", 5 stars
  - Card 3: Avatar placeholder, "Carlos R.", "Diamond Chiller", "Better than any freelance platform. I earn while growing my own social accounts.", 5 stars

Footer:
- 4 columns: Platform (Home, Task Board, Leaderboard, Proof Gallery), Resources (University, Blog, Whitepaper, Roadmap), Services (PR Writing, YouTuber Promo, Distribution, dApp Creation), Legal (Terms, Privacy, Contact)
- Bottom bar: "© 2026 TaskCoins. All rights reserved." and social icons (X, Telegram, Instagram, Discord)

---

PAGE 2: SIGN UP / LOGIN (route: /auth)

- Centered card on dark background
- Toggle tabs at top: "Chiller" and "Advertiser" — clicking each changes the form subtitle
- Chiller selected: subtitle "Start earning crypto by completing social media tasks"
- Advertiser selected: subtitle "Get your project promoted by thousands of real users"
- Form fields: Display Name, Email, Password, Confirm Password
- Optional field: "Referral Code" (pre-filled if URL has ?ref= parameter)
- Checkbox: "I agree to the Terms of Service and Privacy Policy"
- "Sign Up" button (blue, full width)
- Divider: "or"
- "Connect Wallet" button (outline, full width, MetaMask icon)
- "Sign in with Google" button (outline, full width, Google icon)
- Bottom text: "Already have an account? Log In" — links to login view
- Login view: Email + Password fields + "Log In" button + "Forgot Password?" link
- Use Supabase Auth for email/password signup and login (make it functional)

---

PAGE 3: CHILLER DASHBOARD (route: /dashboard/chiller)

Sidebar navigation (collapsible on mobile, becomes bottom tab bar):
- Logo at top
- Menu items with icons: Dashboard, Task Board, My Tasks, Wallet, Staking, Leaderboard, Referrals, University, Profile, Settings
- Active item highlighted with blue background
- Bottom: user avatar + display name + level badge

Main content area:

Top row — 5 stat cards in a horizontal row (scrollable on mobile):
- Card 1: "Available Balance" — "8,450 TASK" — green icon (wallet)
- Card 2: "Total Earned" — "24,200 TASK" — blue icon (trending-up)
- Card 3: "Tasks Completed" — "186" — purple icon (check-circle)
- Card 4: "Current Level" — "Gold" with gold badge icon — progress bar below showing "186/200 tasks to Diamond"
- Card 5: "Reputation Score" — circular gauge showing "87/100" — green color

Earnings Chart section:
- Line chart showing earnings over last 30 days (use Recharts)
- X-axis: dates, Y-axis: TASK earned
- Use sample data: gradual uptrend with some variation
- Toggle: 7 days / 30 days / 90 days

Available Tasks Preview section:
- Heading: "Top Paying Tasks" with "View All" link to /tasks
- 5 task cards in a list:
  - Each card shows: platform icon (X, Reddit, etc.), task title, reward amount in TASK, required level badge, time remaining, progress bar (completed/total)
  - Sample tasks:
    1. X icon — "Share TokenX Launch Announcement" — 200 TASK — Gold+ — 18h left — 45/100
    2. Reddit icon — "Post in r/cryptocurrency about DeFi Protocol" — 150 TASK — Silver+ — 23h left — 12/50
    3. CMC icon — "Community post about $TASK utility" — 100 TASK — Bronze+ — 12h left — 89/100
    4. Binance Square icon — "Write about AI crypto trends" — 175 TASK — Gold+ — 20h left — 23/75
    5. YouTube icon — "Comment on crypto review video" — 75 TASK — Bronze+ — 8h left — 67/80
  - Each card has a "Claim" button on the right

Recent Activity feed:
- List of recent events: "Task #234 approved — +150 TASK", "Referral bonus — +12 TASK", "Level up! You reached Gold", "Task #231 approved — +100 TASK"
- Each with timestamp and icon

---

PAGE 4: TASK BOARD (route: /tasks)

Top bar:
- Heading: "Task Board"
- View toggle: Grid view / List view icons
- Search bar: "Search tasks..."

Filter sidebar (left on desktop, slide-out sheet on mobile):
- Platform filter (checkboxes with icons): X (Twitter), Reddit, CoinMarketCap, Binance Square, YouTube, Telegram, All
- Reward range: slider from 0 to 500 TASK
- Minimum level required: dropdown (Any, Bronze, Silver, Gold, Diamond)
- Sort by: dropdown (Newest, Highest Reward, Ending Soon, Most Available)
- "Apply Filters" button and "Reset" link

Task cards grid (3 columns desktop, 2 tablet, 1 mobile):
Each card (glass-morphism, dark card):
- Top: platform icon + platform name badge (e.g., blue "X" badge)
- Title: task name (bold, white)
- Description: 2 lines max, truncated with ellipsis
- Stats row: reward "200 TASK" in green | required level badge | time remaining with clock icon
- Progress bar: "67/100 completed" with percentage
- Bottom: "Claim Task" blue button (full width of card)

Pre-populate with 12 sample tasks across all 6 platforms with varied rewards (50-300 TASK), levels, and completion percentages.

Click on a task card → Task Detail modal or page:
- Full task title and description
- Platform with icon
- Advertiser name with avatar
- Reward: "200 TASK" large and green
- Required level and minimum reputation
- Specific instructions: "Copy the text below and post it on your X account with the provided image. Include all hashtags."
- Content to post: text area (read-only, with "Copy" button)
- Image to use: image preview (if provided by advertiser)
- Submit proof section: file upload area ("Upload screenshot of your post") + text input ("Paste the URL of your post")
- "Submit Proof" blue button
- "Cancel" outline button

---

PAGE 5: MY TASKS (route: /dashboard/chiller/my-tasks)

4 tabs: Active (3), Submitted (5), Approved (42), Rejected (2) — numbers in badges

Active tab:
- Cards showing claimed tasks with countdown timer "18h 32m remaining"
- "Submit Proof" button on each
- "Release Task" secondary button (returns task to pool)

Submitted tab:
- Cards showing submitted tasks with "Awaiting Review" yellow badge
- Shows submitted screenshot thumbnail and link
- "Submitted 2 hours ago" timestamp

Approved tab:
- Cards with green "Approved" badge and "+200 TASK" earned amount
- Shows proof screenshot and link as submitted

Rejected tab:
- Cards with red "Rejected" badge
- Shows rejection reason: "Screenshot does not match required content"
- "Resubmit" button if resubmission is allowed

Pre-populate each tab with sample data.

---

PAGE 6: ADVERTISER DASHBOARD (route: /dashboard/advertiser)

Sidebar navigation:
- Menu items: Dashboard, Create Campaign, My Campaigns, Review Proofs, Analytics, Wallet, Settings
- Active item highlighted blue

Main content:

Top row — 5 stat cards:
- "Total Spend" — "145,000 TASK" — blue
- "Active Campaigns" — "3" — green
- "Tasks Completed" — "847" — purple
- "Posts Live" — "823" — green
- "Estimated Reach" — "1.2M" — orange

Active Campaigns section:
- 3 campaign cards:
  1. "Launch $TOKEN on X" — Active — 67/100 tasks done — progress bar — "Created 2 days ago"
  2. "Reddit AMA Promotion" — Active — 23/50 tasks done — "Created 5 days ago"
  3. "CMC Community Push" — Completed — 100/100 tasks done — green checkmark — "Completed yesterday"
- Each card: click to view details

Recent Proof Submissions:
- List of 5 recent submissions awaiting review with Chiller avatar, username, task name, "Review" button
- Quick approve/reject buttons visible

Quick action: "Create New Campaign" large blue CTA button

---

PAGE 7: CREATE CAMPAIGN (route: /dashboard/advertiser/create)

Step-by-step wizard with progress bar at top showing steps 1-5:

Step 1 — Choose Platforms:
- Heading: "Where do you want your content posted?"
- 6 platform cards in a grid (2x3), each with large icon, platform name, and description:
  - X (Twitter) — "Reach crypto Twitter"
  - Reddit — "Engage subreddit communities"
  - CoinMarketCap — "Post in coin communities"
  - Binance Square — "Binance's social platform"
  - YouTube — "Comments on crypto videos"
  - Telegram — "Share in Telegram groups"
- Multi-select: clicking a card toggles blue border highlight and checkmark
- "Next" button

Step 2 — Create Content:
- Heading: "What should Chillers post?"
- Large text area: "Write the content for Chillers to copy and post" (placeholder text showing example post)
- Image upload: drag-and-drop area with "Upload an image for the post (optional)" — shows preview after upload
- Link field: "Include a link in the post (optional)"
- Instructions text area: "Any specific instructions for Chillers? (optional)" — placeholder: "Make sure to include all hashtags and tag @projecthandle"
- "Next" button, "Back" button

Step 3 — Set Requirements:
- Heading: "Who can complete your tasks?"
- Minimum Chiller Level: dropdown with options Any Level, Silver+, Gold+, Diamond+ — each with description of what it means
- Minimum Reputation Score: slider 0-100, default 0, shows current value
- Task deadline: "How long do Chillers have to complete?" dropdown: 12 hours, 24 hours, 48 hours, 72 hours
- "Next" button, "Back" button

Step 4 — Set Budget:
- Heading: "Set your campaign budget"
- "Reward per task": input field with TASK suffix, default 100
- "Number of tasks": input field, default 50
- Live calculation box below:
  - "Worker rewards: 5,000 TASK (100 × 50)"
  - "Platform fee (20%): 1,250 TASK"
  - "Total campaign cost: 6,250 TASK" — large, bold
  - "Your balance: 50,000 TASK" — shows if sufficient (green) or insufficient (red)
- "Next" button, "Back" button

Step 5 — Review & Launch:
- Heading: "Review Your Campaign"
- Summary card showing all selections: platforms (icons), content preview, requirements, budget breakdown
- Checkbox: "I confirm this campaign follows TaskCoins guidelines"
- "Launch Campaign" large blue button with rocket icon
- "Back" button
- On launch: success modal with confetti animation, "Your campaign is now live! Chillers will start completing tasks immediately."

---

PAGE 8: REVIEW PROOFS (route: /dashboard/advertiser/review)

- Heading: "Review Proof Submissions"
- Filter: dropdown to filter by campaign
- Queue of proof cards (stacked list):
  Each card shows:
  - Left: Chiller avatar, username, level badge, reputation score
  - Center: screenshot thumbnail (click to expand in lightbox/modal showing full image), posted link (clickable, opens in new tab)
  - Right: two large buttons — "Approve" (green with check icon) and "Reject" (red with X icon)
  - If reject clicked: text input appears "Reason for rejection" + "Confirm Reject" button
  - Timestamp: "Submitted 2 hours ago"
  - Platform icon badge
- Pre-populate with 8 sample submissions with placeholder screenshots
- Top stats bar: "12 Pending Review" | "847 Approved" | "23 Rejected"

---

PAGE 9: WALLET (route: /dashboard/wallet)

Large balance display at top center:
- Token icon + "8,450 TASK" in large text (48px)
- USD equivalent below in gray: "≈ $845.00"
- Two action buttons below: "Deposit" and "Withdraw"

Two tabs: Deposit | Withdraw

Deposit tab:
- "Connect your wallet to deposit TASK tokens"
- "Connect Wallet" button (MetaMask icon) — mock connection
- After "connected": shows wallet address truncated, input field "Amount to deposit" with MAX button, "Deposit" blue button
- Info text: "Deposits are confirmed after 12 block confirmations (~3 minutes)"

Withdraw tab:
- Shows current withdrawal tier with visual progress:
  - If new account: large yellow banner "Withdrawals unlock after 30 days of activity" with countdown timer showing "22 days 14 hours remaining"
  - Progress bar showing account warming: 0-30 days (locked) → 30-60 days (monthly) → 60+ days (bi-weekly) → VIP (weekly)
  - Current tier highlighted
- Withdrawal rules displayed in a clean table:
  - New (0-30 days): No withdrawals
  - Warmed (30-60 days): Once per month, minimum 500 TASK
  - Trusted (60+ days, reputation 70+): Bi-weekly, minimum 200 TASK
  - VIP (Diamond+, reputation 90+): Weekly, minimum 100 TASK
- If eligible: input field "Amount to withdraw" + wallet address field + "Request Withdrawal" button
- Blue banner at bottom: "TaskCoins is designed for long-term growth. The longer you hold, the more your earnings are worth. Hold for 100x."

Transaction History section below:
- Table with columns: Date, Type (with colored badges: green "Earned", blue "Deposited", orange "Withdrawn", purple "Staked", yellow "Referral Bonus"), Amount (+ green or - red), Status (Completed/Pending/Failed badges)
- Pre-populate with 20 sample transactions
- Pagination at bottom

---

PAGE 10: STAKING (route: /dashboard/chiller/staking)

Hero: "Stake TaskCoins — Unlock Premium Rewards" with blue glow effect

Current staking status card:
- "Currently Staked: 5,000 TASK"
- "Current Tier: Tier 2"
- "Active Benefit: 5% bonus on all earnings"
- If nothing staked: "You haven't staked any TaskCoins yet. Stake now to unlock premium benefits."

4 tier cards in a row (scrollable on mobile):
- Tier 1: "1,000 TASK" — star icon — "Access premium tasks" — if unlocked: blue glow border, if locked: dimmed with lock icon
- Tier 2: "5,000 TASK" — trending-up icon — "5% bonus on all earnings" — highlighted as current
- Tier 3: "10,000 TASK" — lightning icon — "10% bonus + early access" — locked, dimmed
- Tier 4: "50,000 TASK" — crown icon — "VIP + direct advertiser offers" — locked, dimmed

Stake section:
- Input: "Amount to stake" with TASK label and "MAX" button
- "Available balance: 8,450 TASK" shown below input
- "Stake Now" blue button

Unstake section:
- Input: "Amount to unstake"
- Warning text in orange: "Unstaking has a 7-day cooldown. Your benefits remain active during the cooldown period."
- "Request Unstake" outline button

Staking history table:
- Date, Action (Staked/Unstaked), Amount, Status
- Pre-populate with 5 entries

---

PAGE 11: LEADERBOARD (route: /leaderboard)

Hero: "Top Chillers — Compete, Climb, Earn" centered

Time filter tabs: This Week | This Month | All Time (default: This Month)
Category tabs: Most Tasks | Most Earned | Best Reputation | Most Referrals

Rankings table (full width):
- Columns: Rank #, Avatar, Username, Level (badge), Tasks Completed, TASK Earned, Reputation, Platforms (small icons)
- Row 1: gold background tint, large rank "#1" — "CryptoKing" — Legend badge — 1,247 tasks — 89,400 TASK — 98 — X/Reddit/CMC icons
- Row 2: silver background tint — "#2"
- Row 3: bronze background tint — "#3"
- Rows 4-50: normal dark styling
- Pre-populate with 50 users with varied data

Sticky bar at bottom of viewport:
- "Your Rank: #47 — Complete 14 more tasks to reach #40" with progress indicator
- Blue background, fixed to bottom

---

PAGE 12: REFERRAL (route: /dashboard/chiller/referrals)

Hero: "Invite Friends. Earn 5% of Everything They Make — Forever." white heading, blue "Forever"

Referral link box:
- Large display: "https://taskcoins.io/ref/ABC123XYZ" in a bordered box
- "Copy Link" blue button (shows "Copied!" for 2 seconds after click)
- Share buttons row: X icon, Telegram icon, WhatsApp icon, Email icon — each opens share intent

Stats cards (3 in a row):
- "Total Referrals" — "12"
- "Active Referrals" — "8" (completed at least 1 task)
- "Total Referral Earnings" — "3,240 TASK"

Referral table:
- Columns: Avatar, Username, Signed Up, Their Tasks Completed, Your Earnings From Them
- Pre-populate with 8 referrals at various activity levels
- Some active (green dot), some inactive (gray dot)

How It Works section at bottom:
- 3 steps with icons:
  1. Share icon — "Share your unique referral link"
  2. User-check icon — "They sign up and start completing tasks"
  3. Coins icon — "You earn 5% of their earnings — forever (paid from platform fee, NOT from their pay)"

---

PAGE 13: UNIVERSITY (route: /university)

Hero: "TaskCoins University" heading, "Learn, Grow, Earn More" subheading

Course grid (3 columns desktop, 1 mobile):
6 course cards, each with:
- Thumbnail placeholder (gradient background with topic icon)
- Title
- Difficulty badge: green "Beginner", orange "Intermediate", red "Advanced"
- Stats: "8 lessons • 45 min"
- "Start Course" blue button

Courses:
1. "How to Grow Your X Account from 0 to 10K" — Beginner — 8 lessons — 45 min — thumbnail: X logo on blue gradient
2. "Reddit Karma Building: The Complete Guide" — Beginner — 6 lessons — 30 min — Reddit logo on orange gradient
3. "YouTube Channel Growth for Beginners" — Intermediate — 10 lessons — 60 min — YouTube logo on red gradient
4. "Maximize Your TaskCoins Earnings" — Beginner — 5 lessons — 20 min — TaskCoins logo on blue gradient
5. "Crypto Basics: Wallets, Tokens, and DeFi" — Beginner — 7 lessons — 35 min — wallet icon on purple gradient
6. "How to Use MetaMask Like a Pro" — Beginner — 4 lessons — 15 min — MetaMask fox on orange gradient

Click a course → Course detail page:
- Course header: title, difficulty, "4/8 lessons completed" progress bar
- Left sidebar: lesson list with checkmarks for completed, highlight current
- Main area: lesson content (placeholder paragraphs), video embed placeholder (gray box with play icon), "Mark as Complete" green button, "Next Lesson" blue button

---

PAGE 14: SERVICES (route: /services)

Hero: "Web3 Services — Built by the Team Behind Pepeto" heading, "End-to-end crypto solutions from a team that's done it." subheading

Service cards (2 columns desktop, 1 mobile):
Each card has: icon, title, description, starting price, "Request Quote" button

1. Document icon — "PR Writing" — "Professional crypto press releases distributed to major outlets" — "From 5,000 TASK"
2. Play icon — "YouTuber Promotion" — "Get featured by crypto YouTubers with 50K-200K subscribers" — "From 10,000 TASK"
3. Newspaper icon — "Distribution on Outlets" — "Get published on CoinDesk, CoinTelegraph, and major crypto news sites" — "From 25,000 TASK"
4. Code icon — "dApp Creation" — "Smart contract development + frontend for your Web3 project" — "From 50,000 TASK"
5. Rocket icon — "Token Launch" — "ERC-20/BEP-20 token creation + Uniswap listing assistance" — "From 30,000 TASK"
6. Image icon — "NFT Development" — "Collection creation, minting page, marketplace listing" — "From 20,000 TASK"
7. Shield icon — "Smart Contract Audit" — "Security audit for your existing smart contracts" — "From 15,000 TASK"
8. Lightbulb icon — "Web3 Consulting" — "Tokenomics, go-to-market strategy, community building advisory" — "From 10,000 TASK"

"Request Quote" opens modal form: Name, Email, Project URL, Budget dropdown (5K-10K / 10K-25K / 25K-50K / 50K+ TASK), Description textarea, "Submit Request" button

Why Choose Us section:
- 3 cards: "Proven Team" (Pepeto track record), "End-to-End" (from token creation to marketing), "Results-Driven" (real metrics, not empty promises)

---

PAGE 15: BLOG (route: /blog)

Featured post hero: large card at top with gradient overlay on placeholder image, title, excerpt, date, "Read More" button

Post grid below (3 columns desktop, 1 mobile):
- Category filter bar: All, News, Updates, Partnerships, Guides, Community

3 placeholder posts:
1. "TaskCoins Launches: The Future of Social Media Earning" — News — March 8, 2026 — 5 min read — placeholder image
2. "How 300 Chillers Earned Their First TaskCoins" — Community — March 7, 2026 — 3 min read
3. "TaskCoins Tokenomics Explained: Why We Built a Utility Token" — Guides — March 6, 2026 — 7 min read

Each card: image, title, excerpt (2 lines), date, category badge, read time

Individual post page (route: /blog/:slug):
- Hero image, title (large), author avatar + name + date, content area with 5 placeholder paragraphs, share buttons (X, Telegram, copy link), "Related Posts" section with 2 cards at bottom

---

PAGE 16: WHITEPAPER (route: /whitepaper)

Clean document reading layout on dark background.

Sticky sidebar table of contents (desktop, collapses to dropdown on mobile):
1. Abstract
2. Problem Statement
3. The TaskCoins Solution
4. Platform Architecture
5. Token Utility
6. Tokenomics
7. Token Allocation
8. Platform Fee Model
9. Burn Mechanism
10. Staking Model
11. Governance Roadmap
12. Team
13. Legal Disclaimer

Clicking a TOC item smooth-scrolls to that section.

"Download PDF" button in the top right corner.

Content for each section (write 3-5 sentences per section as placeholder):

Section 6 — Tokenomics: prominently display "Total Supply: 590,000,000 TASK" in a highlighted box. Network: Ethereum ERC-20. No on-chain tax.

Section 7 — Token Allocation: animated donut chart with: Uniswap Liquidity 30% (blue), Platform Treasury 25% (green), Team 15% (orange, "12-month vesting"), Community Airdrop 10% (purple), Marketing 10% (yellow), Staking Rewards 10% (cyan). Legend next to chart with token amounts.

Section 8 — Platform Fee Model: visual flow diagram showing: "Advertiser pays 1,000 TASK → 800 TASK to Workers (80%) → 200 TASK to Platform (20%)" with arrows and boxes.

Section 9 — Burn Mechanism: "5% of platform fees burned quarterly" with example: "Q1 fees: 1,000,000 TASK → 50,000 TASK burned" and fire icon.

Typography: large section headings in Satoshi bold, body in Inter, generous line height (1.8) for readability.

---

PAGE 17: ROADMAP (route: /roadmap)

Vertical timeline design. On desktop: alternating left/right cards connected by a vertical line with dots. On mobile: single column.

Status dot indicators: completed = green dot + checkmark, in progress = blue pulsing/glowing dot, upcoming = gray dot.

Phase 1 — Launch (Month 1) — Status: IN PROGRESS (blue pulse):
- Token deployment on Ethereum
- Uniswap liquidity pool live
- Platform beta launch
- First 300 Chillers onboarded
- CoinMarketCap + CoinGecko listing applications

Phase 2 — Growth (Month 2-3) — Status: UPCOMING (gray):
- CEX listing (MEXC / LBank)
- University launch with first courses
- 1,000 active Chillers
- Anti-cheat verification system v1
- Advertiser onboarding campaign

Phase 3 — Scale (Month 4-6) — Status: UPCOMING:
- Mobile Progressive Web App
- Services marketplace live
- Staking system launch
- 5,000 active Chillers
- First quarterly token burn

Phase 4 — Expand (Month 6-12) — Status: UPCOMING:
- Multi-language support (Arabic, Spanish, Turkish, Indonesian, Russian, Portuguese)
- Advertiser API for programmatic campaigns
- Governance voting for token holders
- 20,000 active Chillers

Phase 5 — Ecosystem (Year 2) — Status: UPCOMING:
- Native mobile apps (iOS + Android)
- Additional CEX listings
- DAO governance
- 100,000 active Chillers
- Global expansion

Subtle scroll animation: timeline line fills in with blue color as user scrolls down.

---

PAGE 18: PROOF GALLERY (route: /proof-gallery)

Public page, no login required.

Hero: "Real Tasks. Real Posts. Real Proof." heading. Subheading: "Every task on TaskCoins is verified with screenshot proof and live links."

Filter bar: All Platforms | X | Reddit | CMC | Binance Square | YouTube | Telegram

Masonry grid of proof cards:
Each card:
- Screenshot thumbnail (placeholder image, click to expand in lightbox modal)
- Platform icon badge in top-right corner
- Bottom overlay: Chiller username, task type, date, green "Verified" badge with checkmark
- Hover: subtle scale up + blue glow border

Pre-populate with 20 cards using placeholder screenshots, varied platforms.

"Load More" button at bottom.

---

PAGE 19: ADVERTISER ANALYTICS (route: /dashboard/advertiser/analytics)

Top stat cards (4):
- Total Tasks Completed: 847
- Total Posts Live: 823
- Average Cost Per Post: 142 TASK
- Estimated Total Reach: 1.2M

Charts:
- Line chart: "Tasks Completed Over Time" — last 30 days — uptrend (Recharts)
- Bar chart: "Performance by Platform" — bars for X, Reddit, CMC, Binance Square, YouTube, Telegram with different colors
- Both charts have dark backgrounds matching the theme

Table: "Top Performing Chillers"
- Columns: Avatar, Username, Level, Tasks Completed (for this advertiser), Approval Rate, "Hire Directly" button
- 10 rows of sample data

---

PAGE 20: PROFILE (route: /dashboard/chiller/profile)

Header:
- Large avatar (placeholder, with "Edit" overlay on hover)
- Display name (editable)
- Level badge (Gold) with visual tier display
- Member since date
- "Edit Profile" button

Stats section (4 cards):
- Tasks Completed: 186
- Total Earned: 24,200 TASK
- Reputation Score: 87/100 (circular gauge)
- Referrals: 12

Platforms section:
- Connected platforms with icons: X (connected, green check), Reddit (connected), YouTube (not connected, "Connect" button)

Activity feed:
- Recent 10 activities: tasks completed, levels earned, badges unlocked

Badges section:
- Grid of achievement badges: "First Task", "100 Tasks", "Speed Demon" (10 tasks in 1 day), "Perfect Score" (100% approval rate for 50+ tasks), "Top Referrer" — earned badges in color, unearned grayed out with lock

---

SUPABASE DATABASE TABLES:

Create all these tables and connect them to the UI:

users: id (uuid, PK), email, password_hash, wallet_address, account_type (text: 'advertiser' or 'chiller'), display_name, avatar_url, level (int, default 1), reputation_score (int, default 50), total_earned (numeric, default 0), total_spent (numeric, default 0), tasks_completed (int, default 0), referral_code (text, unique), referred_by (text), created_at (timestamptz), last_active_at (timestamptz), is_banned (boolean, default false)

campaigns: id (uuid, PK), advertiser_id (FK users), title, description, content_text, content_image_url, platforms (text[]), reward_per_task (numeric), total_tasks (int), tasks_completed (int, default 0), tasks_remaining (int), min_chiller_level (int, default 1), min_reputation (int, default 0), status (text: 'active'/'paused'/'completed'/'expired'), created_at, expires_at

tasks: id (uuid, PK), campaign_id (FK campaigns), chiller_id (FK users), status (text: 'available'/'claimed'/'submitted'/'approved'/'rejected'), proof_screenshot_url, proof_link, claimed_at, submitted_at, reviewed_at, rejection_reason

wallets: id (uuid, PK), user_id (FK users), balance (numeric, default 0), total_deposited (numeric, default 0), total_withdrawn (numeric, default 0), total_earned (numeric, default 0), total_spent (numeric, default 0), total_staked (numeric, default 0), withdrawal_tier (text: 'new'/'warmed'/'trusted'/'vip'), first_task_completed_at (timestamptz)

transactions: id (uuid, PK), user_id (FK users), type (text: 'deposit'/'withdrawal'/'earned'/'spent'/'staked'/'unstaked'/'referral_bonus'/'platform_fee'), amount (numeric), status (text: 'pending'/'completed'/'failed'), tx_hash (text), created_at

stakes: id (uuid, PK), user_id (FK users), amount (numeric), tier_unlocked (int), staked_at, unstake_requested_at, unstake_available_at

referrals: id (uuid, PK), referrer_id (FK users), referred_id (FK users), total_earned_from_referral (numeric, default 0), created_at

blog_posts: id (uuid, PK), title, slug (unique), excerpt, content, featured_image_url, category, author, published_at, is_published (boolean)

service_requests: id (uuid, PK), user_id (FK users), service_type, name, email, project_url, budget, description, status (text: 'new'/'in_progress'/'completed'), created_at

Seed the database with realistic sample data so the platform looks alive when loaded.

---

IMPORTANT RULES:
- Build ALL 20 pages. Do not skip any.
- Do not defer anything to "future phases."
- Every page must have sample/placeholder data so it looks like a live platform.
- All navigation links must work and route to the correct pages.
- Supabase auth must work for signup/login.
- Mobile responsive on every page.
- Dark mode only — no light mode toggle needed.
- Use shadcn/ui components where possible (buttons, inputs, cards, tables, badges, tabs, modals, dropdowns, sliders, progress bars).
- Use Recharts for all charts.
- Use Lucide icons for all icons.
