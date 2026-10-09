# 04 Milk Factory · Milk Mining

The Milk Factory is where **cows** earn **IRT**: stake adult cows and share the server-wide milk pool by hashpower.

## Requirements

- An **adult cow** in the shed, not feeding / in breeding cooldown / otherwise busy  
- The cow has **energy**: the energy you commit at staking sets the milking duration (1 energy = 60 s)  

---

## How to play

1. Open the **Milk Factory**  
2. Pick an adult cow, enter the energy to commit, **Stake**  
3. Output accrues per second; **Claim** any time  
4. **Renew** before expiry (commit more energy); after expiry it stops — **Redeem** → feed in the shed → stake again  

- Duration never exceeds the cow's remaining lifespan  
- A staking cow cannot breed, leave the shed, or be listed  
- Milk tech "Scientific Production" lowers the energy consumed (up to −20%)  

---

## How income is calculated

> Your income = daily server pool × (your hashpower ÷ total staked hashpower)

- **Daily server pool**: currently **200,000 IRT / day** (contract setting, released per second)  
- **One cow's hashpower** = (Milk × Lactation Booster + Milk Rate × Milking Kit) ÷ 2 × **farm level multiplier** (1.00 – 1.30)  
- A Normal cow's milk stats already include the star multiplier (a 0-star cow has only 25% of base), so **star-up matters a lot for milk**  
- The more total hashpower on the server, the smaller each cow's share  

Exact numbers follow the in-game panel.

---

## Badge bonus

Equip **one badge** at the Milk Factory for extra hashpower:

| Badge | Bronze | Silver | Gold | Platinum | Diamond | Master |
|---|---|---|---|---|---|---|
| Hashpower | +1000 | +2000 | +6000 | +30000 | +40000 | +60000 |

- The badge only works while **at least one cow is staked**; its duration follows the latest-expiring staked cow  
- Removing the badge settles the income it produced  
- Badge sources and crafting: [12](./12-backpack.md)  

---

## Tax

Milk claims are taxed at your planet rate (Home 20%, Frontier 10%, Federation members at the mother Home's 20%):

- The tax counts toward your guild **contribution** (the guild quest "contribute tax" tracks it)  
- Tax flows into the guild pools: 70% normal tax (leader withdraws or funds daily benefits), 30% guild battle pool  

See [08 Planets & Guilds](./08-guild.md).

---

## FAQ

**Q: Why is my income so low?**  
A: Heavy server staking, low own hashpower (0-star Normal cows especially), low farm level, no badge, or short claim intervals.

**Q: Can a staking cow breed?**  
A: No — redeem first.

**Q: What if energy runs out?**  
A: Milking stops at expiry. Redeem, feed, re-stake — or renew before expiry.

**Q: Genesis vs Normal cows?**  
A: Genesis stats apply at 100% with higher base, so hashpower is usually several times a 0-star Normal cow's; eternal life means no death before expiry.

Next: [05 Breeding Institute](./05-breeding.md) or [07 Arena](./07-arena.md)
