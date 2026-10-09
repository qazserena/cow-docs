# 11 Daily Play

Everything you can claim or do each day: check-in, quests, mail, Rewards Center, leaderboards.

All "daily" resets happen at **00:00 Beijing time**; "weekly" at **Monday 00:00**.

## Check-in

- Once per day; the reward is fixed (set by ops — IRG / items) and goes to the **Rewards Center** (tax-free)  
- If the Rewards Center has a pending claim order, check-in says "locked"; finish that wallet transaction first  

Entry: sidebar "Check-in".

---

## Quests

Two tabs — "Personal" and "Guild" — grouped as daily / weekly / achievements. Claim on completion; rewards go to the Rewards Center (tax-free). Format: IRG + items.

### Daily (personal)

| Quest | Reward |
|---|---|
| Milk Factory: 2 / 4 / 6 / 8 cows actively staked today | 1000 IRG + Supreme Hay ×10 / 3000 IRG + Supreme Hay ×20 / Prime Battery ×1 / Supreme Battery ×1 |
| PVP matches 10 / 15 / 20 | 1000 IRG + Supreme Hay ×10 / 2000 IRG + Supreme Hay ×10 / 1000 IRG + Supreme Battery ×1 |
| PVE matches 10 / 15 / 20 | 100 IRG / 200 IRG / 500 IRG + Prime Battery ×1 |

### Daily (guild)

| Quest | Reward |
|---|---|
| 5 Arena team matches with guild members | 1000 IRG + Supreme Hay ×10 |
| 2 PVE sweeps (Pass cards) | 1000 IRG + Supreme Hay ×10 |
| 3 5v5 matches with guild members | 2000 IRG + Battery ×1 |

### Weekly (guild)

| Quest | Reward |
|---|---|
| Contribute 100 / 200 / 300 / 400 IRT of tax to the guild | 500 IRG + Battery / 1000 IRG + Battery / 1500 IRG + Prime Battery / 2000 IRG + Supreme Battery |
| Form a bond with a guild member | 1000 IRG + Supreme Battery |
| Take part in one guild battle | 1000 IRG + Supreme Battery |

### Achievements (one-time)

| Quest | Reward |
|---|---|
| Expand the shed once / craft a cattle once / breed once | 5000 IRG each |
| List one rental | 1000 IRG |
| Raise one calf to adult | 1000 IRG |
| Ranch level 2 / 3 / 4 / 5 / 6 | 2000 IRG + Supreme EXP Card / 5000 IRG + Supreme Battery / 5000 IRG + Supreme Battery + Supreme EXP Card / 10000 IRG + same / 20000 IRG + Supreme Battery ×2 + Supreme EXP Card ×2 |
| Star up a Normal cattle to 1 / 2 / 3 | 5000 IRG / 10000 IRG / **1 cattle box** |
| Max each of the 9 tech nodes | 10000 IRG each |

Guild-battle quests appear only for Home planet members.

---

## Mail

- System mail (server-wide / targeted by ops), group mail (auto-delivered by join-date rules), referral reward mail, etc.  
- May carry attachments: tokens, items, NFTs, boxes; **Claim All** supported, attachments go to the Rewards Center (tax-free)  
- Mark read / delete; some mail expires (referral mail after 10 days) — claim in time  

---

## Rewards Center

Collects rewards from everywhere into two pools: **tax-free** (check-in, quests, mail, guild benefits, Ladders chests) and **taxable** (Match win chest…).

### Claim flow

1. Click "Claim" → the server creates an **on-chain claim order** (server-signed)  
2. Confirm in wallet; assets arrive; the taxable pool is taxed at your planet rate  
3. Until the order completes, **the Rewards Center is locked**: check-in, mail, benefits, and chests all say "locked"  
4. It unlocks automatically after the transaction; if the tx succeeded but it still shows locked, reopening the Rewards Center reconciles it  

### Notes

- Under congestion, wait instead of spamming (duplicate gas)  
- On testnet, top up test ETH first if gas runs out  

---

## Leaderboards

| Board | Period | Notes |
|---|---|---|
| Arena Ladders | Weekly | ≥ 1100 to appear; settled Monday 00:00; top 50 get UR / SSR / SR chests |
| Guild battle points | Permanent | Guild strength; sets guild battle divisions |
| Guild battle damage | Weekly | Personal attack contribution |
| Guild battle healing | Weekly | Personal healing contribution |

In game: Arena "Ranking" and the guild events page; portal `/social/leaderboards` shows this week / last week / all-time and your rank when connected.

---

## Suggested daily list

1. Check in  
2. Clear quests (personal + guild): stake cows, hit PVP / PVE tiers, sweep with 2 Pass cards  
3. Milk Factory: claim, renew  
4. Arena: claim yesterday's two win chests; submit a PVP report at 10 wins  
5. Claim everything in the Rewards Center and confirm on-chain  
6. Check guild benefits and guild battle status  
7. During beta: claim the portal daily supply (every 24 h)  

Related: guild benefits → [08](./08-guild.md); combat → [07](./07-arena.md); beta → [17](./17-beta.md)
