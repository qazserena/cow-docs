# 07 Arena

The Arena is the combat hub for **adult bulls**: turn-based card battles across PVE, Match, and Ladders, earning **IRG / IRT**, points, and chest rewards.

## Before you fight

1. An adult **bull** in the shed, in a usable state  
2. Enough **combat energy** (charge at the energy station with vitality or vitality packs; energy pool has a cap)  
3. Daily entries for that mode not used up  
4. Optional: wear skins; bring Clear Tickets / Power Cards / Point Protection Cards, etc.  

---

## Three modes

### 1) PVE (campaign)

- Challenge bosses / climb stages  
- Use **Clear Tickets** to sweep (daily limits apply)  
- Mainly produces game coin and win progress  

### 2) Match (PVP)

- Supports 1v1, 3v3, 5v5  
- Invite friends or guild chat to party up  
- Match timeout may fill with bots  

### 3) Ladders

- Usually 5v5  
- ELO-style rating, weekly boards and rewards  
- Use **Point Protection Cards** to avoid losses (per item text)  

---

## How combat works (rules overview)

- **Turn-based cards**: dice or similar decide first move  
- Cards split into combat / defense / magic types (many idiom-named cards)  
- **Spirit (mana)**: in-match resource for playing cards — see the next section; do not confuse it with pre-match **combat energy** or CowShed **vitality**  
- Hand size is capped; at most **2** cards per turn, and they cannot share the same type  
- Buffs include crit, lifesteal, reflect, invuln, seal, stun, and more  
- Supports surrender votes and reconnect; if everyone is disconnected for too long, the match may end  

For card details, open the in-arena **card codex**.

---

## Spirit (in-match mana)

Every card has a cost. If your remaining spirit is below that cost, you see **“Not enough spirit”** and the card will not play. That is the rule, not a bug.

| Rule | Detail |
|---|---|
| Start | **3 / 3** |
| Start of your turn | Cap **+1**, then **refill** to the new cap |
| Cap | Max **8** |
| Spend | Playing a card deducts its cost (typically 1–6) |
| Recover | **No potions and no energy station refill spirit.** Wait for your next turn |
| No carry-over | Unused points this turn do not stack; next turn still fills to the current cap |

How it differs from other resources:

- **Vitality**: CowShed feeding — used for growth / milk / charging the energy station  
- **Combat energy**: charged at the energy station **before** a match; without it you cannot enter the Arena  
- **Spirit**: used **inside** a match to play cards  

Tips: with only 3–4 spirit in the first turns, play 1–2 cost cards; save 4-cost and 6-cost cards until the cap grows. If you already played one card this turn and cannot afford the next, switch to a cheaper card or end the turn.

---

## How a PK match plays out (server rules)

Every Arena mode shares one turn-based engine. Flow: match → enter → guess first → play cards / attack → resolve.

### 1. Before the fight

- An adult **bull** with valid on-chain combat stats (ATK / STA / DEF), not dead  
- Enough **combat energy**: current entry cost is **300** per mode (template can change)  
- Cattle selected; party modes also need a full roster  

Not enough energy blocks entry (separate from in-match spirit). PVE Power Cards and equipped skins apply as you enter.

### 2. How you get an opponent

| Mode | Size | Pairing |
|---|---|---|
| **PVE campaign** | You vs the stage monster | No human match. You always go first |
| **Match 1v1** | 2 players | Another 1v1 team that already tapped Start. **Normal cattle only fight adjacent star grades** (0★ vs 0–1, 1★ vs 0–2, 2★ vs 1–3, 3★ vs 2–3). **Genesis only fights Genesis** |
| **Match 3v3 / 5v5** | 6 / 10 | Both sides must be full. Positions shuffle on enter |
| **Ladders** | Up to 5 per side, fill 5v5 | Ready parties are packed into red/blue by size (largest first) until each side has 5 |

If Match finds no valid opponent for **15 seconds**:

- **1v1**: fight a bot (each of your three stats minus about 200–500; counted as Match 1v1)  
- **3v3 / 5v5**: fill the other side with bots; Normal bots ~5000±2000, Genesis ~10000±2000  

Ladders do **not** fill with bots — they keep waiting.

Party: leader creates, picks cattle, invites / guild-chat join, then Start. Leader leaving dismisses the party; a kick or leave cancels matching.

### 3. Positions

| Mode | Layout |
|---|---|
| PVE, 1v1 (including bots) | One cattle each, back-middle |
| 3v3, Ladders | Back row top / mid / bottom |
| 5v5 | 2 front + 3 back |

A side wins when the other side has no living cattle (section 6).

### 4. Guess, deal, turns

1. After load + ready, **guess first**: Match / Ladders roll red vs blue (higher goes first). PVE: you always first.  
2. Each player shuffles a full deck and is dealt **3** cards.  
3. The first side acts on turn 1. Spirit rules: previous section.  
4. **When a cattle acts**: extra cards (usually 2), hand cap **6**; empty pile reshuffles the full set.  
5. Play timeout ~**20 s**, action timeout ~**8 s**; server auto-skips.  
6. After chosen cards resolve, the cattle makes **one basic attack** (cows heal the Guardian in guild battle; Arena uses bulls, so this is an attack).  
7. After every living ally has acted, the other side’s turn starts.

Illegal plays are rejected:

- Cost above current spirit  
- More than **2** cards in one turn  
- Two cards of the **same type** in one turn  
- Sealed types  

Bots wait ~2.5–7 s then randomly play 0–2 cards.

### 5. Damage

Basic attack (floored):

**damage = ((0.5 × ATK)² / (ATK + DEF) × 0.8)**

ATK/DEF include this turn’s cards and buffs. Common modifiers:

- **Ignore DEF** ≈ ATK / 2  
- **Crit** from card rate, then crit-ratio extra  
- **Damage amp / splash / lifesteal / reflect** from buffs  
- **Invulnerable** blocks HP loss  

Also:

- **Death Contract**: small chance (~10%) at turn start if HP is very low  
- **Lucy / overdrive**: after **10** spirit spent this match, small one-time chance (~10%) to greatly raise DEF  

Card text in the codex wins for specifics.

### 6. Win, surrender, disconnect

After each cattle acts:

- Enemy all down → you win  
- You all down → you lose  
- Both sides empty → **draw**  
- Surrender vote passes → you lose, they win  

1v1: your surrender succeeds immediately. Larger modes need enough yes votes on your team; too many nos fail the vote.

Disconnect:

- **Everyone** gone ~**60 s** → match force-ends  
- **Some** gone ~**30 s** → server forces the next step  
- PVE / vs-bot disconnect counts as surrender  
- Match / Ladders can reconnect and resync board + hand  

### 7. Ladder rating

ELO vs the enemy **average** rating. Win scores 1.15, loss 0. K is 40 below 1800, 36.67 through 2400, 20 above.  

**Draws**, or **20** valid Ladder games already today → rating unchanged.  
**Point Protection Card** plus a loss → stay at pre-match rating. Floor is 0.

### 8. Win chests

Daily wins snap to tiers: under 10 → 0, 10–14 → 10, 15–19 → 15, 20+ → 20, then × ranch cattle-rate.  

Match 3v3 / 5v5 can get a party multiplier (~1.1, or ~1.2 if those wins are all 5v5). Playing with an **intimate friend** adds more — see [10](./10-social.md).  

PVE Clear Tickets: up to **2**/day. PVE Power Cards: **2**/day. Point Protection: **1**/day.

---

## Rewards and daily limits

- Each mode has a daily match cap (e.g. separate PVP / PVE / Ladder counts; adjustable)  
- **Win chests**: claim at daily win tiers such as 10 / 15 / 20; higher tiers have reward multipliers  
- Qualifying PVP battle reports can be **claimed on-chain** (wallet confirm; may involve a Banker signature flow)  
- Claiming IRT-type rewards may also trigger planet tax  

Party bonus examples (trust in-game):

- High-winrate five-stacks may get extra multipliers  
- Intimate friends in a party may get reward bonuses (see [10](./10-social.md))  

---

## Helper items at a glance

| Item | Effect |
|---|---|
| Clear Ticket | PVE +1 win progress / sweep related; daily limits |
| Point Protection Card | Ladder losses don’t drop rating |
| PVE Power Card | Temporary 3-stat boost |
| Shuffle Card, etc. | Per item text |

Guild shops often sell some combat items.

---

## Leaderboards

- Ladder **weekly board** (periodic settlement and rewards)  
- Related ranks under Arena “Points Ranking,” etc.  

Guild battle boards: [09](./09-guild-battle.md).

---

## Newbie combat tips

1. Start with PVE to learn cards and pacing; early turns have little spirit, so play cheap cards first  
2. Keep combat energy topped at the energy station — avoid “cattle but no energy” (that is not in-match spirit)  
3. Clear win-chest tiers every day  
4. Push Ladders once you have a stable lineup  

Guild-side combat → [09 Guild Battle](./09-guild-battle.md)
