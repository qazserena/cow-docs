# 15 FAQ

Look up by symptom. If it's still unresolved, keep a screenshot, the time, and your wallet address (never your private key) and post in the forum's "Bugs & Feedback" category ([bbs.cowgalaxy.com/new?category=3](https://bbs.cowgalaxy.com/new?category=3), visible only to you and admins) or contact community admins on Telegram: [t.me/cowgalaxy](https://t.me/cowgalaxy).

---

## Login & account

**Can't connect the wallet / signature fails?**  
Check the wallet is unlocked, the network is right (beta = Sepolia testnet), and the browser isn't blocking pop-ups. The game client supports injected wallets such as MetaMask and TokenPocket.

**"Logged in elsewhere" / sudden disconnect?**  
One account may be online in one place; a new login kicks the old session.

**Rename says not enough renames?**  
The first rename is free; afterwards use a Rename Card (300 IRT in the shop) from the backpack first.

**My avatar reset?**  
When the avatar NFT leaves your wallet the avatar resets to default; hold it again to switch back.

---

## Cattle & shed

**Why can't my cattle milk / fight?**  
Check: adult, correct gender, in the shed, enough energy, and not in a conflicting state (staking / fighting / listed / feeding / cooldown / dead).

**Can't put cattle in the shed?**  
Bind a planet first; expand at the Academy if slots are full; remove dead cattle occupying slots.

**My Normal cattle died?**  
Lifespan = 35 days × Life ÷ 10000 and it burns when it runs out. Use HP potions (max +10 days per cattle) or star-up to reset lifespan.

**Why are my cattle's stats so much lower than expected?**  
Normal stats = base × star multiplier: 0★ 25%, 1★ 40%, 2★ 60%, 3★ 80%. Star-up is the main upgrade, see [06](./06-academy.md).

**"Daily growth cap reached"?**  
Each calf gains at most 15,000 growth per day from hay / energy (resets 00:00 Beijing); EXP cards are exempt.

**How do I raise farm level / farm EXP?**  
No button. Expansion, breeding, raising a calf to adult, and using batteries / EXP cards / HP potions all add **farm EXP**; filling the tier levels you up automatically. Check in Profile → "Farm EXP". Level 2 needs 200. See [03](./03-cowshed-and-growth.md).

---

## Milk

**Income too low / zero?**  
Confirm the stake succeeded, hasn't expired, and you clicked Claim; income also depends on server hashpower, your stats (incl. star multiplier), farm level, badge, and tax. The daily pool is 200,000 IRT.

**Balance smaller after claiming?**  
Planet tax (Home 20%, Frontier 10%), see [08](./08-guild.md).

**Badge has no effect?**  
Badges work only while at least one cow is staked.

---

## Combat

**Can't enter the Arena — not enough energy?**  
Each match costs 300 combat energy; charge at the "Cattle Energy Station" with bull energy or batteries (cap 20,000). This is not the in-match Spirit.

**No opponents?**  
Match fills with bots after 15 s; Ladders never does and keeps waiting. You may also have used today's valid matches.

**"Not enough Spirit" in a match?**  
Spirit is the card resource — not shed energy, not station energy. You start with **3**, +1 cap and refill each of your turns (max **8**). **No item restores Spirit**; play cheaper cards or end the turn. See [07](./07-arena.md).

**Win chest does nothing / can't claim?**  
Chests settle **yesterday's** wins; today's are claimable tomorrow. Under 10 wins yesterday earns no tier; one claim per mode per day; a locked Rewards Center also blocks it.

**Pass / protection card had no effect?**  
Server daily limits: Pass 2, Score Protection 2, PVE Power 3; extra cards are consumed with no effect.

**Can't join guild battle?**  
You must be on the leader's roster, in the battle phase, and in a Home guild that signed up (Federation members fight with the mother planet).

---

## Guild

**Can the leader change the tax rate?**  
No. Rates are fixed by type: Home 20%, Frontier 10%.

**I distributed daily benefits but can't see them myself?**  
Leaders don't take part in daily benefits — normal.

**Members can't see them either?**  
Check it was "distributed" today, hasn't expired (23:59:59), the member didn't join today, and their rank has a share.

**Can't claim loot benefits?**  
Requires this week's guild battle win and the leader having claimed and distributed; losers see "no reward".

**Rename / notice says time limit?**  
Name and notice can each change once per 8 hours.

---

## Breeding

**Can't breed?**  
Check counts (5 per cattle), cooldown (3 days), energy (1000 each), IRT + IRG balance (from 100 IRT + 100k IRG for the first time), states; rentals also need the stud still listed.

**No Genesis from boxes?**  
The breeding box Genesis rate is **0.01% (1 in 10,000)**; many opens with only calves or shards is normal. Full tables in [16](./16-blind-box.md).

---

## Claims & on-chain

**Check-in / mail / benefits say "locked"?**  
The Rewards Center has an unfinished on-chain claim order. Finish the wallet confirmation there; it unlocks on arrival. If the tx already succeeded, reopening the Rewards Center reconciles and unlocks.

**Claimed in the Rewards Center but nothing in the wallet?**  
Many rewards need a second on-chain confirmation; check the tx status, network, and pending state.

**Gas failed / stuck?**  
Raise gas or wait for congestion to ease; don't resubmit with different parameters.

**Is approving dangerous?**  
Approve official contracts only; review and revoke unknown approvals in a block explorer periodically.

---

## Marketplace & transfers

**Why do some cattle have "Sell" and others don't?**  
**Normal adults cannot be listed** (on-chain rule). Only **Normal calves** and **Genesis** can be sold.

**Normal cattle transfer failed?**  
Normal cattle (adult or not) cannot be transferred wallet-to-wallet on-chain; marketplace only. Genesis transfers freely. See [13](./13-market.md).

**Listing failed?**  
Not approved, Normal adult, calf USDT price below 150, cattle still in the shed (remove to wallet first), not enough gas, wrong network.

---

## Beta

**Can't claim the starter pack?**  
Once per address; "enter the game first / finish a quest" are daily-supply conditions; "out of stock" waits for ops restock. See [17](./17-beta.md).

**Bound an invite code but no points?**  
Filtered invites (same network as the inviter, or more than 3 from one network in 30 days) earn nothing for either side; the inviter gets +50 / +100 only when the friend actually enters the game and finishes a quest.

---

## Want the full picture?

Read module by module from the [README](./README.md); box odds in [16](./16-blind-box.md); cards in [Appendix · Cards](./appendix/cards.md); terms in [Appendix · Glossary](./appendix/terminology.md).
