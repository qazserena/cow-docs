# 08 Planets & Guilds

In Interstellar Rangeland, **planet ≈ guild**. After you bind a planet, tax, benefits, and guild battles all revolve around it.

> Important: **you cannot change planets by yourself after binding**. The only exits are being kicked by the leader / vice leader, or founding your own guild with a planet card. Choose carefully.

## Planet types

| Type | Role | How to get | Population cap | Tax | Federation slots | Guild battle |
|---|---|---|---|---|---|---|
| **Home planet** | End-game planet, the "great powers" | **One per beta starter pack**; tradable; Frontier upgrade | 10,000 | 20% | up to 100 | Can sign up |
| **Frontier planet** | Starter planet, "pre-Home" | Event hand-outs (early beta packs issued some); not tradable | 5,000 | 10% | not open in beta | Cannot sign up (battle pool still accrues) |
| **Federation planet** | Affiliate of a Home | Home member applies, Home leader approves → minted | 1,000 | set on application (< 20%); members actually pay the mother Home's 20% | — | Fights with the mother planet |

Rates are fixed by type and **leaders cannot change them**. Values come from the on-chain contract.

### Frontier vs Home — the real difference

**Same**: a Frontier planet is a sovereign planet, not anyone's affiliate. Founding, ranks, notice / icon, entry fee, join approval, kicking, daily benefits, guild quests, guild shop, tax — all identical to Home.

**Different**:

- Smaller: population 5,000 (Home 10,000), tax 10% (Home 20%). Lighter tax helps recruiting; the leader earns less.  
- No external power: cannot sign up for guild battle, cannot approve Federation planets; guild-battle quests don't appear in the list.  
- Battle pool still accrues: the 30% of tax routed to the battle pool accumulates and becomes usable after upgrading.  
- Upgradable: leader → "Guild Management → Settings → Upgrade to Home", burning about **$500 worth of IRT** (converted at the IRT price at upgrade time; the dialog shows the exact amount and the accrued battle pool). Population, federation slots, tax, and guild-battle eligibility unlock at once.  

> Every beta starter pack carries a Home card — "everyone can found a guild and fight guild battles" is deliberate, to stress-test the guild system. Frontier holders (early packs or events) who want guild battles can upgrade to Home or join someone's Home.

### Founding your own guild

An address holding a Home / Frontier card and not bound to any planet can **Create Guild** on the planet screen: the card is deposited in the contract, you become leader and are bound automatically.

- One address can lead only one planet and cannot be a member elsewhere at the same time  
- The leader can **withdraw the card** (give up leadership and take the card back); not while the planet is leased  
- If the card changes hands, the new holder uses "Take Over" to become leader  

---

## Ranks

Five tiers, low to high: **Trainee → Member → Elite → Vice Leader → Leader** (new members start as Trainee).

- **Leader**: notice, icon, rename, join settings (entry fee, approval), set ranks, approve joins, kick, fund and distribute benefits, withdraw tax, sign up for guild battle, pick fighters, armor the guardian, approve federation applications  
- **Vice Leader**: approve join requests, kick members below their rank; cannot set ranks or change settings  
- **Elite / Member / Trainee**: pay tax, claim benefits, fight and quest; rank affects daily-benefit shares  

Leadership comes from the on-chain planet card (synced by the portal); ranks are set by the leader in the member list "Set Position" (tiers 0 – 3) and affect the next benefit claim immediately.

### Notice, rename, icon

- Guild name: 2 – 6 Chinese characters or at least 3 letters, not identical to the current one, filtered for banned words  
- Notice: up to 100 characters  
- **Name and notice can each be changed once per 8 hours**; the icon any time  
- Editable in the game "Guild Management" or the portal "Social → My Planet"  

---

## Tax and contribution

When you claim **taxable IRT income** (milk, Match win chest, PVP report, rental income):

1. Tax is deducted at the planet rate (Home 20%, Frontier 10%, Federation members 20% of the mother Home)  
2. The amount counts toward your **contribution** (member list sorts by it; the guild quest "contribute tax" tracks it)  
3. Tax enters the guild pools: **70% normal tax** (leader can withdraw to their wallet or fund daily benefits), **30% guild battle pool** (the stake in guild battle looting)  
4. Federation members' tax first gives the federation leader a share of "federation rate ÷ 20%", the rest goes to the mother Home  

Check-in, quests, mail, and guild benefits are tax-free.

Guilds have **levels and EXP** (1 – 10; thresholds 1000 / 3000 / 7000 / 15000 / 31000 / 63000 / 127000 / 255000 / 511000) and **guild battle points**; the guild ranking sorts by members / level / points / contribution.

---

## Guild benefits

The leader configures and distributes two kinds (members view and claim under "Guild Benefits"; claims go to the Rewards Center, tax-free).

### Daily benefits

1. As tax accrues, the leader **funds** part of the normal tax into the benefit pool (on-chain)  
2. Sets the **share ratio** per rank (Vice Leader / Elite / Member / Trainee, total 100%)  
3. Clicks **Distribute**. Per-person share = pool × rank ratio ÷ members of that rank  
4. Members claim **before 23:59:59 that day**; it expires after; the leader **must re-distribute every day**  
5. Distribution doesn't deduct the pool; each claim does. Unclaimed amounts stay in the pool  

Participation rules:
- **The leader does not participate** and cannot claim  
- **Members who joined today don't count** today; they participate from the next day  
- Claims match the **current rank**: after a rank change, wait for the next distribution to get the new rank's share  
- With no eligible members, distribution says "no members to distribute to"  

### Loot benefits

From the **guild battle winner's loot**. Four tiers by this period's **contribution ranking** (1 – 5, 6 – 10, 11 – 20, 21 – 50), equal split within a tier; if nobody contributed, split evenly among fighters. Claim before the next guild battle begins.  
See [09 Guild Battle](./09-guild-battle.md).

---

## Joining: direct vs approval

Two switches in "Guild Management → Settings":

| Setting | Effect |
|---|---|
| Require entry fee | Joining deducts an IRT fee (amount set by leader), non-refundable |
| Require join approval | No direct joining; apply first, approved by leader / vice leader |

Approval flow:

1. Choose planet → Join Guild; the button says "Apply"; one pending application at a time (cancel to withdraw)  
2. Leader / vice leader sees it under "Guild Management → Applications", approves or rejects  
3. Once approved, the button becomes "Confirm Join"; confirm in wallet to join. Unconfirmed approvals expire after **24 hours**  
4. "Quick Join" prefers guilds without approval; if all require it, it applies to the first one  

## Kicking members

- The leader can kick anyone but themselves; a vice leader only ranks below their own (Trainee / Member / Elite)  
- Path: Guild Management → Members → settings icon → "Kick"; the operator's wallet sends one transaction  
- A kicked member online gets a prompt and returns to planet selection, free to join another guild; entry fees are not refunded; a pending federation deposit is returned  
- Planet owners and current lessors cannot be kicked  

---

## Federation planet application

Home members can apply to the leader to found a Federation planet (not open to Home leaders during beta):

1. Submit a **bid** (IRT, to the Home leader) and a proposed tax (must be < 20%); a **500 IRT deposit** is locked  
2. Wait for approval; cancel any time before that for a full refund of bid and deposit  
3. On approval: the bid goes to the leader, the **deposit is burned**, a Federation planet is minted to you and you become its leader (population cap 1,000)  
4. The mother Home has a federation slot cap (100); one address may own one planet  

Federation members pay the mother's 20%; the federation leader receives the "federation rate ÷ 20%" share and can run their own daily benefits.

---

## Planet leasing (portal)

A Home leader can lease leadership at **Card Package → planet detail → Rent**:

- Set a monthly rent (IRT) and the tenant's address; the tenant becomes acting leader with leader rights (benefits, guild battle sign-up…)  
- The tenant **pays rent** on the portal; each payment extends 30 days; renewable any time during the lease  
- The lessor can **cancel the lease** after it expires to recover leadership; the card can't be withdrawn while leased  
- A tenant with no planet is bound to this planet automatically; each party can be in only one lease at a time  

---

## Guild shop (Star Shop)

| Tab | Item | Price |
|---|---|---|
| **Regular** | Hay / Prime / Supreme | 100 / 200 / 300 IRG |
| | EXP cards, STR batteries (3 tiers) | 100 / 200 / 300 IRT |
| | HP potions (3 tiers) | 4000 / 8000 / 12000 IRT |
| | Cattle shard | 500 IRT |
| | Rename card | 300 IRT |
| | Breed card (Genesis) | 1000 IRT |
| | Pass / Score Protection / Shuffle / PVE Power card | 200 IRT each |
| **Limited** | Guardian Armor (leader only, guardian defense +20%) | 500 IRT |
| | Packs, skin boxes, badge shreds, power potions… | as listed by ops |

Shelves are maintained by ops; trust the in-game list.

---

## Guild quests

The quest screen has a "Guild" tab: team Arena with guild members, 5v5, pay tax, form a bond, join a guild battle. Full list in [11 Daily Play](./11-daily.md).

---

## Common questions

**Q: Why is my milk claim smaller?**  
A: Planet tax. Home 20%, Frontier 10%; see the breakdown under "Guild Tax".

**Q: Can the leader lower the tax rate?**  
A: No. Rates are fixed by type; for a lower rate choose a Frontier planet (10%).

**Q: I distributed daily benefits but can't see them myself?**  
A: Leaders don't participate in daily benefits; check with another rank's account.

**Q: Members can't see them either?**  
A: In order: was it re-distributed today (benefits are same-day only), did the member join today (eligible from tomorrow), did their current rank have members at distribution time (a rank with 0 members gets no share).

**Q: "Join" fails / the button says "Apply"?**  
A: The guild requires approval. Apply, wait for approval, then "Confirm Join" within 24 hours.

**Q: I'm vice leader; where is "Set Position"?**  
A: Ranks and settings are leader-only; vice leaders approve joins and kick lower ranks.

**Q: I founded a guild with a Frontier planet — why can't I sign up for guild battle?**  
A: Frontier planets can't; the button says "Upgrade to Home to sign up". Upgrade in "Guild Management → Settings → Upgrade to Home", or join a Home planet.

**Q: What does the upgrade cost and what stays?**  
A: About $500 in IRT at the current price (shown in the dialog). Members, tax, benefits, and the battle pool are all kept; only caps and rights become Home's.

**Q: "Set Position" says "you are not the leader"?**  
A: Leadership comes from the on-chain card, synced by the portal. Right after a leader change or a service restart, wait a moment and retry; if it persists, contact support.

Next: [09 Guild Battle](./09-guild-battle.md)
