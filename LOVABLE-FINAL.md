# TaskCoins.io — Complete Platform Visual Prototype

You are building a VISUAL PROTOTYPE of a crypto micro-task platform called TaskCoins. This is a design prototype to show a development team exactly how the platform should look and feel. Every page must be fully designed with realistic sample data. No backend, no database, no Supabase — just a beautiful, complete, fully navigable frontend prototype.

DO NOT skip any page. DO NOT defer anything. DO NOT simplify. Build every single page listed below with every element described. If you cut corners, the prototype is useless.

---

## DESIGN SYSTEM

**Theme:** Dark mode only. Crypto-native aesthetic inspired by dYdX, Blur, and Phantom wallet. Professional, premium, trustworthy.

**Colors:**
- Background: #0A0E17 (deep navy-black)
- Card backgrounds: #111827 with glass-morphism effect (backdrop-blur-xl, border: 1px solid rgba(255,255,255,0.08))
- Primary accent: #388EFF (electric blue) — used for CTAs, active states, highlights
- Success: #09CE84 (green) — used for earnings, approved, positive numbers
- Warning: #FFA01E (orange) — used for pending, caution
- Danger: #FC564E (red) — used for rejected, errors, negative
- Purple: #8B5CF6 — used for staking, premium features
- Text primary: #FFFFFF
- Text secondary: #9CA3AF
- Text muted: #6B7280
- Borders: rgba(255,255,255,0.08)
- Hover states: rgba(56,142,255,0.1) background tint

**Typography:**
- Headings: font-family 'Satoshi', sans-serif — bold weight, clean geometric look
- Body: font-family 'Inter', sans-serif — regular/medium weight
- Hero heading: 56px desktop, 36px mobile
- Section headings: 32px desktop, 24px mobile
- Card titles: 18px bold
- Body text: 16px, line-height 1.6
- Small text: 14px
- Stat numbers: 32px bold

**Components:**
- Cards: rounded-2xl (16px), bg-[#111827], border border-white/8, shadow-lg, hover:border-blue-500/30 transition
- Buttons primary: bg-[#388EFF] hover:bg-[#2B7AE0], text-white, rounded-xl, px-6 py-3, font-semibold, subtle blue glow shadow
- Buttons secondary: bg-transparent, border border-[#388EFF], text-[#388EFF], hover:bg-[#388EFF]/10
- Badges: rounded-full, px-3 py-1, text-xs font-medium
- Input fields: bg-[#0A0E17], border border-white/10, rounded-xl, text-white, focus:border-[#388EFF]
- Tables: bg-[#111827], rounded-xl, divide-y divide-white/5

**Icons:** Use Lucide icons throughout (Wallet, TrendingUp, CheckCircle, Star, Crown, Shield, Zap, Clock, Users, ArrowUpRight, Copy, Share2, Filter, Search, Menu, X, ChevronRight, Award, Flame, BarChart3, PieChart, Globe, BookOpen, Rocket, Code, Image, Lightbulb, FileText, Play, MessageSquare, Heart, Eye, ExternalLink)

---

## NAVIGATION (appears on every page)

**Desktop header (sticky, h-16, bg-[#0A0E17]/80 backdrop-blur-xl, border-b border-white/5):**
- Left: "TaskCoins" logo text in Satoshi bold 24px white, with a small blue circle/coin icon before the text
- Center: navigation links in Inter 15px #9CA3AF, hover:text-white — Home, Task Board, University, Services, Blog, Whitepaper, Roadmap, Leaderboard
- Right: "Connect Wallet" button (secondary/outline style, small wallet icon), "Sign Up" button (primary blue filled)
- When "logged in" (simulate with a toggle or default to logged-in state on dashboard pages): show wallet icon + "0x4f2...8a3" truncated address + user avatar dropdown

**Mobile header:**
- Left: TaskCoins logo
- Right: hamburger menu icon
- Menu opens as a full-screen dark overlay with all nav links stacked vertically + Sign Up / Connect Wallet buttons at bottom

**Dashboard pages get a sidebar (desktop) / bottom tab bar (mobile):**
- Sidebar: 250px wide, bg-[#111827], full height, logo at top, menu items with Lucide icons, active item has blue left border + blue text + blue/10 background
- Mobile bottom bar: 5 main tabs with icons — Home, Tasks, Wallet, Referrals, Profile

---

## PAGE 1: LANDING PAGE (/)

This is the first page anyone sees. It must be stunning. Every section described below must be built.

**Section 1 — Hero (full viewport height, centered content):**
- Background: gradient from #0A0E17 to #0F172A, with a subtle animated grid pattern or floating dots/particles
- Main heading: "Complete Tasks." on line 1, "Earn TaskCoins." on line 2 — Satoshi bold 56px (36px mobile), white, with "TaskCoins" highlighted in #388EFF
- Subheading below: "Get paid in crypto to post on social media. Join thousands of Chillers earning daily." — Inter 20px (16px mobile), #9CA3AF
- Two buttons side by side (stacked on mobile):
  - "Start Earning" — primary blue filled, large (px-8 py-4), with ArrowUpRight icon
  - "Launch a Campaign" — secondary outline, large, with Rocket icon
- Below the buttons, three stat counters in a row with animated count-up effect:
  - "12,847" with label "Tasks Completed" below — CheckCircle icon
  - "2,450,000" with label "TASK Distributed" below — Wallet icon
  - "1,234" with label "Active Chillers" below — Users icon
  - Each stat in a small glass card with icon, number in 32px bold white, label in 14px #9CA3AF

**Section 2 — How It Works (bg slightly different: #0F172A):**
- Section heading: "How It Works" — centered, Satoshi 32px
- Subheading: "Three simple steps to start earning crypto" — centered, #9CA3AF
- Three cards in a row (1 column on mobile), connected by a subtle dashed line or arrow between them:
  - Card 1: Large "01" in blue 48px, UserPlus icon in blue circle, title "Sign Up" in 20px bold, description "Create your free account as a Chiller or Advertiser. Connect your crypto wallet or sign up with email. It takes 30 seconds." in 15px #9CA3AF
  - Card 2: Large "02" in blue, ClipboardCheck icon, title "Complete Tasks", description "Browse available tasks on the Task Board. Pick a task, post the content on your social media account, and submit proof with a screenshot and link."
  - Card 3: Large "03" in blue, Coins icon, title "Earn TaskCoins", description "Every approved task earns you TaskCoins (TASK). Hold your tokens for long-term growth, stake them for bonus rewards, or withdraw to your wallet."
  - Cards have glass-morphism styling, hover:scale-105 transition

**Section 3 — For Advertisers:**
- Two-column layout (stacked on mobile)
- Left column:
  - Small blue badge: "FOR ADVERTISERS"
  - Heading: "Get 300 Real People Posting About Your Project in 24 Hours" — Satoshi 36px (28px mobile)
  - Paragraph: "Create a campaign, set your budget, and let our army of verified Chillers distribute your content across X, Reddit, CoinMarketCap Community, Binance Square, YouTube, and Telegram. Every post comes with screenshot proof and a live link. Real accounts. Real engagement. Real results." — Inter 16px, #9CA3AF, line-height 1.8
  - Bullet points with check icons:
    - "6 platforms: X, Reddit, CMC, Binance Square, YouTube, Telegram"
    - "Verified proof for every single post — screenshot + live link"
    - "Target Chillers by level, reputation, and platform expertise"
    - "Transparent pricing: 80% goes to workers, 20% platform fee"
  - "Launch a Campaign" blue button with ArrowUpRight icon
- Right column: a mockup campaign card showing:
  - Card title: "Promote $TOKEN Launch"
  - Platform badges: X, Reddit, CMC (small colored icons)
  - "Reward: 150 TASK per post" in green
  - Progress: "67/100 tasks completed" with progress bar
  - "Status: Active" green badge
  - "Budget: 15,000 TASK"
  - "Estimated Reach: 450K"
  - Two small proof thumbnails at bottom showing "screenshots submitted"

**Section 4 — For Chillers:**
- Two-column layout (reversed — content right, mockup left on desktop)
- Right column:
  - Small green badge: "FOR CHILLERS"
  - Heading: "Earn Crypto by Posting on Social Media — No Investment Needed" — Satoshi 36px
  - Paragraph: "Browse tasks on the Task Board, post content from your own social media accounts, submit a screenshot as proof, and earn TaskCoins for every approved task. The more tasks you complete, the higher your level, and the higher-paying tasks you unlock. Top Chillers earn thousands of TASK every month." — Inter 16px, #9CA3AF
  - Bullet points with check icons:
    - "No investment required — earn from day one"
    - "Level up: Bronze → Silver → Gold → Diamond → Legend"
    - "5% referral bonus — earn from everyone you invite, forever"
    - "Stake your earnings for bonus rewards and premium tasks"
  - "Start Earning" blue button
- Left column: a mockup Chiller dashboard card showing:
  - "Available Balance: 12,450 TASK" in large green numbers
  - "Level: Gold" with a gold badge icon
  - "Tasks Completed: 234"
  - "Reputation: 87/100" with a circular progress gauge
  - Small earnings chart (sparkline showing uptrend)
  - "Referral Earnings: 1,240 TASK"

**Section 5 — Platform Stats (full width, bg #111827):**
- Section heading: "The Numbers Speak" — centered
- Four large stat boxes in a row (2x2 on mobile):
  - "$2.4M" — "Total Value Distributed" — TrendingUp icon
  - "847" — "Active Campaigns" — BarChart3 icon
  - "156K" — "Posts Verified" — CheckCircle icon
  - "98.7%" — "Approval Rate" — Award icon
- Each box: glass card, icon in colored circle at top, large number in white 40px bold, label in #9CA3AF 14px

**Section 6 — Token Info:**
- Two-column layout
- Left:
  - Small purple badge: "TASKCOINS TOKEN"
  - Heading: "Powered by $TASK — An ERC-20 Utility Token" — Satoshi 36px
  - Paragraph: "TaskCoins (TASK) is the native currency of the platform. Advertisers buy TASK to fund campaigns. Chillers earn TASK for completing tasks. The token has real, built-in demand — every campaign requires purchasing TASK tokens. With quarterly token burns, staking rewards, and a growing user base, TASK is designed for long-term value growth." — Inter 16px, #9CA3AF
  - Key facts list:
    - "Total Supply: 590,000,000 TASK"
    - "Network: Ethereum (ERC-20)"
    - "No on-chain tax — zero transfer fees"
    - "5% of platform fees burned every quarter"
    - "Staking available for bonus rewards"
  - Two buttons: "Read Whitepaper" (secondary), "Buy on Uniswap" (primary)
- Right: Token allocation donut chart showing:
  - Uniswap Liquidity 30% (blue)
  - Platform Treasury 25% (green)
  - Team 15% (orange) — "12-month vesting"
  - Community Airdrop 10% (purple)
  - Marketing 10% (yellow)
  - Staking Rewards 10% (cyan)
  - Legend below the chart with color dots + label + percentage + token amount

**Section 7 — Trusted By / Press:**
- Horizontal logo bar, centered
- "As Featured In" small heading above
- Logos (use text styled as logos in gray #4B5563, each in a subtle bordered box): CoinDesk, CoinTelegraph, CoinMarketCap, Bitcoin Magazine, Uniswap, MEXC
- Logos should be grayscale, hover:white transition

**Section 8 — Testimonials:**
- Section heading: "What Our Community Says" — centered
- Three testimonial cards in a row (scroll on mobile):
  - Card 1: circle avatar placeholder (gradient blue), "Ahmed K." bold, "Gold Chiller — Morocco" in #9CA3AF, five yellow star icons, quote: "I've earned over 50,000 TASK in my first month. The withdrawal warming system actually helped me — by the time I could withdraw, my tokens were worth 5x more. This platform changed my life."
  - Card 2: circle avatar placeholder (gradient green), "Sarah M." bold, "Advertiser — United States" in #9CA3AF, five stars, quote: "We got 280 verified posts about our token launch in under 12 hours. Every single one came with a screenshot and live link. The ROI compared to traditional marketing agencies is insane."
  - Card 3: circle avatar placeholder (gradient purple), "Carlos R." bold, "Diamond Chiller — Brazil" in #9CA3AF, five stars, quote: "Better than any freelance platform I've used. I earn TaskCoins while growing my own social media accounts. The level system keeps me motivated — I'm grinding for Legend."
  - Cards have quote icon (") in blue at top-left

**Section 9 — CTA Banner (full width, gradient from #388EFF to #2563EB):**
- Heading: "Ready to Start?" — white 40px bold
- Subheading: "Join 1,200+ Chillers earning TaskCoins every day" — white/80
- Two buttons side by side: "Start Earning" (white bg, blue text), "Launch a Campaign" (white outline, white text)

**Section 10 — Footer (bg #0A0E17, border-t border-white/5):**
- 4 columns (stacked on mobile):
  - Column 1 "Platform": Home, Task Board, Leaderboard, Proof Gallery, Advertiser Marketplace
  - Column 2 "Resources": University, Blog, Whitepaper, Roadmap, Documentation
  - Column 3 "Services": PR Writing, YouTuber Promotion, Outlet Distribution, dApp Creation, Token Launch, Smart Contract Audit
  - Column 4 "Legal": Terms of Service, Privacy Policy, Cookie Policy, Contact Us
- Bottom bar: left "© 2026 TaskCoins. All rights reserved.", right: social icons (X, Telegram, Instagram, Discord, GitHub) — white/40, hover:white

---

## PAGE 2: SIGN UP & LOGIN (/auth)

Centered on the page, max-width 480px card on dark background.

**Sign Up view (default):**
- Card with glass-morphism styling, padding 40px
- TaskCoins logo at top center
- Heading: "Create Your Account" — Satoshi 28px
- Toggle pill/tabs: "Chiller" | "Advertiser" — selected has blue bg, unselected has transparent
  - When "Chiller" selected, subtitle: "Start earning crypto by completing social media tasks"
  - When "Advertiser" selected, subtitle: "Get your project promoted by thousands of verified users"
- Form fields (each with label above, glass-style input):
  - "Display Name" — text input, placeholder "Enter your name"
  - "Email Address" — email input, placeholder "you@example.com"
  - "Password" — password input with show/hide eye icon, placeholder "Create a password"
  - "Confirm Password" — password input, placeholder "Confirm your password"
  - "Referral Code (optional)" — text input, placeholder "Enter referral code", smaller text below: "Have a friend on TaskCoins? Enter their code to connect."
- Checkbox: "I agree to the Terms of Service and Privacy Policy" (with links underlined)
- "Create Account" button — full width, primary blue, large
- Divider line with "or" text in center
- "Connect Wallet" button — full width, secondary outline, Wallet icon left — text "Sign up with MetaMask"
- "Continue with Google" button — full width, secondary outline, Google G icon
- Bottom text: "Already have an account?" + "Log In" blue link

**Log In view:**
- Same card styling
- Heading: "Welcome Back"
- Subtitle: "Log in to your TaskCoins account"
- Form: Email + Password (with show/hide) fields
- "Log In" primary blue button full width
- "Forgot Password?" link below in blue
- Divider + "Connect Wallet" + "Continue with Google" buttons
- Bottom: "Don't have an account?" + "Sign Up" blue link

---

## PAGE 3: CHILLER DASHBOARD (/dashboard/chiller)

**Sidebar (desktop):**
- Logo at top
- User section: avatar circle with initial letter, display name "Ahmed K.", level badge "Gold" in gold color, "87 Rep" small text
- Menu items with Lucide icons, 14px Inter, #9CA3AF, active: white text + blue left border + blue/10 bg:
  - LayoutDashboard — Dashboard (active)
  - ClipboardList — Task Board
  - ListTodo — My Tasks
  - Wallet — Wallet
  - Lock — Staking
  - Trophy — Leaderboard
  - Users — Referrals
  - BookOpen — University
  - User — Profile
  - Settings — Settings
- Bottom of sidebar: small "Logout" link in red/50

**Main content:**

**Row 1 — Welcome + Quick Stats:**
- "Welcome back, Ahmed" — 28px Satoshi bold
- "Here's your earning overview" — 16px #9CA3AF
- 5 stat cards in a row (horizontal scroll on mobile, each min-width 200px):
  - Card 1 (green tint): Wallet icon in green circle, "Available Balance" label in 13px #9CA3AF, "8,450 TASK" in 28px bold white, "≈ $845.00" in 14px #9CA3AF below
  - Card 2 (blue tint): TrendingUp icon in blue circle, "Total Earned" label, "24,200 TASK" value, "+1,250 this week" in small green text
  - Card 3 (purple tint): CheckCircle icon in purple circle, "Tasks Completed" label, "186" value, "12 this week" in small text
  - Card 4 (gold tint): Award icon in gold circle, "Current Level" label, "Gold" value with gold badge, progress bar below: "186/200 — 14 more tasks to Diamond" in 12px
  - Card 5 (blue tint): Shield icon in blue circle, "Reputation" label, circular gauge/ring showing 87/100, green color for the ring

**Row 2 — Earnings Chart:**
- Glass card, full width
- Header: "Earnings Overview" left, time toggle right: "7D" | "30D" | "90D" pill buttons (30D active/blue)
- Line chart (area chart with gradient fill below the line):
  - X axis: dates (last 30 days, show every 5th date)
  - Y axis: TASK amounts
  - Line color: #388EFF
  - Area fill: gradient from #388EFF/20 to transparent
  - Sample data: upward trend with natural variation, starting ~200 TASK/day, ending ~400 TASK/day
  - Tooltip on hover showing exact date and amount

**Row 3 — Two columns (stacked on mobile):**

Left column — "Top Paying Tasks" (with "View All →" link to /tasks):
- 5 task items in a list, each as a small card/row:
  1. Blue X icon | "Share $TOKEN Launch on X" | "200 TASK" green | "Gold+" badge | "18h left" with clock | "45/100" small progress bar | "Claim" small blue button
  2. Orange Reddit icon | "Post about DeFi Protocol in r/crypto" | "150 TASK" | "Silver+" | "23h left" | "12/50" | "Claim"
  3. Blue CMC icon | "Community post about $TASK utility" | "100 TASK" | "Any" | "12h left" | "89/100" | "Claim"
  4. Yellow Binance icon | "Write about AI crypto trends" | "175 TASK" | "Gold+" | "20h left" | "23/75" | "Claim"
  5. Red YouTube icon | "Comment on crypto review video" | "75 TASK" | "Any" | "8h left" | "67/80" | "Claim"

Right column — "Recent Activity":
- Activity feed list (8 items), each with icon, description, timestamp, and TASK amount:
  - CheckCircle green — "Task #247 approved" — "+200 TASK" green — "2 hours ago"
  - Users blue — "Referral bonus from @maria_r" — "+12 TASK" green — "5 hours ago"
  - Award gold — "Level up! You reached Gold" — "" — "Yesterday"
  - CheckCircle green — "Task #244 approved" — "+150 TASK" green — "Yesterday"
  - CheckCircle green — "Task #241 approved" — "+100 TASK" green — "2 days ago"
  - Lock purple — "Staked 5,000 TASK — Tier 2 unlocked" — "" — "3 days ago"
  - CheckCircle green — "Task #238 approved" — "+175 TASK" green — "3 days ago"
  - Users blue — "New referral: @carlos_r signed up" — "" — "4 days ago"

**Row 4 — Referral Banner (full width, subtle blue gradient bg):**
- Left: "Invite friends. Earn 5% of everything they make — forever." in 20px bold
- Right: referral link "taskcoins.io/ref/AHMED2024" with "Copy" button + share icons (X, Telegram, WhatsApp)

---

## PAGE 4: TASK BOARD (/tasks)

**Top bar:**
- Heading: "Task Board" — 28px Satoshi bold
- Right side: Search bar (glass input, Search icon, placeholder "Search tasks...") + View toggle (Grid icon | List icon, grid active)

**Filter sidebar (left, 250px on desktop — slide-out sheet on mobile with Filter icon button to open):**
- "Filters" heading with "Reset All" link
- **Platform** section: checkboxes with colored icons next to each:
  - ☐ All Platforms
  - ☐ X (Twitter) — blue icon
  - ☐ Reddit — orange icon
  - ☐ CoinMarketCap — blue icon
  - ☐ Binance Square — yellow icon
  - ☐ YouTube — red icon
  - ☐ Telegram — blue icon
- **Reward Range** section: dual-handle slider 0 to 500 TASK, showing "50 - 300 TASK" selected range
- **Level Required** section: dropdown select with options: Any Level, Bronze+, Silver+, Gold+, Diamond+
- **Sort By** section: dropdown with: Newest First, Highest Reward, Ending Soon, Most Available
- "Apply Filters" blue button (full width)

**Task grid (3 columns desktop, 2 tablet, 1 mobile):**
12 task cards total. Each card (glass card, rounded-2xl, hover:border-blue-500/30):
- Top-left: Platform icon + colored platform badge (e.g., blue rounded badge "X (Twitter)" or orange "Reddit")
- Top-right: time remaining "18h 32m" with Clock icon in #9CA3AF
- Title: task name in 17px bold white — "Share $TOKEN Launch Announcement on X"
- Description: 2 lines max, truncated, 14px #9CA3AF — "Copy the provided text and image, post it on your X account with all hashtags. Tag @tokenproject."
- Divider line (border-white/5)
- Stats row:
  - "200 TASK" in #09CE84 bold with Coins icon
  - "Gold+" level badge (gold colored small badge)
  - "45/100" with small progress bar
- "Claim Task" button — full width, primary blue, rounded-xl

Sample tasks (vary these across the 12 cards):
1. X — "Share $TOKEN Launch Announcement" — 200 TASK — Gold+ — 18h — 45/100
2. Reddit — "Post in r/cryptocurrency about DeFi Protocol" — 150 TASK — Silver+ — 23h — 12/50
3. CMC — "Community post about $TASK utility" — 100 TASK — Any — 12h — 89/100
4. Binance Square — "Write about AI crypto trends" — 175 TASK — Gold+ — 20h — 23/75
5. YouTube — "Comment on crypto review video" — 75 TASK — Any — 8h — 67/80
6. Telegram — "Share announcement in 3 Telegram groups" — 50 TASK — Any — 24h — 34/100
7. X — "Retweet and quote tweet about NFT collection" — 120 TASK — Silver+ — 16h — 55/80
8. Reddit — "Post analysis in r/defi" — 200 TASK — Gold+ — 20h — 8/30
9. CMC — "Bullish post about $ETH community" — 80 TASK — Any — 6h — 91/100
10. Binance Square — "Share trading strategy post" — 150 TASK — Silver+ — 22h — 18/50
11. X — "Thread about Web3 gaming launch" — 250 TASK — Diamond+ — 24h — 5/20
12. YouTube — "Review video comment with insights" — 100 TASK — Bronze+ — 14h — 42/60
13. X — "Follow + Retweet @tokenproject" — 25 TASK — Any — 48h — 120/200 — (engagement task, lower reward)
14. X — "Like + Quote Tweet about $TASK" — 40 TASK — Any — 24h — 85/150 — (engagement task)

**Task Detail (opens when clicking a card — modal overlay or separate page):**
- Top: back arrow + "Task Details"
- Platform badge (large) + task title in 24px bold
- Advertiser info: small avatar + "Posted by CryptoProject_X" + "Active Advertiser" green badge
- Stats row: "200 TASK" reward large green | "Gold+ required" badge | "18h 32m remaining" clock | "45/100 completed" progress
- Divider
- "Instructions" section heading:
  - "1. Copy the text below exactly as written"
  - "2. Post it on your X (Twitter) account"
  - "3. Include the provided image in your post"
  - "4. Make sure to include all hashtags"
  - "5. Take a screenshot of your live post"
  - "6. Submit the screenshot and your post URL below"
- "Content to Post" section: dark box with the text to copy, "Copy Text" button in top-right with Copy icon
- "Image to Include" section: image preview thumbnail (placeholder gradient image), "Download Image" button
- Divider
- "Submit Proof" section:
  - File upload area: dashed border box, "Upload screenshot of your post" text, "Click to upload or drag and drop" subtext, "PNG, JPG up to 10MB" small text
  - Text input: "Post URL" — placeholder "https://x.com/youraccount/status/..."
  - "Submit Proof" blue button (large, full width)
  - "Cancel" secondary button below

---

## PAGE 5: MY TASKS (/dashboard/chiller/my-tasks)

- Heading: "My Tasks" — 28px
- 4 tab buttons: "Active (3)" | "Submitted (5)" | "Approved (42)" | "Rejected (2)" — active tab has blue underline + white text, others #9CA3AF. Numbers in small blue badge circles.

**Active tab (default):**
3 task cards, each showing:
- Platform icon + task title + advertiser name
- Reward: "200 TASK" green
- Countdown: "18h 32m remaining" with animated clock icon, orange if < 6h
- "Submit Proof" blue button + "Release Task" small gray text button below

**Submitted tab:**
5 task cards, each showing:
- Platform icon + task title
- "Awaiting Review" yellow badge with Clock icon
- Submitted proof: small screenshot thumbnail + link text (truncated)
- "Submitted 2 hours ago" timestamp

**Approved tab:**
List of 10 visible (with "Show More" to see all 42):
- Each: platform icon + task title + "Approved" green badge with CheckCircle
- "+200 TASK" in green bold on the right
- "Approved 3 hours ago" timestamp
- Small screenshot thumbnail

**Rejected tab:**
2 cards:
- Platform icon + task title + "Rejected" red badge with XCircle
- Rejection reason in red/orange text: "Screenshot does not match the required content. The post is missing the required hashtags."
- "Resubmit" blue outline button

---

## PAGE 6: ADVERTISER DASHBOARD (/dashboard/advertiser)

**Sidebar** (same style as Chiller but different menu items):
- LayoutDashboard — Dashboard (active)
- PlusCircle — Create Campaign
- FolderOpen — My Campaigns
- Eye — Review Proofs
- BarChart3 — Analytics
- Wallet — Wallet
- Settings — Settings

**Main content:**

**Row 1 — Stats (5 cards):**
- "Total Spend" — 145,000 TASK — Wallet blue icon — "32,000 this month" small text
- "Active Campaigns" — 3 — Rocket green icon — "2 completed" small text
- "Tasks Completed" — 847 — CheckCircle purple icon — "+124 this week" small text
- "Posts Live" — 823 — Globe green icon — "98% live rate" small text
- "Estimated Reach" — 1.2M — Eye orange icon — "across 6 platforms" small text

**Row 2 — Active Campaigns:**
- Section header: "Active Campaigns" + "Create New Campaign" blue button on right
- 3 campaign cards (horizontal, each takes full width):
  - Card 1: "Launch $TOKEN on X & Reddit" — platform icons (X, Reddit) — status "Active" green badge — "67/100 tasks" with progress bar at 67% — "Spend: 15,000 TASK" — "Created 2 days ago" — "View Details" link
  - Card 2: "Reddit AMA Promotion" — Reddit icon — "Active" — "23/50 tasks" progress 46% — "Spend: 7,500 TASK" — "Created 5 days ago"
  - Card 3: "CMC Community Push Q1" — CMC icon — "Completed" green badge with check — "100/100 tasks" progress 100% green — "Spend: 10,000 TASK" — "Completed yesterday"

**Row 3 — Two columns:**

Left — "Recent Proof Submissions" (with "Review All →" link):
- 5 submission rows:
  - Avatar circle + "CryptoKing" + Gold badge → "Share $TOKEN on X" → small screenshot thumb → "2 min ago" → "Review" blue button
  - Avatar + "maria_r" + Silver → "Reddit AMA post" → screenshot → "15 min ago" → "Review"
  - Avatar + "DefiHunter" + Gold → "CMC community post" → screenshot → "1 hour ago" → "Review"
  - Avatar + "carlos_crypto" + Diamond → "Binance Square write-up" → screenshot → "2 hours ago" → "Review"
  - Avatar + "web3sarah" + Silver → "YouTube comment" → screenshot → "3 hours ago" → "Review"

Right — "Campaign Performance" mini chart:
- Small bar chart showing tasks completed per day for last 7 days
- Total: "124 tasks this week"

---

## PAGE 7: CREATE CAMPAIGN (/dashboard/advertiser/create)

Full-page wizard with progress bar at top.

**Progress bar:** 5 steps, connected by lines, current step = blue circle with number, completed = green circle with check, upcoming = gray circle with number. Labels below each: "Platforms" → "Content" → "Requirements" → "Budget" → "Review"

**Step 1 — Choose Platforms:**
- Heading: "Where do you want your content posted?" — 28px Satoshi
- Subheading: "Select one or more platforms. You can target multiple platforms in a single campaign." — #9CA3AF
- 6 platform cards in 3x2 grid (2x3 on mobile). Each card (glass, rounded-2xl, padding 24px, text-center):
  - When unselected: normal border, icon in gray
  - When selected: border-[#388EFF], blue glow, icon in color, small blue checkmark in top-right corner
  - Card 1: large blue X icon, "X (Twitter)" bold, "280M monthly active users. Best for crypto announcements and threads." small text
  - Card 2: large orange Reddit icon, "Reddit", "430M monthly active users. Best for community discussions and analysis posts."
  - Card 3: large blue CMC icon, "CoinMarketCap", "350M monthly visits. Best for coin-specific community posts."
  - Card 4: large yellow Binance icon, "Binance Square", "150M users. Best for trading insights and market analysis."
  - Card 5: large red YouTube icon, "YouTube", "2.5B monthly active users. Best for video comments and engagement."
  - Card 6: large blue Telegram icon, "Telegram", "800M monthly active users. Best for group sharing and announcements."
- Bottom: "Next →" blue button right-aligned + "Cancel" gray link left

**Step 2 — Create Content:**
- Heading: "What should Chillers post?"
- "Post Content" label + large textarea (6 rows, glass input), placeholder: "Write the exact text you want Chillers to copy and post. Include hashtags, mentions, and any specific messaging..."
- "Upload Image (optional)" — drag-and-drop zone: dashed border, cloud-upload icon, "Drag and drop an image or click to browse", "PNG, JPG, GIF up to 5MB" — after upload shows image preview with "Remove" X button
- "Link to Include (optional)" — text input, placeholder "https://yourproject.com"
- "Special Instructions (optional)" — textarea (3 rows), placeholder "Any additional instructions for Chillers? E.g., 'Tag @ourproject', 'Use at least 3 hashtags', 'Post between 9 AM - 12 PM EST'"
- Bottom: "← Back" gray button left, "Next →" blue button right

**Step 3 — Set Requirements:**
- Heading: "Who can complete your tasks?"
- "Minimum Chiller Level" — 5 clickable option cards in a row:
  - "Any Level" (green border if selected) — "Open to all Chillers"
  - "Silver+" — "50+ tasks completed"
  - "Gold+" — "200+ tasks completed"
  - "Diamond+" — "500+ tasks completed"
  - "Legend" — "1,000+ tasks completed"
- "Minimum Reputation Score" — slider from 0 to 100, current value shown in blue circle above handle, default 0. Marks at 0, 25, 50, 75, 100.
- "Task Deadline" — radio button options: "12 hours", "24 hours" (selected by default, blue), "48 hours", "72 hours"
- "← Back" + "Next →" buttons

**Step 4 — Set Budget:**
- Heading: "Set your campaign budget"
- Launch promotion banner at top (green border glass card, Zap icon): "🎉 Launch Bonus: Get 5% extra distribution on your campaign! Pay for 1,000 TASK worth of tasks, get 1,050 TASK in distribution. Limited time offer."
- "Reward Per Task" — number input with "TASK" suffix label, default 100, stepper buttons +/-
- "Number of Tasks" — number input, default 50, stepper buttons
- Live calculation card below (glass card, blue border):
  - Line 1: "Worker Rewards:" — "5,000 TASK" right-aligned — "(100 × 50)" small text
  - Line 2: "Platform Fee (20%):" — "1,250 TASK"
  - Divider line
  - Line 3 bold: "Total Campaign Cost:" — "6,250 TASK" in 24px bold blue
  - Line 4: "Your Balance:" — "50,000 TASK" in green — green CheckCircle icon — "(Sufficient)" green text
  - (If balance insufficient: red text "Insufficient balance — deposit more TASK" with "Deposit" link)
- "← Back" + "Next →" buttons

**Step 5 — Review & Launch:**
- Heading: "Review Your Campaign"
- Summary card (glass, large padding):
  - "Platforms:" row with selected platform icons/badges
  - "Content Preview:" first 3 lines of content text + "Show full content" toggle
  - "Image:" thumbnail preview (or "No image")
  - "Requirements:" "Gold+ | 50+ reputation | 24h deadline"
  - "Budget:" "100 TASK × 50 tasks = 5,000 TASK + 1,250 fee = 6,250 TASK total"
  - Divider
  - Checkbox: "I confirm this campaign follows TaskCoins community guidelines"
- "← Back" gray button, "Launch Campaign 🚀" large blue button with glow effect
- On click: success overlay/modal — confetti animation, green check circle, "Your campaign is now live!", "Chillers will start completing tasks immediately.", "View Campaign" button + "Create Another" link

---

## PAGE 8: REVIEW PROOFS (/dashboard/advertiser/review)

- Heading: "Review Proof Submissions" — 28px
- Stats bar: "12 Pending" yellow badge | "847 Approved" green badge | "23 Rejected" red badge
- Filter dropdown: "All Campaigns" | "Launch $TOKEN on X" | "Reddit AMA" | "CMC Push"

Proof submission queue — 8 cards stacked vertically:
Each card (glass, rounded-2xl, padding 20px):
- Left section (30%): Chiller avatar circle + username bold + level badge (Gold/Silver/etc) + reputation "87/100" small text + "Member since Jan 2026" tiny text
- Center section (40%):
  - Screenshot thumbnail (placeholder image, ~200x150px) — click opens lightbox/modal showing full-size image
  - Below screenshot: link text "https://x.com/cryptoking/status/1234..." — blue, clickable, ExternalLink icon
  - "Submitted 2 hours ago" — #9CA3AF small text
  - Platform badge: "X (Twitter)" blue badge
- Right section (30%):
  - "Approve" large green button (CheckCircle icon + "Approve" text)
  - "Reject" large red outline button (XCircle icon + "Reject" text)
  - When Reject is clicked: text input slides down "Reason for rejection" + "Confirm Reject" small red button

Sample submissions with varied Chillers, platforms, and timestamps.

---

## PAGE 9: WALLET (/dashboard/wallet)

**Balance hero section (centered, padding 48px):**
- Small "Your Balance" label in #9CA3AF
- Large token display: blue coin icon + "8,450 TASK" in 48px Satoshi bold white
- USD equivalent: "≈ $845.00" in 20px #9CA3AF
- Two buttons below, side by side: "Deposit" (primary blue, ArrowDown icon) | "Withdraw" (secondary outline, ArrowUp icon)

**Two tabs below: "Deposit" | "Withdraw"**

**Deposit tab:**
- Glass card with:
  - Heading: "Deposit TaskCoins to Your Account"
  - Step 1: "Connect your wallet" — "Connect MetaMask" button (outline, MetaMask fox icon) — when "connected": green check + "0x4f2...8a3 Connected" text
  - Step 2: "Enter amount" — number input with "TASK" suffix + "MAX" small blue button
  - Step 3: "Confirm deposit" — "Deposit TASK" primary blue button (full width)
  - Info box: blue border, info icon, "Deposits are confirmed after 12 block confirmations (~3 minutes). Gas fees apply."

**Withdraw tab:**
- Glass card with:
  - **Withdrawal Tier Progress** (visual, this is important):
    - Horizontal progress bar with 4 stages labeled:
      - Stage 1: "New (0-30 days)" — red/locked icon — "No withdrawals"
      - Stage 2: "Warmed (30-60 days)" — orange — "Monthly, min 500 TASK"
      - Stage 3: "Trusted (60+ days)" — green — "Bi-weekly, min 200 TASK"
      - Stage 4: "VIP (Diamond+)" — blue/purple with star — "Weekly, min 100 TASK"
    - Current tier highlighted with glow effect
    - If new account: large yellow warning banner: "⚠ Withdrawals unlock after 30 days of activity" with countdown: "22 days 14 hours remaining" and progress bar showing days elapsed
  - Tier rules table (glass card):
    - 4 rows: Account Status | Withdrawal Frequency | Minimum Amount | Requirements
    - New (0-30 days) | Locked | — | Complete 30 days of activity
    - Warmed (30-60 days) | Once per month | 500 TASK | 30+ days active
    - Trusted (60+ days) | Bi-weekly | 200 TASK | 60+ days + 70+ reputation
    - VIP | Weekly | 100 TASK | Diamond+ level + 90+ reputation
    - Current tier row highlighted with blue border
  - If eligible: "Amount to withdraw" number input + "Wallet address" text input (placeholder "0x...") + "Request Withdrawal" primary button
  - Blue info banner at bottom: Wallet icon, "TaskCoins is designed for long-term growth. The longer you hold, the more your earnings are worth. Workers who held from Day 1 saw their tokens grow 10x. Hold for 100x. 💎"

**Transaction History section below:**
- Heading: "Transaction History" + "Export CSV" small link
- Table (glass card, rounded-2xl):
  - Columns: Date | Type | Amount | Status
  - Type badges: green "Earned", blue "Deposited", orange "Withdrawn", purple "Staked", cyan "Referral Bonus", gray "Platform Fee"
  - Amount: green "+200 TASK" for earnings, red "-500 TASK" for withdrawals
  - Status badges: green "Completed", yellow "Pending", red "Failed"
  - 20 sample rows with varied types, dates (last 30 days), and amounts
  - Pagination: "← Previous | Page 1 of 3 | Next →"

---

## PAGE 10: STAKING (/dashboard/chiller/staking)

- Hero: "Stake TaskCoins" in 32px Satoshi bold, "Unlock premium rewards and higher-paying tasks" in #9CA3AF — subtle blue glow effect behind text

**Current Status card (glass, blue border if staking active):**
- If staking: "Currently Staked: 5,000 TASK" in 24px bold, "Current Tier: Tier 2" with TrendingUp icon, "Active Benefit: 5% bonus on all earnings" in green
- If not staking: "You haven't staked any TaskCoins yet." in #9CA3AF, "Stake now to unlock premium benefits and earn more from every task." subtext

**Tier cards (4 in a row, scrollable on mobile):**
Each card (glass, rounded-2xl, tall, centered content):
- Tier 1: Star icon in blue circle, "Tier 1" label, "1,000 TASK" in 24px bold, "Access premium task queue" description, if unlocked: blue glow border "Active", if locked: dimmed with Lock icon overlay
- Tier 2: TrendingUp icon in green circle, "Tier 2", "5,000 TASK", "5% bonus on all earnings", currently active: green glow border "Current Tier ✓"
- Tier 3: Zap icon in purple circle, "Tier 3", "10,000 TASK", "10% bonus + early access to new campaigns", locked: dimmed, "5,000 more TASK needed"
- Tier 4: Crown icon in gold circle, "Tier 4", "50,000 TASK", "VIP status + direct advertiser offers", locked: dimmed, "45,000 more TASK needed"

**Stake/Unstake section (two glass cards side by side, stacked on mobile):**

Left card — "Stake":
- "Amount to Stake" number input with TASK suffix + "MAX" button
- "Available: 8,450 TASK" text below input
- "Stake Now" primary blue button full width
- Small text: "Staked tokens are locked until you request unstaking."

Right card — "Unstake":
- "Amount to Unstake" number input with TASK suffix + "MAX" button
- "Currently Staked: 5,000 TASK" text below
- "Request Unstake" secondary outline button full width
- Warning box: orange border, AlertTriangle icon, "Unstaking has a 7-day cooldown period. Your tier benefits remain active during the cooldown. After 7 days, tokens return to your available balance."

**Staking History table (glass card):**
- Columns: Date | Action | Amount | Tier Change | Status
- 5 sample rows:
  - Mar 5, 2026 | Staked | +5,000 TASK | Tier 1 → Tier 2 | Completed
  - Feb 28, 2026 | Staked | +1,000 TASK | None → Tier 1 | Completed
  - Feb 20, 2026 | Unstaked | -500 TASK | (partial) | Completed
  - Feb 15, 2026 | Staked | +1,500 TASK | None → Tier 1 | Completed
  - Feb 10, 2026 | Staked | +500 TASK | — | Completed

---

## PAGE 11: LEADERBOARD (/leaderboard)

- Hero: "Leaderboard" 36px Satoshi bold centered, "Top Chillers — Compete, Climb, Earn" 18px #9CA3AF

**Time toggle:** "This Week" | "This Month" (active, blue) | "All Time" — pill buttons
**Category toggle:** "Most Tasks" (active) | "Most Earned" | "Best Reputation" | "Most Referrals" — tab buttons with underline

**Top 3 podium section (visual, above the table):**
- Three cards in a row, center one (#1) slightly larger/elevated:
  - #1 (center, gold): large gold crown icon, avatar circle, "CryptoKing" bold 20px, "Legend" badge with purple glow, "1,247 tasks" stat, "89,400 TASK earned", gold background tint card
  - #2 (left, silver): silver medal, avatar, "DefiQueen" bold, "Diamond" badge, "1,102 tasks", "76,200 TASK", silver tint
  - #3 (right, bronze): bronze medal, avatar, "Web3Wizard" bold, "Diamond" badge, "987 tasks", "68,500 TASK", bronze tint

**Rankings table (glass card, below podium):**
- Columns: Rank | User | Level | Tasks | TASK Earned | Reputation | Platforms
- Rows 4-50 with sample data, each row:
  - Rank number (#4, #5...) in #9CA3AF
  - Avatar circle + username — bold white
  - Level badge colored (Bronze/Silver/Gold/Diamond)
  - Tasks completed number
  - TASK earned with green color
  - Reputation score /100
  - Small platform icons (X, Reddit, CMC etc.) showing which platforms they're active on
- Alternate row backgrounds for readability (subtle)
- Pre-populate with 50 users (rows 4-50 after the podium shows 1-3), realistic varied data

**Sticky bottom bar (fixed to viewport bottom, blue bg):**
- "Your Rank: #47" left side, "Complete 14 more tasks to reach #40" center, small progress bar right

---

## PAGE 12: REFERRALS (/dashboard/chiller/referrals)

- Heading: "Referral Program" 32px, "Invite Friends. Earn 5% of Everything They Make —" then "Forever." in #388EFF — 20px subheading

**Referral Link section (glass card, blue border, padding 32px):**
- "Your Referral Link" label
- Large display box: "https://taskcoins.io/ref/AHMED2024" in monospace 18px white, glass background
- Buttons row: "Copy Link" blue button (Copy icon — shows "Copied! ✓" for 2 sec after click) | Share icons: X, Telegram, WhatsApp, Email — each in small circle buttons

**Stats row (3 glass cards):**
- Card 1: Users icon in blue circle, "Total Referrals" #9CA3AF, "12" in 32px bold
- Card 2: UserCheck icon in green circle, "Active Referrals" label, "8" in 32px bold, "(completed 1+ task)" small text
- Card 3: Wallet icon in green circle, "Referral Earnings" label, "3,240 TASK" in 32px bold green, "≈ $324.00" small text

**Referral table (glass card):**
- Columns: User | Joined | Their Tasks | Their Status | Your Earnings
- 8 rows:
  - Avatar + "maria_r" | Mar 2, 2026 | 47 tasks | green dot "Active" | +620 TASK
  - Avatar + "carlos_crypto" | Feb 28, 2026 | 82 tasks | green "Active" | +1,140 TASK
  - Avatar + "web3kid" | Feb 25, 2026 | 23 tasks | green "Active" | +280 TASK
  - Avatar + "nft_lover" | Feb 20, 2026 | 56 tasks | green "Active" | +670 TASK
  - Avatar + "defi_sarah" | Feb 15, 2026 | 31 tasks | green "Active" | +390 TASK
  - Avatar + "trader_mo" | Feb 10, 2026 | 5 tasks | yellow "New" | +40 TASK
  - Avatar + "hodl_king" | Feb 5, 2026 | 12 tasks | green "Active" | +100 TASK
  - Avatar + "moon_boy" | Jan 30, 2026 | 0 tasks | gray "Inactive" | +0 TASK

**How It Works section (3 cards in a row at bottom):**
- Card 1: Share2 icon in blue, "Share Your Link", "Send your unique referral link to friends via social media, messaging, or email."
- Card 2: UserPlus icon in green, "They Sign Up & Earn", "Your friends create an account and start completing tasks to earn TaskCoins."
- Card 3: Coins icon in gold, "You Earn 5% — Forever", "Every time your referral earns TaskCoins, 5% is automatically credited to you. This comes from the platform fee — their earnings are never reduced."

---

## PAGE 13: UNIVERSITY (/university)

- Hero: "TaskCoins University" 36px Satoshi bold, "Learn how to grow your accounts and maximize your earnings" 18px #9CA3AF, BookOpen icon in blue

**Course grid (3 columns desktop, 1 mobile):**
6 course cards, each (glass card, rounded-2xl, overflow-hidden):
- Top: gradient thumbnail area (200px tall) with large icon centered:
  - Course 1: Blue gradient (#1DA1F2 to #0A66C2) with large X logo, title overlay at bottom "How to Grow Your X Account from 0 to 10K"
  - Course 2: Orange gradient (#FF4500 to #FF6B35) with Reddit icon, "Reddit Karma Building: The Complete Guide"
  - Course 3: Red gradient (#FF0000 to #CC0000) with YouTube icon, "YouTube Channel Growth for Beginners"
  - Course 4: Blue gradient (#388EFF to #2563EB) with TaskCoins icon, "Maximize Your TaskCoins Earnings"
  - Course 5: Purple gradient (#8B5CF6 to #6D28D9) with Wallet icon, "Crypto Basics: Wallets, Tokens, and DeFi"
  - Course 6: Orange gradient (#F6851B to #E2761B) with fox icon, "How to Use MetaMask Like a Pro"
- Bottom section (padding 20px):
  - Difficulty badge: green "Beginner" or orange "Intermediate"
  - Stats: "8 lessons • 45 min" with BookOpen + Clock icons
  - "Start Course" blue button full width

**Click a course → Course page:**
- Header: course title 28px, difficulty badge, "4/8 lessons completed" progress bar green
- Two-column layout:
  - Left sidebar (250px): lesson list, numbered, each with title, checkmark if completed (green check), current lesson highlighted blue
    - Lesson 1: "Introduction to X" ✓ completed
    - Lesson 2: "Setting Up Your Profile" ✓ completed
    - Lesson 3: "Content Strategy" ✓ completed
    - Lesson 4: "Hashtag Research" ← Current (blue highlight)
    - Lesson 5: "Engagement Tactics" (locked, gray)
    - Lesson 6: "Growth Hacking" (locked)
    - Lesson 7: "Analytics & Optimization" (locked)
    - Lesson 8: "Monetization" (locked)
  - Main content area:
    - Lesson title: "Lesson 4: Hashtag Research" 24px
    - Video placeholder: dark box 16:9 ratio with Play circle icon centered, "Video lesson coming soon" text
    - Lesson content: 4 paragraphs of placeholder text about the topic, formatted with headings, bullet points
    - "Mark as Complete" green button
    - Navigation: "← Previous Lesson" | "Next Lesson →" buttons

---

## PAGE 14: SERVICES (/services)

- Hero: "Web3 Services" 36px Satoshi bold, "Built by the team behind Pepeto. End-to-end crypto solutions." 18px #9CA3AF
- Small badges in a row: "Trusted Team" green, "50+ Projects Delivered" blue, "Since 2024" purple

**Service cards (2 columns desktop, 1 mobile), 8 cards total:**
Each card (glass, rounded-2xl, padding 28px, hover:border-blue-500/30):
- Icon in colored circle (48px) at top
- Title in 20px bold below
- Description in 15px #9CA3AF (2-3 sentences)
- Price: "Starting from X TASK" in #388EFF bold
- "Request Quote" button (secondary outline, full width at bottom)

Cards:
1. FileText icon / blue circle — "PR Writing" — "Professional crypto press releases written by experienced blockchain journalists. Distributed to major outlets including CoinDesk, CoinTelegraph, and Bitcoin Magazine. Includes SEO optimization and keyword targeting." — "From 5,000 TASK"
2. Play icon / red circle — "YouTuber Promotion" — "Get your project featured by established crypto YouTubers with 50K-200K subscribers. We handle outreach, scripting guidance, and performance tracking. Average 50K+ views per feature." — "From 10,000 TASK"
3. Globe icon / green circle — "Distribution on Outlets" — "Get your news published on CoinDesk, CoinTelegraph, Bitcoin Magazine, Decrypt, and 20+ tier-1 crypto news outlets. We have direct relationships with editorial teams." — "From 25,000 TASK"
4. Code icon / purple circle — "dApp Creation" — "Full smart contract development plus frontend UI for your Web3 project. Includes Solidity/Vyper contracts, testing, deployment, and a React/Next.js frontend with wallet integration." — "From 50,000 TASK"
5. Rocket icon / orange circle — "Token Launch" — "End-to-end ERC-20 or BEP-20 token creation, deployment, and Uniswap/PancakeSwap listing. Includes tokenomics design, contract audit, and liquidity setup." — "From 30,000 TASK"
6. Image icon / pink circle — "NFT Development" — "NFT collection creation with generative art engine, ERC-721/1155 smart contract, custom minting page, and marketplace listing on OpenSea and Blur." — "From 20,000 TASK"
7. Shield icon / cyan circle — "Smart Contract Audit" — "Comprehensive security audit for your existing smart contracts. Includes vulnerability assessment, gas optimization recommendations, and a detailed PDF report." — "From 15,000 TASK"
8. Lightbulb icon / yellow circle — "Web3 Consulting" — "Strategic advisory on tokenomics design, go-to-market strategy, community building, and investor relations. Led by founders who launched Pepeto to a $50M+ market cap." — "From 10,000 TASK"

**"Request Quote" modal (opens on button click):**
- Overlay with glass card, 500px max-width
- Heading: "Request a Quote" 24px
- Form fields: Name, Email, Project URL (optional), Service Type (pre-filled from card clicked), Budget dropdown ("5K-10K TASK" / "10K-25K" / "25K-50K" / "50K-100K" / "100K+"), Description textarea (placeholder "Tell us about your project and what you need...")
- "Submit Request" blue button + "Cancel" link
- On submit: success message "Your request has been submitted. We'll get back to you within 24 hours."

**Why Choose Us section (3 cards at bottom):**
- Card 1: Award icon, "Proven Team", "The team behind Pepeto — launched and scaled to $50M+ market cap. We've done it ourselves, so we know what works."
- Card 2: Zap icon, "End-to-End", "From token creation to marketing to community building. One team handles everything — no need to coordinate 5 different agencies."
- Card 3: BarChart3 icon, "Results-Driven", "We measure everything. Real metrics, real ROI, real proof. No vanity metrics, no empty promises."

---

## PAGE 15: BLOG (/blog)

- Hero section: Featured post as a large card (full width, 400px tall):
  - Gradient placeholder image background
  - Dark overlay gradient from bottom
  - Category badge "News" in blue, top-left
  - Title: "TaskCoins Launches: The Future of Social Media Earning" in 32px bold white, bottom-left
  - Excerpt: "The platform that pays you to post on social media is officially live. Here's everything you need to know about TaskCoins." in 16px white/80
  - "Read More →" blue link, bottom-right
  - Date: "March 8, 2026" + "5 min read" bottom-left below title

- Category filter bar below hero: "All" (active/blue) | "News" | "Updates" | "Partnerships" | "Guides" | "Community" — horizontal scroll on mobile

- Post grid (3 columns desktop, 1 mobile), 3 posts:
  - Post card 1: placeholder image (blue gradient), "News" badge, "TaskCoins Launches: The Future of Social Media Earning", excerpt 2 lines, "March 8, 2026 • 5 min read", Read More link
  - Post card 2: placeholder (green gradient), "Community" badge, "How 300 Chillers Earned Their First TaskCoins", excerpt, "March 7, 2026 • 3 min read"
  - Post card 3: placeholder (purple gradient), "Guides" badge, "TaskCoins Tokenomics Explained: Why We Built a Utility Token", excerpt, "March 6, 2026 • 7 min read"

**Individual blog post page (/blog/:slug):**
- Hero image (full width, 300px, gradient placeholder)
- Title: 36px Satoshi bold
- Meta row: avatar circle + "TaskCoins Team" + "March 8, 2026" + "5 min read" + category badge
- Content area (max-width 720px, centered):
  - 5 paragraphs of placeholder text, formatted with:
    - Heading 2s in 24px Satoshi
    - Body text in 16px Inter, line-height 1.8, #E5E7EB
    - A blockquote styled with blue left border
    - A bullet list
- Share buttons bar: "Share this article:" + X icon + Telegram icon + Copy link icon
- "Related Posts" section: 2 post cards from the blog grid

---

## PAGE 16: WHITEPAPER (/whitepaper)

**Layout:** two-column on desktop — sticky sidebar (250px) left, content right. Single column on mobile with dropdown TOC.

**Top bar:** "TaskCoins Whitepaper" 28px left, "Download PDF" button (secondary, Download icon) right

**Sidebar — Table of Contents:**
- Sticky, scrolls with page, highlights current section
- Numbered list, each clickable (smooth scroll):
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
- Active section: blue text + blue left border, others #9CA3AF

**Content (max-width 800px, generous padding, readable typography):**
Each section has a heading (28px Satoshi bold) + content (16px Inter, line-height 1.8, #D1D5DB):

Section 1 — Abstract: "TaskCoins is a decentralized micro-task platform that connects advertisers with a global workforce of social media users. The platform is powered by TASK, an ERC-20 utility token on Ethereum. Advertisers purchase TASK tokens to fund campaigns, and Chillers (workers) earn TASK by completing social media distribution tasks. The platform charges a 20% fee on all campaigns, creating sustainable revenue without relying on token sales. This whitepaper outlines the platform architecture, tokenomics, and long-term vision for TaskCoins."

Section 2 — Problem Statement: "The crypto marketing industry is broken. Projects spend millions on marketing agencies that deliver fake followers, bot engagement, and inflated metrics. There is no transparency, no verification, and no accountability. Meanwhile, billions of social media users around the world have real accounts and real audiences — but no way to monetize their social presence for micro-marketing tasks. TaskCoins solves both sides of this equation."

Section 3 — The TaskCoins Solution: "TaskCoins provides a platform where advertisers can distribute content through real social media accounts with verified proof of every post. Chillers (workers) browse a task board, post content on their own accounts across X, Reddit, CoinMarketCap, Binance Square, YouTube, and Telegram, and submit screenshot proof. Every task is verified before payment is released. The result: advertisers get genuine distribution, and Chillers earn crypto for work they can do from their phone."

Section 4 — Platform Architecture: "The platform consists of two primary account types: Advertisers and Chillers. Advertisers create campaigns by defining the content, selecting target platforms, setting reward amounts, and specifying requirements (minimum level, reputation score). Chillers browse available tasks, claim them, post the content on their social media accounts, and submit proof (screenshot + live post URL). An anti-cheat system verifies submissions before releasing payment."

Section 5 — Token Utility: "TASK is the sole currency of the TaskCoins platform. It serves three primary functions: (1) Payment — advertisers must purchase TASK to fund campaigns, creating organic buy pressure. (2) Rewards — Chillers earn TASK for completing tasks, incentivizing participation. (3) Staking — Chillers can stake TASK to unlock premium features and earn bonus rewards, locking supply and reducing sell pressure."

Section 6 — Tokenomics:
- Highlighted box: "Total Supply: 590,000,000 TASK" in large text, blue border
- "Network: Ethereum (ERC-20)"
- "On-chain Tax: None — zero transfer fees on all transactions"
- "The total supply mirrors Solana's circulating supply, providing familiar scale for crypto investors."

Section 7 — Token Allocation:
- Donut/pie chart (animated, colorful):
  - 30% Uniswap Liquidity (blue) — 177,000,000 TASK — "Paired with ETH at launch"
  - 25% Platform Treasury (green) — 147,500,000 TASK — "Operations, bonuses, burns"
  - 15% Team (orange) — 88,500,000 TASK — "12-month vesting schedule"
  - 10% Community Airdrop (purple) — 59,000,000 TASK — "First users and army members"
  - 10% Marketing (yellow) — 59,000,000 TASK — "Listings, influencers, promotions"
  - 10% Staking Rewards (cyan) — 59,000,000 TASK — "Distributed over 24 months"
- Legend below with color dots, label, percentage, and token count

Section 8 — Platform Fee Model:
- Visual flow diagram (3 boxes connected by arrows):
  - Box 1: "Advertiser pays 1,000 TASK" (blue border)
  - Arrow → splits into two:
  - Box 2: "800 TASK → Workers (80%)" (green border)
  - Box 3: "200 TASK → Platform (20%)" (orange border)
- "The 20% fee is applied off-chain at the platform level. The TASK token itself has no transfer tax. This keeps the token CEX-friendly and ensures holders and traders are never penalized."

Section 9 — Burn Mechanism:
- "Every quarter, 5% of the platform's accumulated fees are permanently burned."
- Example box with Flame icon: "Q1 2026: Platform collects 1,000,000 TASK in fees → 50,000 TASK burned forever → Circulating supply decreases"
- "All burn transactions are executed on-chain and publicly verifiable. Burns are announced on the TaskCoins blog and social channels."

Section 10 — Staking Model: table of 4 tiers with amounts and benefits (same as staking page)

Section 11 — Governance Roadmap: "Phase 1: Centralized governance (founding team). Phase 2: Community voting on platform features and fee adjustments (Month 6+). Phase 3: Full DAO governance with on-chain proposals and voting (Year 2+)."

Section 12 — Team: "TaskCoins is built by the team behind Pepeto, a crypto project that achieved a $50M+ market cap. The team has experience in token launches, community building, PR distribution, and platform development. The team operates under KYC verification for CEX listing compliance."

Section 13 — Legal Disclaimer: "TaskCoins (TASK) is a utility token. It is not a security, investment contract, or financial instrument. Purchasing TASK tokens does not represent equity, ownership, or profit-sharing rights in any entity. Users should conduct their own research and consult financial advisors before participating. Crypto assets are volatile and may lose value."

---

## PAGE 17: ROADMAP (/roadmap)

- Hero: "Roadmap" 36px centered, "Our journey from launch to global adoption" 18px #9CA3AF

**Vertical timeline:**
- Center vertical line (2px, gradient from blue to gray going down)
- Cards alternate left and right on desktop, all on one side (right of the line) on mobile
- Each phase connected to the line by a horizontal connector + dot

Phase 1 — Launch (Month 1) — BLUE PULSING DOT (in progress):
- Glass card with blue left border
- "Phase 1" small blue badge, "Launch" 24px bold, "Month 1" #9CA3AF
- Checklist items:
  - ○ Token deployment on Ethereum mainnet
  - ○ Uniswap V2/V3 liquidity pool live
  - ○ TaskCoins.io platform beta launch
  - ○ First 300 Chillers onboarded (from existing army)
  - ○ CoinMarketCap + CoinGecko listing applications
  - ○ First self-funded campaigns live

Phase 2 — Growth (Month 2-3) — GRAY DOT (upcoming):
- Glass card, gray left border
- Checklist:
  - ○ CEX listing (MEXC / LBank)
  - ○ University launch with first 6 courses
  - ○ 1,000 active Chillers
  - ○ Anti-cheat verification system v1
  - ○ Advertiser onboarding campaign
  - ○ First 10 external advertisers

Phase 3 — Scale (Month 4-6) — GRAY:
  - ○ Progressive Web App (mobile)
  - ○ Services marketplace live
  - ○ Staking system launch
  - ○ 5,000 active Chillers
  - ○ First quarterly token burn
  - ○ Proof Gallery launch

Phase 4 — Expand (Month 6-12) — GRAY:
  - ○ Multi-language: Arabic, Spanish, Turkish, Indonesian, Russian, Portuguese
  - ○ Advertiser API for programmatic campaigns
  - ○ Governance voting for token holders
  - ○ 20,000 active Chillers
  - ○ Advertiser Marketplace launch
  - ○ Advanced analytics dashboard

Phase 5 — Ecosystem (Year 2) — GRAY:
  - ○ Native mobile apps (iOS + Android)
  - ○ Additional CEX listings (tier-1 exchanges)
  - ○ Full DAO governance
  - ○ 100,000 active Chillers
  - ○ International expansion across 7+ languages
  - ○ Enterprise advertiser partnerships

Scroll animation: as user scrolls, the center line fills with blue color and dots light up.

---

## PAGE 18: PROOF GALLERY (/proof-gallery)

Public page, no login required.

- Hero: "Proof Gallery" 36px, "Real Tasks. Real Posts. Real Proof." 18px #9CA3AF, "Every task on TaskCoins is verified. Here's the evidence." smaller text

- Filter bar: "All" (active) | X icon "X" | Reddit icon "Reddit" | CMC icon "CMC" | Binance "Binance Sq." | YouTube "YouTube" | Telegram "Telegram"

- Masonry grid (3 columns desktop, 2 tablet, 1 mobile) of proof cards:
  20 cards total. Each card (glass, rounded-xl, overflow-hidden):
  - Top: screenshot placeholder image (varied gradient colors to simulate different screenshots, ~250px tall)
  - Platform icon badge in top-right corner (small colored circle with platform icon)
  - Bottom overlay (dark gradient from bottom):
    - "CryptoKing" username bold 14px
    - "Posted on X" or platform name — 12px #9CA3AF
    - "Verified ✓" small green badge
    - "2 hours ago" timestamp
  - Hover effect: scale 1.02, blue glow border
  - Click: opens lightbox/modal showing the "full screenshot" with details: username, platform, task name, verification timestamp, posted link

- "Load More" button at bottom center (secondary outline)

---

## PAGE 19: ADVERTISER ANALYTICS (/dashboard/advertiser/analytics)

- Heading: "Campaign Analytics" 28px

**Stats row (4 cards):**
- "Tasks Completed" — 847 — CheckCircle purple — "+124 this week" green small text
- "Posts Live" — 823 — Globe green — "98% live rate"
- "Avg Cost Per Post" — 142 TASK — Wallet blue — "-8% vs last month" green
- "Estimated Reach" — 1.2M — Eye orange — "across 6 platforms"

**Charts row (two charts side by side, stacked on mobile):**

Left — "Tasks Completed Over Time" (line/area chart):
- Last 30 days, upward trend
- Blue line, blue/10 area fill
- X axis: dates, Y axis: task count
- Hover tooltip with exact numbers

Right — "Performance by Platform" (bar chart):
- Bars for each platform: X (blue, tallest ~300), Reddit (orange, ~200), CMC (blue, ~150), Binance Square (yellow, ~100), YouTube (red, ~60), Telegram (blue, ~37)
- Horizontal bars or vertical bars, each in platform color

**Top Performing Chillers table (glass card, full width):**
- Columns: Rank | Chiller | Level | Tasks Done | Approval Rate | Avg Response Time | "Hire"
- 10 rows of sample data with "Hire Directly" small blue buttons
- Best performers have 99-100% approval rates

**Campaign Comparison table (glass card):**
- Columns: Campaign | Status | Tasks | Completion Rate | Avg Cost | Reach
- 3 campaigns from dashboard data with metrics

---

## PAGE 20: CHILLER PROFILE (/dashboard/chiller/profile)

**Profile header (glass card, full width):**
- Left: large avatar circle (80px, gradient placeholder with initial letter "A")
- Center: "Ahmed K." 28px bold, "Gold Chiller" with gold badge, "Member since January 2026" #9CA3AF, "Reputation: 87/100" with small gauge
- Right: "Edit Profile" secondary button

**Stats row (4 glass cards):**
- "Tasks Completed" — 186 — CheckCircle
- "Total Earned" — 24,200 TASK — Wallet
- "Reputation Score" — 87/100 — circular gauge green
- "Referrals" — 12 — Users

**Connected Platforms section (glass card):**
- Heading: "Connected Platforms"
- List of platforms with connection status:
  - X (Twitter) — green check "Connected" — "@ahmed_crypto" — "12.4K followers"
  - Reddit — green check "Connected" — "u/ahmed_defi" — "8.2K karma"
  - YouTube — gray X "Not connected" — "Connect" blue button
  - Telegram — green check "Connected" — "@ahmed_task"
  - Instagram — gray X "Not connected" — "Connect" blue button

**Badges/Achievements section (glass card):**
- Heading: "Achievements"
- Grid of badge circles (4 columns):
  - "First Task" — star icon — green (earned) — "Completed your first task"
  - "Century Club" — "100" icon — green (earned) — "100 tasks completed"
  - "Speed Demon" — Zap icon — green (earned) — "10 tasks in one day"
  - "Perfect Score" — CheckCircle icon — blue (earned) — "100% approval on 50+ tasks"
  - "Referral Master" — Users icon — green (earned) — "10+ active referrals"
  - "Diamond Hands" — Diamond icon — gray (locked) — "Hold 10,000+ TASK for 30 days"
  - "Top 10" — Trophy icon — gray (locked) — "Reach top 10 on leaderboard"
  - "Legend" — Crown icon — gray (locked) — "Complete 1,000 tasks"
  - Locked badges: dimmed, lock icon overlay, tooltip showing requirement

**Recent Activity (glass card):**
- "Recent Activity" heading
- 10 activity items (same format as dashboard activity feed)

---

## PAGE 21: ADVERTISER MARKETPLACE (/marketplace)

Public page — advertisers browse Chiller profiles to find the best workers for targeted campaigns.

- Hero: "Advertiser Marketplace" 36px, "Find the Perfect Chillers for Your Campaign" 18px #9CA3AF

**Filter sidebar (left on desktop, top sheet on mobile):**
- "Platform Expertise" — checkboxes: X, Reddit, CMC, Binance Square, YouTube, Telegram
- "Minimum Level" — dropdown: Any, Silver+, Gold+, Diamond+, Legend
- "Reputation Score" — range slider 0-100
- "Follower Count" — dropdown: Any, 1K+, 5K+, 10K+, 50K+
- "Sort By" — dropdown: Most Tasks Completed, Highest Reputation, Newest Members
- "Apply Filters" blue button + "Reset" link

**Chiller profile cards grid (3 columns desktop, 1 mobile):**
15 cards. Each card (glass, rounded-2xl):
- Avatar circle (gradient placeholder) + username bold 18px
- Level badge (colored: Bronze/Silver/Gold/Diamond/Legend)
- Reputation gauge (small circular, showing score /100)
- Platform icons row showing which platforms they're active on (small colored icons)
- Stats: "186 tasks completed" | "Member since Jan 2026"
- Follower count: "12.4K followers on X" if connected
- "Hire Directly" blue button (full width at bottom of card)

Sample Chillers with varied levels (3 Bronze, 3 Silver, 4 Gold, 3 Diamond, 2 Legend), varied reputations (60-98), varied platforms.

**"Hire Directly" modal (opens on button click):**
- Heading: "Send a Direct Task Offer to [username]"
- Select platform dropdown
- Task content textarea
- Reward amount input (TASK)
- Task deadline dropdown (12h/24h/48h/72h)
- "Send Offer" blue button + "Cancel" link

---

## PAGE 22: MY CAMPAIGNS — Advertiser (/dashboard/advertiser/campaigns)

- Heading: "My Campaigns" 28px
- Filter tabs: "All (6)" | "Active (3)" | "Completed (2)" | "Paused (1)"
- "Create New Campaign" blue button top-right

**Campaign cards (stacked list, full width):**
Each card (glass, rounded-2xl, padding 24px):
- Left: campaign title 20px bold + platform icon badges + creation date
- Center: progress section — "67/100 tasks completed" large text + progress bar + percentage
- Right: status badge (green "Active" / blue "Completed" / orange "Paused") + total spend "15,000 TASK"
- Bottom row: "Tasks Completed: 67" | "Posts Live: 65" | "Estimated Reach: 195K" | "Avg Cost: 150 TASK"
- "View Details" blue link + "Pause" outline button (for active) or "Reactivate" button (for paused)

6 sample campaigns:
1. "Launch $TOKEN on X & Reddit" — X, Reddit — Active — 67/100 — 15,000 TASK — 2 days ago
2. "Reddit AMA Promotion" — Reddit — Active — 23/50 — 7,500 TASK — 5 days ago
3. "CMC Community Push Q1" — CMC — Completed — 100/100 — 10,000 TASK — completed 1 day ago
4. "Binance Square Awareness" — Binance — Completed — 75/75 — 11,250 TASK — completed 1 week ago
5. "$TASK Token Awareness" — X, Reddit, CMC, Telegram — Active — 145/300 — 45,000 TASK — 3 days ago
6. "YouTube Comment Campaign" — YouTube — Paused — 12/40 — 6,000 TASK — paused, "Low approval rate" note

**Click a campaign → Campaign Detail view (or modal):**
- Campaign title + status + all details
- Progress bar large
- Budget breakdown: "Reward: 150 TASK × 100 tasks = 15,000 + 3,750 fee = 18,750 total"
- List of all task submissions for this campaign: Chiller avatar + username + status (approved/pending/rejected) + proof screenshot + timestamp
- Quick approve/reject buttons for pending submissions

---

## PAGE 23: SETTINGS (/dashboard/settings)

Works for both Chiller and Advertiser accounts.

- Heading: "Settings" 28px

**Profile Settings section (glass card):**
- Avatar upload area: current avatar + "Change Avatar" button
- Display Name — text input (pre-filled "Ahmed K.")
- Email — text input (pre-filled, with "Verified ✓" green badge)
- Bio — textarea (optional, placeholder "Tell us about yourself")
- "Save Changes" blue button

**Wallet Settings section (glass card):**
- "Connected Wallet" — "0x4f2...8a3" with green dot + "Disconnect" red link
- "Default Withdrawal Address" — text input (pre-filled with wallet address)
- "Connect a Different Wallet" outline button

**Notification Settings section (glass card):**
- Toggle switches (blue when on):
  - "Task approved notifications" — ON
  - "New task available notifications" — ON
  - "Referral signup notifications" — ON
  - "Campaign completion (advertiser)" — ON
  - "Weekly earnings summary email" — OFF
  - "Marketing emails" — OFF

**Security section (glass card):**
- "Change Password" — Current password + New password + Confirm fields + "Update Password" button
- "Two-Factor Authentication" — "Not enabled" badge + "Enable 2FA" outline button

**Language section (glass card):**
- "Platform Language" — dropdown with: English (selected), العربية (Arabic), Español, Türkçe, Bahasa Indonesia, Русский, Português
- "Save Language" button

**Danger Zone section (glass card, red border):**
- "Delete Account" — "Permanently delete your account and all data" — "Delete Account" red outline button

---

## PAGE 24: ADMIN PANEL (/admin)

Internal page — for platform operators only. Different layout from user dashboards.

**Admin sidebar (dark, bg-[#0A0E17]):**
- "TaskCoins Admin" logo at top in red/orange accent
- Menu: Dashboard, Users, Campaigns, Tasks, Finances, Analytics, Blog Manager, Settings
- "Back to Platform" link at bottom

**Admin Dashboard (default view):**
- 6 stat cards top row:
  - "Total Users" — 1,247 — Users icon — "+47 today" green
  - "Active Chillers" — 1,089 — green
  - "Active Advertisers" — 158 — blue
  - "Total Revenue (Platform Fees)" — 287,400 TASK — Wallet — "+12,300 today"
  - "Tasks Today" — 342 — CheckCircle
  - "Pending Reviews" — 12 — Clock orange
- Charts row:
  - Line chart: "Daily Active Users" (30 days)
  - Bar chart: "Revenue per Day" (30 days, TASK amounts)
- Recent activity feed: "New user signup: @newuser123", "Campaign created: Launch $X", "Task flagged by advertiser", "Withdrawal request: 2,000 TASK"

**Admin Users page:**
- Search bar: "Search users by name, email, or wallet..."
- Table: Avatar | Username | Email | Type (Chiller/Advertiser badge) | Level | Reputation | Tasks | Joined | Status (Active/Banned) | Actions
- Actions column: "View" link, "Ban" red button (or "Unban" green), "Edit Level" dropdown
- 20 sample user rows
- Pagination

**Admin Campaigns page:**
- Table: Campaign Title | Advertiser | Status | Tasks (progress) | Spend | Created | Actions
- Actions: "View", "Pause", "Remove" (red)
- 10 sample campaigns

**Admin Finances page:**
- Large stat: "Total Platform Fees Collected: 287,400 TASK" — "≈ $28,740"
- "Treasury Balance: 145,200 TASK"
- "Total Burned: 14,350 TASK"
- Table: "Burn History" — Date | Amount Burned | Tx Hash (truncated) | Status
- Table: "Withdrawal Requests" — User | Amount | Wallet | Requested Date | Status (Pending/Approved/Rejected) | Approve/Reject buttons
- Revenue chart: monthly revenue bar chart (6 months)

**Admin Blog Manager page:**
- "Create New Post" blue button top-right
- Table: Title | Category | Status (Published/Draft) | Date | Actions (Edit/Delete/Unpublish)
- Blog editor (on create/edit): Title input, Slug input (auto-generated), Category dropdown, Content rich text area (large textarea), Featured Image upload, "Publish" / "Save Draft" buttons

---

## IMPORTANT RULES FOR LOVABLE:

1. BUILD ALL 24 PAGES. Every single one. Do not skip any page. Do not say "we'll add this later." Build it now.
2. NO BACKEND. No database. No Supabase. No API calls. This is a VISUAL PROTOTYPE with hardcoded sample data. All data is written directly in the components.
3. Every page must have realistic sample data so the platform looks like it's alive and being used by real people.
4. All navigation links must work. Every sidebar link, every nav link, every button that says "View All" or "View Details" must route to the correct page. Here is the full route map:
   - / → Landing Page
   - /auth → Sign Up / Login
   - /tasks → Task Board
   - /leaderboard → Leaderboard
   - /university → University
   - /services → Services
   - /blog → Blog
   - /blog/:slug → Blog Post
   - /whitepaper → Whitepaper
   - /roadmap → Roadmap
   - /proof-gallery → Proof Gallery
   - /marketplace → Advertiser Marketplace
   - /dashboard/chiller → Chiller Dashboard
   - /dashboard/chiller/my-tasks → My Tasks
   - /dashboard/chiller/staking → Staking
   - /dashboard/chiller/referrals → Referrals
   - /dashboard/chiller/profile → Profile
   - /dashboard/wallet → Wallet (shared by both account types)
   - /dashboard/settings → Settings (shared by both account types)
   - /dashboard/advertiser → Advertiser Dashboard
   - /dashboard/advertiser/create → Create Campaign
   - /dashboard/advertiser/campaigns → My Campaigns
   - /dashboard/advertiser/review → Review Proofs
   - /dashboard/advertiser/analytics → Advertiser Analytics
   - /admin → Admin Panel (internal)
5. Mobile responsive on EVERY page. Test on 375px width.
6. Dark mode only. No light mode toggle.
7. The design must feel PREMIUM — like dYdX, Blur, Phantom wallet. Not cheap, not playful, not corporate. Crypto-native, professional, trustworthy.
8. Use Lucide React for all icons. Use Recharts for all charts. Use React Router for navigation.
9. Transitions and hover effects on all interactive elements. Cards should have hover:border-blue-500/30 transition. Buttons should have hover state changes.
10. Import Satoshi font from Google Fonts or Fontshare for headings. Use Inter (already in most setups) for body text.
11. The Chiller and Advertiser dashboards are SEPARATE experiences with DIFFERENT sidebars and DIFFERENT pages. They must not share the same dashboard layout. A Chiller sees: Dashboard, Task Board, My Tasks, Wallet, Staking, Leaderboard, Referrals, University, Profile, Settings. An Advertiser sees: Dashboard, Create Campaign, My Campaigns, Review Proofs, Analytics, Wallet, Settings.
12. Simulate logged-in state: dashboard pages should show the sidebar and user info as if someone is logged in. The landing page and public pages (leaderboard, proof gallery, blog, whitepaper, roadmap, services, university, marketplace) show the main nav header with Sign Up / Connect Wallet buttons.
