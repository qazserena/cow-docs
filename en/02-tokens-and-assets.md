# 02 Tokens & Core Assets

## Two game tokens

| Token | Use |
|---|---|
| **IRT** | Main token: breeding, star-up, tech, expansion, items / skins, entry fees, federation applications, tax, milk & combat rewards |
| **IRG** | Game gold: main output of PVE win chests and quests; spent (and burned) on hay and breeding |

During beta they are called **TIRT / TIRG** (test tokens) with identical rules. Some portal events use **USDT** (IGO boxes, Interstellar Mining, marketplace settlement).

### How to earn

| | IRT | IRG |
|---|---|---|
| In game | Milk Factory, Match win chest, on-chain PVP battle report, guild benefits, Ladders weekly chest, quests / mail | PVE win chest, quests (most common), chests |
| Portal | Year-End Staking, airdrops, beta starter pack | Interstellar Mining (USDT staking), CattleMart FOMO pool, daily supply, airdrops |
| Trading | "IRT Exchange / IRG Exchange" in the client balance bar → DEX | Same |

### Where it goes (common prices, current config)

| Spend on | Token | Amount |
|---|---|---|
| Hay normal / prime / supreme | IRG | 100 / 200 / 300 |
| EXP card, STR battery normal / prime / supreme | IRT | 100 / 200 / 300 |
| HP potion normal / prime / supreme | IRT | 4000 / 8000 / 12000 |
| Rename card | IRT | 300 |
| Shed expansion (slot 3 onward) | IRT | 500 → 3200 rising |
| Breeding (1st – 5th time) | IRT + IRG | 100 – 500 IRT + 100k – 500k IRG |
| Tech tree (one node to max) | IRT | 1000 |
| Skins | IRT or USDT | 625 / 935 / 1250 USD-equivalent |
| Guild entry fee | IRT | set by leader |
| Federation planet application | IRT | 500 deposit + bid |
| Frontier → Home upgrade | IRT | 500 USD-equivalent |

Taxable income (milk, Match win chest, PVP report, rental income) is taxed automatically on claim — see [08](./08-guild.md).

---

## Cattle NFTs (the core asset)

Every cattle is an on-chain NFT and the vehicle for raising, milk, combat, and breeding.

### Bloodline: Genesis vs Normal

| | Genesis | Normal |
|---|---|---|
| Source | 1-in-10,000 from boxes, IGO / CattleMart, beta pack, marketplace | 90% of boxes, breeding, 10 shards crafting, marketplace (calves only) |
| Lifespan | **Eternal** | Finite; dies and burns when it runs out |
| Stars | None, stats apply at **100%** | 0 – 3 stars, stats scaled by star multiplier (below) |
| Base stats | 8000 – 12000 | Calves 4000 – 5000 (parents' average when bred); event / pack adults 6000 – 8000 |
| Growth | Born adult | Must be fed to 30,000 growth |
| Breeding | 5 times + unlimited via breed cards | 5 times max |
| Transfer & trade | Free wallet transfer, always sellable | **No direct wallet transfer**; marketplace only, and **only calves can be listed** |
| Life extension | Not needed, HP potions not allowed | HP potions, max +10 days total |
| CowShed | Genesis bulls cannot leave for 24 h after entering | — |

### Gender decides gameplay

| Gender | Specific stats | Main play |
|---|---|---|
| **Bull** | Attack, Stamina, Defense | Arena combat, guild battle attack, charging the energy station |
| **Cow** | Milk, Milk Rate | Milk Factory staking, healing the guardian in guild battle |

Shared stats: Life (lifespan length), Energy cap, Growth.

### Star multiplier (must-read for Normal cattle)

A Normal cattle's displayed and effective stats are base × star multiplier:

| Stars | 0 | 1 | 2 | 3 | Genesis |
|---|---|---|---|---|---|
| Multiplier | **25%** | 40% | 60% | 80% | 100% |

A 0-star bull with base 4800 attack actually has 1200; at 3 stars, 3840. Star-up is the main way to make Normal cattle stronger — see [06](./06-academy.md).

### Lifespan

- Normal lifespan = **35 days × Life ÷ 10000**: calves ≈ 14 – 17 days, pack adults ≈ 21 – 28 days  
- HP potions add at most **10 days** total per cattle  
- **Star-up resets lifespan to full** (and at least 30 days) — the other way to "extend life"  
- When time runs out the cattle is dead; it still occupies a slot and is burned when removed from the shed  

### Cattle states (why a button is greyed out)

Idle, In Shed, Staking, In Battle, Feeding, Listed, Dead.

- A staking cow must be redeemed before breeding / removal  
- During the feeding countdown (10 – 20 min per hay) nothing else is possible  
- After breeding: 3-day cooldown (tech can shorten)  

---

## Boxes

| Type | Drops | Source |
|---|---|---|
| **Cattle box (embryo)** | Normal calf 90%, shards 9.99% (4 – 5), Genesis 0.01% | Breeding; referral reward; beta pack |
| **IGO Genesis box** | Genesis / Normal / item pack / skin pack (prize pool) | Portal IGO (USDT) |
| **Skin box** | 5 skins (30 / 30 / 15 / 15 / 10%) | Shop, guild shop, IGO skin pack, vouchers |
| **N – UR chests** | Fixed item bundle + IRT, not random | Ladders weekly ranking, events |
| **Shard box** | A few shards | Events |

Full counts and percentages: **[16 Blind Box Odds](./16-blind-box.md)**. **10 shards** craft one Normal cattle (see [06](./06-academy.md)).

---

## Other on-chain assets

| Asset | Notes |
|---|---|
| **Items (ERC1155)** | Hay, EXP cards, batteries, HP potions, rename cards, pass cards… see [12](./12-backpack.md) |
| **Skins (ERC721)** | Change combat look and add stats; craftable into the ultimate skin |
| **Badges (ERC721)** | Equip at the Milk Factory for hashpower, Bronze → Master (6 tiers) |
| **Planet NFT** | Home / Frontier / Federation; leadership and tax rights |
| **Avatar NFT** | Issued automatically at birth / adulthood; switch avatar in profile |
| **Voucher NFT** | Redeem at the portal Voucher Center for hay, items, skin boxes… |

---

## Where to look

- In game: balance bar, CowShed, Backpack, Profile (cattle stats, cumulative IRT / IRG income)  
- Portal: Card Package `/profile` (all NFTs with details), NFT Marketplace, event pages  
- Wallet / explorer: contract balances and transaction history  

Next: [03 CowShed & Growth](./03-cowshed-and-growth.md)
