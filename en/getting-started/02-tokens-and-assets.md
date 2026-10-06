# 02 Tokens & Core Assets

## Two game tokens

| Token   | Role                                                                                       |
| ------- | ------------------------------------------------------------------------------------------ |
| **IRT** | Main token: breeding, star-up, tech, skins / some items, tax, milk and some combat rewards |
| **IRG** | Game coin: earned from PVE and similar modes; spent (and burned) on forage and more        |

Some portal events also use **USDT** (e.g. IGO box purchases, certain staking mines).

### How to earn

* **IRT**: Milk Factory output, some Arena rewards, quests / mail / events, market or DEX
* **IRG**: Arena (especially PVE), quests and events, swaps

The client usually has “Swap IRT / Swap IRG” shortcuts to a DEX.

### How to spend

* Feeding forage (mainly IRG)
* Breeding fees, star-up, tech tree, CowShed expansion (mainly IRT)
* Guild shop, skin shop, item shop
* Auto tax when claiming taxed rewards (see [08 Planets & Guilds](../combat-and-guilds/08-guild.md))

***

## Cattle NFTs (the core asset)

Every cattle is an on-chain NFT — the carrier for growth, milk, combat, and breeding.

### Bloodline: Genesis cattle vs Normal cattle

|            | Genesis cattle                                                | Normal cattle                                  |
| ---------- | ------------------------------------------------------------- | ---------------------------------------------- |
| How to get | Extremely rare from boxes, events, high market prices         | Boxes, breeding, market, shard crafting        |
| Lifespan   | Eternal (does not die from lifespan)                          | Has lifespan; dies and is burned when depleted |
| Stars      | No star rank                                                  | 0–3 stars, can star-up                         |
| Stat range | Higher (about 86–100 tier)                                    | Lower (about 60–85 tier; star-up can boost)    |
| Specials   | Can use Genesis avatars, etc.; some life potions do not apply | Can use life potions; can craft from shards    |

### Gender decides playstyle

| Gender   | Key stats                      | Main play                                            |
| -------- | ------------------------------ | ---------------------------------------------------- |
| **Bull** | Combat, stamina, defense, etc. | Arena fights, guild battle offense                   |
| **Cow**  | Milk yield, milk rate, etc.    | Milk Factory staking, heal guardians in guild battle |

Shared stats also include: HP, vitality, growth, XP, and more.

### Cattle states (why a button is grayed out)

What a cattle can do depends on state. Common ones:

* Idle, in CowShed, staked, in combat, feeding, listed, dead

Example: a staked cow must be redeemed before other actions; during a feeding countdown it usually cannot do other activities; dead cattle still occupy stalls until removed.

### Death and extending life

* **Normal cattle** die and burn when lifespan runs out; use **Life Potion (HP pack)** early to extend life
* **Genesis cattle** do not die from lifespan, and generally do not use the HP-pack logic
* Cattle outside the shed keep draining vitality; long neglect risks death (see [03](../growth-and-earnings/03-cowshed-and-growth.md))

***

## Blind box types

| Type                              | Typical drops                                        | Common sources                        |
| --------------------------------- | ---------------------------------------------------- | ------------------------------------- |
| **Cattle blind box (embryo box)** | Genesis (extremely rare), Normal calf, cattle shards | Guaranteed from breeding; events      |
| **IGO Genesis box**               | High-value Genesis / Normal calf / item packs        | Limited portal IGO (often needs USDT) |
| **Skin blind box**                | Random skins                                         | Shops, limited guild shop, events     |
| **UR chests (N–UR Chest)**        | Items / badges / skins / IRT, etc.                   | Events, drops                         |
| **Cattle shard box**              | 1–3 shards                                           | Limited guild shop, etc.              |

**Cattle shards ×10** craft one Normal cattle (see [06 Academy](../growth-and-earnings/06-academy.md)).

***

## Other common on-chain assets

| Asset               | Notes                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Items (ERC1155)** | Forage, boost packs, potions, rename cards, clear tickets, etc. — see [12](../social-and-daily/12-backpack.md) |
| **Skins**           | Change combat look and add stats                                                                               |
| **Badges**          | Equip at the Milk Factory to boost milk hashrate                                                               |
| **Planet NFT**      | Core asset for guild leader identity and tax rights                                                            |
| **Vouchers**        | Portal redemption for forage / items, with thresholds                                                          |

***

## Where to check tokens and assets

* In-game: balance bar, CowShed, backpack, profile stats
* Portal: NFT market, profile, event pages
* Wallet / explorer: contract balances and tx history

Next: [03 CowShed & Growth](../growth-and-earnings/03-cowshed-and-growth.md)
