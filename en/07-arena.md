# 07 Arena

The Arena is the combat hub for **adult bulls**: turn-based card battles across PVE, Match (PVP), and Ladders, earning **IRG / IRT**, rating points, and chests.

## Before you fight

1. An adult **bull** in the shed, alive  
2. Enough **combat energy**: **300** per match, charged at the "Cattle Energy Station" with bull energy or STR batteries; pool cap 20,000 (see [03](./03-cowshed-and-growth.md))  
3. Valid matches left today (each mode counts **20** per day for rewards)  
4. Optional: wear a skin (adds attack / defense / stamina), bring pass / power / score-protection cards  

Skin stats, PVE power card, and combat tech are applied on entry. A Normal bull's stats already include the star multiplier (0★ = 25%), see [02](./02-tokens-and-assets.md).

---

## Three modes

### 1) PVE (BOSS floors)

- **20 floors**, cleared in order; you alone vs a floor monster, you always go first  
- Monsters scale with floor: floor 1 ATK 1000 / DEF 100 / HP 1500 → floor 10 ATK 2300 / DEF 640 / HP 3750 → floor 20 ATK 13000 / DEF 8000 / HP 14000  
- Wins count toward PVE daily wins; **Pass cards** add +1 win directly (2 per day)  
- Reward: next day's PVE **win chest (IRG)**  

### 2) Match (PVP)

- 1v1, 3v3, 5v5; invite friends or your guild channel  
- No opponent within 15 s → bots fill in  
- Reward: next day's Match **win chest (IRT)**; 10 wins today lets you submit an on-chain **PVP battle report**  

### 3) Ladders

- 5v5, ELO rating, starts at **1000**; you appear on the board at **≥ 1100**  
- Weekly board settles **Monday 00:00**: ranks 1 – 3 get a **UR chest**, 4 – 10 **SSR**, 11 – 50 **SR** (contents in [16](./16-blind-box.md)); the board resets, personal rating is kept  
- **Score Protection cards** prevent losing points  

---

## How battles work (overview)

- **Turn-based cards**: dice decide who goes first  
- Three card types — Combat / Defense / Magic — 21 cards, cost 1 – 6 (full effects in [Appendix · Card Compendium](./appendix/cards.md))  
- **Spirit (blue bar)**: the in-match card resource, next section; do not confuse with pre-match **combat energy** or shed **cattle energy**  
- Hand cap 6; at most **2** cards per turn, never two of the same type  
- Buffs include crit, lifesteal, reflect, invincibility, seal, stun, bleed, poison…  
- Surrender votes and reconnection are supported; a match ends if everyone disconnects too long  

The in-Arena **Card Compendium** has every card.

---

## Spirit (the blue bar)

Every card has a cost. If your Spirit is below it you get **"Not enough Spirit"** and the card won't play. That is the rule, not a bug.

| Rule | Detail |
|---|---|
| Start | **3 / 3** |
| Start of your turn | cap **+1**, then **refill** to the new cap |
| Cap | **8** |
| Spent | per card cost (1 – 6) |
| Restored | **No potion or station refills Spirit.** Only your next turn |
| No banking | Unspent points don't carry; next turn you still refill to cap |

The three resources:

- **Cattle energy**: fed in the shed; for raising / milk / charging the station  
- **Combat energy**: prepared at the station, 300 per match, no entry without it  
- **Spirit**: used in the match to play cards  

Tip: with 3 – 4 Spirit early, play 1 – 2 cost cards; save 4- and 6-cost cards for later turns.

---

## A full PK, step by step (server rules)

All modes share one engine. Below: matchmaking → placement → coin toss → cards and attacks → result.

### 1. Finding an opponent

| Mode | Players | Rule |
|---|---|---|
| **PVE** | you vs a floor monster | Monster from the floor table, no humans; you go first |
| **Match 1v1** | 2 | Another 1v1 team that pressed Start. **Only adjacent star tiers for Normal cattle** (0★ vs 0 – 1, 1★ vs 0 – 2, 2★ vs 1 – 3, 3★ vs 2 – 3); **Genesis only fights Genesis** |
| **Match 3v3 / 5v5** | 6 / 10 | Both sides must be full; positions are shuffled on entry |
| **Ladders** | up to 5 per side, filled to 5v5 | Ready squads are packed into red / blue by size, largest first, until both sides have 5 |

If no opponent after **15 s** in Match:

- **1v1**: a bot (your bull's three stats minus 200 – 500 each; still counts as a solo match)  
- **3v3 / 5v5**: bots fill the other side; Normal bots ≈ 5000±2000 per stat, Genesis ≈ 10000±2000  

Ladders never add bots — it keeps waiting.

Teams: the captain creates the team, picks cattle, invites via friends or guild channel, starts when full. Captain leaving disbands the team; kicked or leaving players cancel matchmaking.

### 2. Placement

| Mode | Positions |
|---|---|
| PVE, 1v1 (incl. bots) | 1 each, back-center |
| 3v3, Ladders | back row top / middle / bottom |
| 5v5 | 2 front + 3 back |

### 3. Toss, deal, turns

1. After both load and ready, **toss**: Match / Ladders roll random numbers, higher goes first; PVE you go first  
2. Each player shuffles a full deck and draws **3**  
3. **When a cattle acts**: draw (usually 2), hand cap **6**; an empty deck reshuffles all cards  
4. ~**20 s** to play, ~**8 s** for animations; timeouts are skipped by the server  
5. After its cards resolve the cattle makes **one basic attack**  
6. When all living cattle on a side have acted, the other side's turn begins  

Illegal plays are rejected: cost above current Spirit; more than 2 cards; two of the same type; a sealed type. Bots play 0 – 2 random cards after 2.5 – 7 s.

**Redraw your hand (Shuffle Card)**: if your hand is bad, tap "Shuffle ×N" at the bottom right during your own pick phase, before placing any card. Your whole hand is replaced by the same number of new cards (old cards go back into the deck, deck size unchanged); Spirit and the timer are untouched. Once per pick phase, 1 shuffle per use. N is how many shuffles you have banked — "use" Shuffle Cards in the backpack first (up to 5 activations per day); with none banked the button tells you to go to the backpack.

### 4. Damage

Basic attack (rounded down):

**Damage = (0.5 × ATK)² ÷ (ATK + DEF) × 0.8**

ATK / DEF include this turn's cards and buffs. Common modifiers:

- **Ignore defense** (X-Ray): about ATK ÷ 2  
- **Crit**: by the card's crit rate, then crit multiplier  
- **Damage bonus / splash / lifesteal / reflect / shield / invincible**: by buff  
- **Death Contract**: at the start of your turn with very low HP, ~10% to trigger  
- **Lucy Mode**: after 10 cumulative Spirit spent this match, ~10% to trigger once, big defense boost  

### 5. Win, surrender, disconnect

Checked after every action: enemy all down → win; your side all down → loss; both at once → **draw**; surrender vote passes → loss.

Surrender: in 1v1 your own click is enough; larger modes need enough team votes.

Disconnects: **everyone** gone ~60 s → match force-ends; **some** gone ~30 s → server auto-advances turns; PVE / bot matches treat disconnect as surrender; Match / Ladders support reconnect.

### 6. Ladders rating

ELO against the enemy's average rating. Win = 1.15, loss = 0. K: 40 below 1800, 36.67 for 1800 – 2400, 20 above.  
**Draw**, or 20 valid matches already today → rating unchanged. A **Score Protection card** keeps the pre-match rating when you would drop. Floor 0.

---

## From wins to rewards

### Valid wins and multipliers

- Daily wins are tiered: **10 – 14 counts as 10, 15 – 19 as 15, 20+ as 20**; under 10 counts nothing  
- × the farm level **combat multiplier** (1.00 – 1.40, see [03](./03-cowshed-and-growth.md))  
- Match team bonus: ≥ 80% of today's valid wins from 3v3 / 5v5 → **×1.1**; if all of those are 5v5 → **×1.2**  
- Wins with a **bonded friend** on your team add **20%** pro rata (see [10](./10-social.md))  

### Win chests (in game, next day)

The Arena "Win Chest" settles **yesterday's** data, one per tab (Match and PVE):

> Your chest = day pool × (your weighted wins ÷ server-wide weighted wins)

- Match chest pays **IRT**, PVE chest pays **IRG** (pool sizes set by ops)  
- Goes to the **Rewards Center** (the Match chest is taxable); cannot claim while the Rewards Center has a pending order  

### PVP battle report (on-chain pool)

After **10 Match wins** today you can submit a battle report in the Arena (wallet confirm, server-signed):

- The contract has a **10,000 IRT** daily report pool, split by "your weighted wins ÷ all weighted wins submitted that day"  
- Submit today, claim that day's share **from the next day**; planet tax applies on claim  
- Max 20 wins per day per player; repeated submissions only add the increment  

### Daily card limits

| Item | Per day | Effect |
|---|---|---|
| Pass Card | 2 | PVE win +1 |
| PVE Power Card | 2 | +10% to all three stats in PVE (no stacking) |
| Score Protection | 1 | Keep rating when the next Ladders match would drop it |
| Shuffle Card | 5 activations | Each banks 1 in-battle shuffle: replace your whole hand in a pick phase (once per phase) |

At the limit the game says "max N per day" and the card is not consumed. Buy them in the **guild shop** (200 IRT each).

---

## Leaderboards

- Arena "Ranking": Ladders weekly board (≥ 1100 to appear), settled Monday 00:00 with chests  
- Portal `/social/leaderboards`: this week / last week / all-time  

Guild battle boards: [09](./09-guild-battle.md).

---

## Tips for new fighters

1. Start with PVE to learn cards and tempo; play cheap cards early  
2. Keep the energy station full — "has bull, no energy" is the classic mistake (not the same as Spirit)  
3. Hit the 10 / 15 / 20 tiers daily and claim both chests the next day  
4. 0-star Normal bulls are very weak; star up before pushing Ladders  

Guild combat → [09 Guild Battle](./09-guild-battle.md)
