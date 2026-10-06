# 08 Planets & Guilds

In Legend Ranch, a **planet ≈ a guild**. After you bind a planet, tax, benefits, and guild battles all revolve around it.

> Important: **binding is generally permanent**. Choose carefully.

## Planet types

| Type                  | Traits (concept)                                                                                                      |
| --------------------- | --------------------------------------------------------------------------------------------------------------------- |
| **Home planet**       | Top-tier planet, large population; leader controls tax and governance                                                 |
| **Federation planet** | Founded by Home members under IRT and other conditions; most tax goes to the Federation leader, some remitted to Home |
| **Frontier planet**   | Founded under special conditions; rights similar to Home-class settings                                               |

Exact create conditions, capacity, and rates follow the game and contracts.

***

## Ranks

Common ranks, low to high:

**Trainee → Member → Elite → Vice Leader → Leader**

* Leader: change tax rate (within a band), notices, icon, join rules (entry fee, approval), set ranks, approve join requests, kick members, send benefits, sign up for guild battle, etc.
* Vice Leader: approve join requests and kick members of lower rank; cannot set ranks or change guild settings
* Elite: below Vice Leader; exact permissions follow in-game settings
* Member / Trainee: pay tax, claim benefits, join combat and quests

Some notices and renames have cooldowns (e.g. once every 30 days).

***

## Tax and contribution

When you claim **taxed IRT rewards** (milk, some combat rewards, taxed mail, etc.):

1. The system deducts tax at the planet **tax rate** (common default \~20%; leaders can adjust roughly 10%–20%)
2. The deducted amount counts as your **contribution**
3. Tax enters the guild tax pool, managed by the leader

Tax-free claims skip this deduction.

***

## Guild benefits

Leaders can configure and send two benefit types (members view and claim under “Guild Benefits”):

### Daily benefits

1. After tax accumulates, the leader **funds** part of it into the benefit pool
2. Set **share ratios** by rank (Vice / Elite / Member / Trainee; sum to 100%)
3. Click **Distribute rewards**
4. Members claim within the valid window (**the leader usually cannot claim daily benefits**)
5. Members who joined that day often cannot claim the same day

### Plunder benefits

From the **winning side’s guild battle plunder** pool, shared by contribution rank tiers.\
Details: [09 Guild Battle](09-guild-battle.md).

Claiming benefits usually costs your own Gas; rewards may go through the Reward Center / on-chain claim flow.

***

## Joining a guild: open vs. approval

The Leader has two join switches under Guild Management → Settings:

| Setting                | Effect                                                                                    |
| ---------------------- | ----------------------------------------------------------------------------------------- |
| Entrance fee           | Joining costs IRT                                                                         |
| Join approval required | Players cannot join directly; they must apply and be approved by the Leader / Vice Leader |

Approval flow:

1. Select Planet → Join Guild. For an approval guild the button reads **Apply**. Only one pending application at a time; use **Cancel Application** to withdraw.
2. The Leader / Vice Leader sees it under Guild Management → Applications and approves or rejects.
3. Once approved, the button becomes **Confirm Join**; confirm with your wallet to bind on-chain. An approval expires after **24 hours** if not confirmed.
4. Quick Join prefers guilds without approval; if all require approval it applies to the first one.

## Kicking members

* The Leader can kick anyone except themselves; a Vice Leader can only kick members of lower rank (Trainee / Member / Elite).
* Path: Guild Management → Members → member settings → **Kick**. The operator's wallet sends one on-chain transaction.
* A kicked player who is online is notified and returned to planet selection and may join another guild; entrance fees are not refunded.
* The member list syncs from chain to the portal; the headcount may lag a few seconds.

***

## Applying for a Federation planet

Home members can apply to the leader to found a Federation planet:

1. Submit a bid (IRT, etc.) and a proposed tax rate (must be below the Home rate cap)
2. Leader reviews
3. On approval, a new Federation planet is minted on-chain

***

## Guild shop

* **Standing**: Clear Tickets, Point Protection Cards, PVE Power Cards, etc.
* **Limited-time**: packs, shard boxes, skin boxes, badge shards, Guardian Armor, Power Potions, etc.
* Often includes free daily refreshes

Guilds have level, points, and rank: wins add points, losses subtract (exact numbers adjustable).

***

## Guild quests

Quests have a “Guild” tab — e.g. party Arena, 5v5, pay tax, form intimacy bonds, join guild battle.\
See [11 Daily Play](../social-and-daily/11-daily.md).

***

## Player FAQ

**Q: Why did my milk claim come up short?**\
A: Planet tax was deducted. Check the rate on the guild screen.

**Q: I sent daily benefits but can’t see them myself?**\
A: Leaders don’t share in daily benefits — check with another rank account.

**Q: Benefits were sent but members can’t see them?**\
A: Check whether distribute succeeded, whether they expired, whether the member joined today, and whether their rank is in the share list.

**Q: The join button says "Apply" / joining fails?**\
A: That guild requires approval. Apply, wait for the Leader or Vice Leader to approve, then come back and press **Confirm Join** within 24 hours.

**Q: I'm a Vice Leader — why can't I set ranks?**\
A: Rank changes and guild settings remain Leader-only; Vice Leaders can approve join requests and kick lower-rank members.

Next: [09 Guild Battle](09-guild-battle.md)
