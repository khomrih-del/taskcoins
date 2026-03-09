This is a content and naming correction pass. Do NOT rebuild any sections — only change the text and values listed below. Keep all existing design, layout, animations, and styles exactly as they are.

---

## PART 1: NAMING FIX — "TASK" → "TaskCoins"

The coin is called "TaskCoins" (full name). "TASK" is just the exchange ticker. Apply these changes everywhere on the page:

1. **Hero heading:** Change "Mine TASK" → "Mine TaskCoins"
2. **Both navbar buttons:** Change "Buy $TASK" → "Buy $TaskCoins"
3. **"What Is Attention Mining" subheading:** Change "TASK miners use their social media" → "TaskCoins miners use their social media"
4. **"What Is Attention Mining" left paragraph:** Change "Every block earns TASK tokens" → "Every block earns TaskCoins"
5. **Tokenomics heading:** Change "$TASK Tokenomics" → "$TaskCoins Tokenomics"
6. **Tokenomics supply line:** Change "590,000,000 TASK" → "590,000,000 TaskCoins"
7. **CTA section "Buy $TASK" button:** Change → "Buy $TaskCoins"

Do a full scan of the page — if there are ANY other places where "TASK" appears alone (not as part of "TaskCoins"), change it to "TaskCoins". The only exception: inside code/contract address areas, "TASK" as a ticker symbol is fine.

---

## PART 2: HALVING MODEL FIX — Fixed amounts → Multipliers

The old model showed fixed token amounts per block (100/50/25/12.5 TASK). The correct model uses REWARD MULTIPLIERS — miners earn a bonus percentage that decreases each era. This is the biggest change.

### Halving Schedule Cards — Replace all 4 cards' content:

**Card 1 — Era 1 (ACTIVE — keep the blue glowing border and pulsing dot):**
- Big number: **"2x"** (replace "100")
- Below the number: **"Mining Rewards"** (replace "TASK per block")
- Timeline: "Months 1–6" (keep)
- Subtitle: "Current Era — Mine Now" (keep)

**Card 2 — Era 2 (UPCOMING — keep dimmed with lock icon):**
- Big number: **"1.5x"** (replace "50")
- Below the number: **"Mining Rewards"** (replace "TASK per block")
- Timeline: "Months 7–12" (keep)
- Subtitle: "After Halving #1" (keep)

**Card 3 — Era 3 (UPCOMING):**
- Big number: **"1.25x"** (replace "25")
- Below the number: **"Mining Rewards"** (replace "TASK per block")
- Timeline: "Months 13–18" (keep)
- Subtitle: "After Halving #2" (keep)

**Card 4 — Era 4 (UPCOMING):**
- Big number: **"1x"** (replace "12.5")
- Below the number: **"Mining Rewards"** (replace "TASK per block")
- Timeline: "Months 19–24" (keep)
- Subtitle: "Standard Rate" (keep)

### Text below the halving progress bar:

DELETE: "Mining pool: ~200,000,000 TASK allocated. Once it's mined — no more new tokens. Ever."

REPLACE WITH: "Early miners earn double rewards. Each halving cuts the bonus until rewards reach standard rate. The window is closing."

---

## PART 3: COMPARISON TABLE FIX

In the "Bitcoin Mining vs Attention Mining" table:

Change the **"Block reward"** row, TaskCoins column:
- FROM: "100 TASK"
- TO: "2x rewards (Era 1)"

Everything else in the table stays the same.

---

## PART 4: HERO SECTION TEXT FIX

Change the italic text below the countdown timer:

FROM: "Early miners earn 100 TASK per block. After the halving — only 50."

TO: "Early miners earn 2x rewards. After the halving — rewards drop by half. Mine now."

---

## PART 5: HOW MINING WORKS — CARD 03 FIX

Card 03 "Collect Rewards" — change the description text:

FROM: "Verified blocks earn 100 TASK — until the halving. After that, only 50. The earlier you start mining, the more you earn. Forever."

TO: "Verified miners earn 2x rewards in Era 1. After the halving, the bonus drops. The earlier you start mining, the more you earn. Forever."

---

## PART 6: CTA SECTION FIX (blue gradient section at bottom)

Change the subtitle text:

FROM: "Every day you wait, miners are earning 100 TASK per block. After the halving — only 50. Don't be late."

TO: "Every day you wait, miners are earning 2x rewards. After the halving — only 1.5x. Don't be late."

---

## PART 7: ROADMAP TEXT FIX

Fix the halving references in the roadmap phases:

**Phase 3 — "First Halving":**
Change: "HALVING #1: Rewards drop from 100 → 50 TASK"
To: "HALVING #1: Mining rewards drop from 2x → 1.5x"

**Phase 4 — "Network Effect":**
Change: "HALVING #2: Rewards drop to 25 TASK"
To: "HALVING #2: Mining rewards drop from 1.5x → 1.25x"

**Phase 5 — "Mining Empire":**
Change: "HALVING #3: Rewards drop to 12.5 TASK"
To: "HALVING #3: Mining rewards drop from 1.25x → 1x (standard rate)"

---

## PART 8: MINOR LAYOUT FIX

The "Human Only" card in the Proof of Attention section — the description text ("Device fingerprint, account age verification, duplicate detection, and rate limiting. Galxe has 90% bots. We have zero.") is getting cut off at the bottom. Make sure the card has enough padding/height to show the full text without clipping.

---

## SUMMARY OF ALL CHANGES

This prompt changes ONLY text content. Zero layout, design, color, animation, or structural changes.

- 7+ instances of "TASK" → "TaskCoins" (naming fix)
- 4 halving cards: fixed amounts → multipliers (2x/1.5x/1.25x/1x)
- 1 removed paragraph (fake "200M mining pool")
- 5 text blocks updated to use multiplier language (hero, card 03, CTA, comparison table, below halving bar)
- 3 roadmap items updated
- 1 minor layout fix (Human Only card text clipping)
