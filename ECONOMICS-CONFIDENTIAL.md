# TaskCoins — Economics Model (CONFIDENTIAL)

**Do NOT share this document publicly. This is the internal economics breakdown.**

---

## Payment Flow

1. Advertiser sets campaign price in **USDT** (e.g., $500 for 100 posts)
2. Price is always anchored in USDT — never fluctuates with token price
3. Advertiser pays in **TaskCoins** via wallet connect or QR deposit
4. Platform auto-converts at live exchange rate: "10,000 TaskCoins (~$500 USD)"
5. Miner completes task, sees earnings in USDT equivalent: "You earned $5.00 in TaskCoins"
6. Neither side sees the platform split — it happens in the backend

---

## The Halving (Real Mechanism)

Normal platform split: **50% to platform / 50% to miner**

The "halving" is the platform giving up its 50% cut as a bonus to early miners. This bonus decreases (halves) every 6 months until the platform reaches its normal 50% fee.

### Schedule

| Era | Timeline | Miner Gets | Platform Gets | On a $500 Campaign |
|-----|----------|-----------|---------------|-------------------|
| Era 1 | Month 1-6 | 100% | 0% | Miner: $500 / Platform: $0 |
| Era 2 | Month 7-12 | 75% | 25% | Miner: $375 / Platform: $125 |
| Era 3 | Month 13-18 | 62.5% | 37.5% | Miner: $312 / Platform: $188 |
| Era 4 | Month 19-24 | 56.25% | 43.75% | Miner: $281 / Platform: $219 |
| Standard | Month 25+ | 50% | 50% | Miner: $250 / Platform: $250 |

### What Each Side Sees

**Advertiser UI:**
```
Campaign: 100 posts about your project
Price: $500 USD (≈ 10,000 TaskCoins)
[Connect Wallet] [Deposit via QR]
```
No split shown. No percentages. Just the price.

**Miner UI:**
```
Task completed ✓
You earned: $5.00 in TaskCoins (100 TaskCoins)
```
No split shown. They don't know if they got 50% or 100%. They just see what they earned.

**After halving, miner sees:**
```
Task completed ✓
You earned: $3.75 in TaskCoins (75 TaskCoins)
```
They know rewards dropped (the halving). They think "mining rewards decreased like Bitcoin." They don't know the platform started taking a cut.

---

## The Profit Loop

### Era 1 (Month 1-6): Zero Platform Revenue — Maximum Token Growth

Platform earns $0 from fees. But:

- Miners earn 200% (double normal) → they're hyped → they recruit friends
- More miners = more social media posts = more buzz about TaskCoins
- More buzz = more people buying TaskCoins on exchanges
- Token price goes up → boss's liquidity position + token holdings appreciate
- "Halving is coming" narrative drives investor FOMO buying before the event
- YouTubers, Bitcoinomist, CoinDesk PRs all amplify the narrative

**Boss profits from: token appreciation + liquidity profits. Platform fee = $0 but not needed yet.**

### Era 2+ (Month 7+): Platform Revenue Kicks In

- Token already pumped from 6 months of aggressive marketing
- Already profited millions from liquidity + token holdings
- NOW platform starts earning 25% → 37.5% → 50% fee
- Double income stream: liquidity/token profits + platform revenue
- Platform becomes self-sustaining business

### Three Revenue Streams

| Stream | When it kicks in | How it works |
|--------|-----------------|-------------|
| Token holdings | Day 1 | Boss holds allocation. Price goes up from marketing + real platform. Sell or hold. |
| Liquidity position | Day 1 | Provide LP on Uniswap. Profit from trading volume + price appreciation. |
| Platform fee | Era 2 (Month 7) | Starts at 25%, grows to 50%. Real sustainable business revenue from advertiser payments. |

---

## Public Narrative vs Reality

| Public (coin page) | Reality (backend) |
|---|---|
| "Miners earn 2x rewards in Era 1" | Platform gives up its 50% fee as subsidy |
| "Halving cuts mining rewards" | Platform gradually takes back its fee |
| "200% rewards — we pay from our pocket" | Miners just get the full campaign value, platform takes nothing |
| "Fixed 590M supply, deflationary" | True — burns are real |
| "Buy before the halving" | FOMO marketing — halving reduces miner rewards, investors expect price pump |

**Nobody gets scammed:**
- Miners earn real money for real work
- Advertisers get real posts with verified proof
- Investors buy a token backed by a real working platform
- Boss profits from building a real business + smart tokenomics

---

## Miner Level System

Levels affect which campaigns miners can access (higher level = higher-paying campaigns). The halving bonus applies equally to all levels.

| Level | Campaign Access | Example task value |
|-------|----------------|-------------------|
| Bronze | Basic campaigns | $1-3 per task |
| Silver | Medium campaigns | $3-5 per task |
| Gold | Premium campaigns | $5-10 per task |
| Diamond | VIP campaigns + direct offers | $10-25 per task |
| Legend | Highest-paying + auction own slots | $25+ per task |

**In Era 1:** A Bronze miner doing a $3 task earns $3 (200% of their normal $1.50). A Diamond miner doing a $20 task earns $20 (200% of their normal $10).

---

## Key Numbers

- Total supply: 590,000,000 TaskCoins
- Network: Ethereum (ERC-20)
- On-chain tax: ZERO (clean token, CEX-friendly)
- Normal platform fee: 50% (taken off-chain, invisible to users)
- Era 1 effective fee: 0% (full subsidy to miners)
- Halving cycle: Every 6 months
- Target halvings: 4 eras over 24 months → then standard 50/50 forever

---

*This document is CONFIDENTIAL. The public-facing narrative is on the coin page (taskcoins.io). This document explains what actually happens behind the scenes.*
