# KAERU PROTOCOL
## A Rugless Token Standard on Solana
### v0.5 — Draft

*by @kaeru_net*
*Updated: March 2026*

---

## 1. Problem

The crypto space is broken by trust.

Every day, thousands of tokens are launched on Solana. Most of them rug. Developers take liquidity, dump their holdings, and disappear. Buyers are left with nothing.

The problem is not just greed. The problem is that the system makes rugging easy:

- Developers hold large amounts with no lockup
- Bots and coordinated wallets buy before humans can react
- Liquidity is never locked
- There is no cost to lying

But there is a deeper irony.

People escaped banks because they couldn't trust them. Then they invested in anonymous developers who are even less accountable. The problem was never banks. It was trust. And crypto hasn't fixed it — it made it worse.

Platforms profit whether you win or lose. Every rug generates fees. The scammer and the victim are both customers.

We need a new standard. Not just promises. A system where rugging is structurally impossible.

---

## 2. Our Story

This protocol was born from personal experience.

The founder of KAERU was rugged. Not once. The pain of watching trust get exploited — watching a developer disappear with funds — is what drives this project.

$KAERU was launched on pump.fun as the first honest step. No team. No VC. Tiny dev hold. No lies.

But a single honest coin is not enough. We need a protocol.

The greatest proof of trust in crypto history was Satoshi disappearing. When the creator left, Bitcoin became truly trustless. That is the standard we are building toward — a system that doesn't need us to be honest. A system that makes dishonesty structurally impossible.

---

## 3. The World of KAERU

### KAERU NETWORK

KAERU NETWORK is the overarching vision. An ecosystem where honest tokens are the default, not the exception.

### KAERU POND

Inside KAERU NETWORK lives **KAERU POND** — the launchpad. A place where tokens are born with honest structure baked in from the start.

Every token that emerges from KAERU POND is built on KAERU PROTOCOL — the rugless token standard.

```
KAERU NETWORK（the ecosystem）
　└── KAERU POND（the launchpad）
　　　　├── $KAERU（the origin）
　　　　├── $POND（the first born）
　　　　└── ...（future tokens, all rugless）
```

### The Two Tokens

**$KAERU** — The foundation. The origin. Launched on pump.fun before the protocol existed. Holding $KAERU means you believed in honest crypto from the beginning.

**$POND** — The first token born from KAERU POND. Built entirely on KAERU PROTOCOL. The proof that the system works.

---

## 4. Solution: KAERU PROTOCOL

KAERU PROTOCOL is a rugless token standard on Solana.

The goal is simple: make rugging structurally impossible, and make honesty the default.

### Core Principles

- **Fixed supply** — no minting after launch
- **Dev lock** — developer tokens are locked
- **Permanent LP lock** — liquidity cannot be removed
- **Bot resistance** — bots are taxed, not rewarded
- **Sell tax + auto buyback** — sell pressure becomes buy pressure
- **Dev neutralization** — once deployed, the dev cannot interfere

### The Key Insight

Other launchpads lock LP. That prevents the dev from running.
But it doesn't prevent coordinated dump attacks.

KAERU PROTOCOL addresses both — with three independent layers of defense.

---

## 5. Tokenomics Design

### 5.1 Fixed Supply
Total supply is fixed at launch. No new tokens can ever be minted. This removes one of the most common rug vectors.

### 5.2 Gradual Supply Release
Inspired by Bitcoin's mining schedule, tokens are not all available at once.

```
Total Supply: Fixed
↓
Launch: Small amount available
↓
Over time: Gradually released
```

This prevents early whales from buying everything and dumping.

### 5.3 Dev Lock
Developer tokens are locked for a fixed period. Selling before unlock is structurally impossible.

### 5.4 Permanent LP Lock
Liquidity is locked permanently at launch. The developer cannot remove it.

### 5.5 Dev Neutralization
Once the contract is deployed, the developer loses all privileged access. There are no admin functions. No upgrade keys. No hidden backdoors. The dev cannot interfere — even if they wanted to.

This is not a promise. It is enforced by code.

---

## 6. Three-Layer Defense Against Manipulation

KAERU PROTOCOL uses three independent systems to protect against bots, coordinated dumps, and panic selling.

### Layer 1 — Time-based Bot Tax

```
0–10 seconds   → 50% tax
10–30 seconds  → 30% tax
30–60 seconds  → 15% tax
1–5 minutes    →  5% tax
5 minutes+     →  0.25% (industry standard)
```

**Why this works:**
- Bots that buy instantly pay a heavy tax
- Humans who wait 5 minutes pay the normal rate
- Distributed wallets buying simultaneously are all taxed equally — wallet count is irrelevant
- *"Patience is rewarded. Panic is taxed."*

### Layer 2 — Kaeru Egg 🥚

**The problem this solves:**

A sophisticated attacker can distribute funds across hundreds of wallets and dump simultaneously — bypassing bot tax by acting like many slow humans.

**The solution:**

Any purchase made within the high-tax window (first 60 seconds) triggers a **Kaeru Egg** — a random lock period applied to that purchase.

```
Buy within 60 seconds of launch
↓
Kaeru Egg triggered
↓
Random lock: anywhere from 1 second to 24 hours
↓
Cannot sell until lock expires
```

**Why randomness matters:**

If the lock were fixed (e.g. always 24 hours), attackers could plan around it. Random duration makes coordinated dump attacks structurally unpredictable.

### Layer 3 — Sell Tax + Auto Buyback

**The problem this solves:**

Even after the launch window, large holders can slowly dump their position — gradually depressing price without triggering bot tax.

**The solution:**

A sell tax is applied to all sells. Revenue is automatically used to buyback tokens from the market and burn them.

```
Sell occurs
↓
Sell tax collected into pool
↓
When pool reaches threshold
↓
Auto buyback executed
↓
Bought tokens are burned
↓
Total supply decreases
↓
Remaining tokens become more scarce
```

**Why this works:**

- Sell pressure is partially converted into buy pressure
- Every seller contributes to the value of remaining holders
- The more selling occurs, the more deflationary the token becomes
- No human controls the buyback — it executes automatically

*"Those who leave fund those who stay."*

### Dev Hold Cap

- Developer hold is capped at ≤ 10%
- Dev tokens are locked
- No surprise dumps from the inside

---

## 7. Tax Distribution

Tax revenue evolves across phases.

### Phase 1 — KAERU POND launches $POND

```
Trade
↓
0.3% fee total
↓
├── 0.1% → Burned
├── 0.1% → LP
└── 0.1% → $KAERU holders (SOL rewards)
```

### Phase 2 — KAERU POND becomes open launchpad

```
Trade (any token born from KAERU POND)
↓
0.3% fee total
↓
├── 0.05% → Burned
├── 0.05% → LP
└── 0.20% → $KAERU holders (SOL rewards)
```

```
More tokens born from KAERU POND
↓
More bots pay tax
↓
More SOL flows to $KAERU holders
↓
$KAERU becomes more valuable
↓
More devs want to launch on KAERU POND
```

---

## 8. Jackpot Pool (Optional)

```
Trade
↓
0.1% → Jackpot Pool

Every 100 trades
↓
1 random trader wins the pool
```

---

## 9. The Role of $KAERU

$KAERU is the origin. The foundation. The reason KAERU POND exists.

### Why hold $KAERU?

**1. SOL rewards**
Every token born from KAERU POND flows bot tax and sell tax to $KAERU holders — automatically. The bigger the pond grows, the more SOL flows.

**2. Priority access**
$KAERU holders get into new KAERU POND launches before the public.

**3. Trust proof**
Holding $KAERU from the beginning is proof that you believed in honest crypto before it was the standard.

**4. Growing rewards**
Phase 1: 0.1% of bot tax. Phase 2: 0.2% across every token in the pond.

### The flywheel

```
More tokens born from KAERU POND
↓
More honest tokens exist in the world
↓
KAERU PROTOCOL becomes the trust standard
↓
More devs want to launch from KAERU POND
↓
More SOL flows to $KAERU holders
```

---

## 10. Roadmap

### Phase 0 — The Origin
*Now*

- $KAERU lives on pump.fun
- Building community and trust
- KAERU PROTOCOL whitepaper published
- Reaching graduation ($69K market cap)
- LP locked on graduation

### Phase 1 — $POND is born
*Next*

- KAERU POND launches $POND on Solana
- Full KAERU PROTOCOL: bot tax + Kaeru Egg + sell tax + auto buyback + dev lock + fixed supply
- Bot tax: 0.1% burn / 0.1% LP / 0.1% → $KAERU holders in SOL
- Proof that the system works
- $KAERU holders get priority access

### Phase 2 — KAERU POND opens
*Future*

- KAERU POND becomes an open launchpad
- Any developer can launch using the audited standard
- Every token's bot tax flows to $KAERU holders (0.2%)
- The pond keeps growing

### The Big Picture

```
$KAERU (Phase 0) — the origin
↓
$POND (Phase 1) — the proof
↓
KAERU POND open (Phase 2) — the ecosystem
↓
Every honest token strengthens the pond
```

---

## 11. What We Are NOT

- We are not a pump and dump
- We are not paying for promotions or shills
- We are not making promises we cannot keep
- We are not hiding who we are
- We are not asking you to trust us — we are building a system that doesn't require it

---

## 12. Open Questions (TBD)

| Question | Options | Status |
|----------|---------|--------|
| Kaeru Egg trigger | Per purchase vs. first purchase per wallet | Under discussion |
| Kaeru Egg threshold | Fixed (60s) vs. dynamic based on volume | Under discussion |
| Sell tax rate | 0.25% – 1% range | Under discussion |
| Auto buyback threshold | Fixed pool size vs. time-based trigger | Under discussion |

---

## 13. Conclusion

Trust is the only real utility in crypto.

KAERU PROTOCOL is an attempt to make trust structural — not just a promise, but a system.

Three layers of protection. Honest tokenomics. A dev that cannot interfere even if they wanted to.

The pond is small. The pond is early. The pond is honest.

*No rug. Just honest frogs. 🐸*

---

## Contact

- Twitter: [@kaeru_net](https://twitter.com/kaeru_net)
- Telegram: [t.me/kaeru_network](https://t.me/kaeru_network)
- Website: [kaeru-network.github.io/kaeru-network](https://kaeru-network.github.io/kaeru-network)
- $KAERU CA: `3V9N5MH5ZnTWrka1Z98iTY3ByfUzrK7bwpwr5d2kpump`

---

*v0.5 — This is a living document. Details will be updated as the protocol develops.*
