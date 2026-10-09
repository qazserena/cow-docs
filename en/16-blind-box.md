# 16 Blind boxes — drops and odds

Before you buy, breed, or open a box, you should be able to see **what can drop and at what rate**.  
Figures below come from the current on-chain **initial** configs (breeding-box weights, IGO pool counts, CattleMart pool counts, skin-box rolls). If contracts are upgraded or pools change, **trust the live remaining counts / in-game text**.

Opens use on-chain pseudo-randomness. **Each open is independent.** Except CattleMart’s “shard → Genesis” pity ladder, **breeding boxes and skin boxes have no “N opens guaranteed” pity**. Missing Genesis is normal RNG, not a bug.

Three easy-to-mix-up items:

| Name | What it is |
|---|---|
| **Cattle mystery box (embryo)** | NFT from breeding; open in the in-game Breeding Institute |
| **IGO / CattleMart boxes** | Event boxes bought with USDT on the portal |
| **Skin box** | Item id 20003; open in the in-game backpack for a skin NFT |

---

## 1. Cattle mystery box (breeding embryo)

**Where:** Game client → Breeding Institute → Open.  
**How you get it:** One box per successful breed / rental breed; some events / referral rewards send boxes with no parent data.

**Outcomes (weights sum to 10,000):**

| Outcome | Weight | Initial chance | Notes |
|---|---|---|---|
| **Normal calf** | 9000 | **90.00%** | Roughly 50/50 bull/cow. With parents, general stats follow parents; combat leans father, milk leans mother |
| **Cattle shards** | 999 | **9.99%** | **4 or 5** shards per open |
| **Genesis cattle** | 1 | **0.01%** (1 in 10,000) | Extremely rare; better breed-count rules |

**10** shards craft one Normal cattle at the Academy — see [06](./06-academy.md).

This is **not** a depleting prize pool: every open uses the same weights. Genesis does not get rarer because someone else hit it, and does not get more likely because you opened many times.

---

## 2. IGO Genesis box (portal `/IGO`)

**Where:** Portal IGO page (approve the box, then open).  
**How you get it:** Buy with USDT in the sale window (typical **150 USDT** whitelist / **200 USDT** public; per-address cap; typical supply **1,800** — trust the live page).

**Initial pool (1,800 slots; each win removes one; remaining stock is the weight):**

| Outcome | Initial count | Share at start | You receive |
|---|---|---|---|
| **Genesis cattle** | 100 | **5.56%** | Genesis NFT |
| **Normal cattle** | 300 | **16.67%** | Normal calf NFT |
| **Item pack** | 500 | **27.78%** | A set of growth items (initial typical: Hay ×5, STR Battery ×2, EXP Card ×2, HP Potion ×1, Rename Card ×1) |
| **Skin pack** | 900 | **50.00%** | **1 Skin box** (open again in the game backpack — section 4) |

When a category hits 0, its chance becomes 0 and the others rise. The on-page remaining pool beats this table.

---

## 3. CattleMart / Halo box (portal `/CattleMart`)

**Where:** Portal CattleMart.  
**How you get it:** Typical **20 USDT** per Halo box (whitelist 10% off once, referral rebate); typical supply 20,000.

### 3.1 Open a Halo box (initial pool 20,000)

| Outcome | Initial count | Share at start |
|---|---|---|
| **Planet shard** | 16980 | **84.90%** |
| **CattleMart cattle box** (open again — 3.2) | 2000 | **10.00%** |
| **Calf voucher** | 1000 | **5.00%** |
| **Genesis voucher** | 20 | **0.10%** |

Hitting Genesis / calf / nested box also **adds shards back into the pool**, so later opens skew slightly toward shards. Trust on-chain remaining counts.

Opening and crafting also feed a daily IRG pool split among most opens / most shards spent / last crafter — see the Mart page.

### 3.2 Nested CattleMart cattle box

| Outcome | Chance |
|---|---|
| **Calf** | **50%** |
| **Planet shard ×1** | **50%** |

### 3.3 Craft with planet shards (lottery, not a 1:1 exchange)

| Action | Cost | Possible outcomes |
|---|---|---|
| Craft calf (small) | 5 shards | **10%** another CattleMart cattle box; else 1 shard back + IRG consolation |
| Craft calf (large) | 10 shards | **15%** calf voucher; else 2 shards back + IRG |
| Craft Genesis (pity ladder) | 10, then 20, then 40, then 80 | First two attempts **always IRG** (progress); 3rd about **75%** Genesis voucher; 4th **guaranteed**. Cap 150 shards. Genesis vouchers have a global remaining count |
| Craft Home planet | 50 shards | About **7.5%** Home planet; else IRG |

The craft UI shows remaining Genesis vouchers / planets.

---

## 4. Skin box (in-game backpack)

**Where:** Use “Skin Box” in the backpack.  
**How you get it:** Shops, limited guild shop, IGO skin pack, vouchers, event mail.

Each open rolls 1–100 among these five skins:

| Skin | Initial chance |
|---|---|
| Baby Bomber | **30%** |
| Evil Blaze Dryad | **30%** |
| Space Explorer | **15%** |
| Electric-Arc Spirit | **15%** |
| Holo Electro-Magnetizer | **10%** |

You get a skin NFT to equip. Multiple common skins can craft an Ultimate skin — see [12](./12-backpack.md).

---

## 5. UR chests

N–UR chests from the Ladders weekly ranking and events are **not** a loot roll: each chest pays a **fixed** set, all of it, with no hidden second table.

| Chest | Contents | Source |
|---|---|---|
| **N** | EXP Card ×3, STR Battery ×3, 800 IRT | Events |
| **R** | Prime EXP Card ×3, Prime Battery ×3, HP Potion ×1, 1200 IRT | Events |
| **SR** | Prime EXP Card ×5, Prime Battery ×5, HP Potion ×1, 1500 IRT | Ladders ranks 11–50 |
| **SSR** | Supreme EXP Card ×5, Supreme Battery ×5, Prime HP Potion ×1, 3500 IRT | Ladders ranks 4–10 |
| **UR** | Supreme EXP Card ×9, Supreme Battery ×9, Supreme HP Potion ×1, 5000 IRT | Ladders ranks 1–3 |

---

## 6. Cattle shard box

The “Cattle Piece Box” item text says it grants a few cattle shards. The backpack currently **does not show it and has no separate open button** (unlike the skin box). If an event mails shards directly, follow that event. This page does not invent unpublished percentages.

---

## How to open / what to watch

1. Open at the **right place**: breeding boxes in the game; IGO / Mart boxes on the portal.  
2. On-chain opens need approval and Gas; check the contract and amount before confirming.  
3. After a cattle drop, put it in the **CowShed** in the client.  
4. Normal **adult** cattle cannot be listed on the NFT market — trade before adulthood if you plan to sell. See [13](./13-market.md).

Related: [05 Breeding](./05-breeding.md) · [02 Assets](./02-tokens-and-assets.md) · [14 Portal](./14-portal.md) · [15 FAQ](./15-faq.md)
