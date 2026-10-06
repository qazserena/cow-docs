# 04 Milk Factory · Milk Mining

The Milk Factory is where **cows** earn **IRT**: stake adult cows and share the server-wide milk pool by hashrate.

## Prerequisites

* You have an **adult cow**
* The cow has enough **vitality** (determines how long she can stay staked)
* The cow is in a usable state (not in combat, listed, or other conflicting states)

***

## How to play

1. Open the **Milk Factory** building on the main map
2. Select an adult cow and **stake**
3. Wait for output to accumulate and **claim rewards** anytime
4. When vitality runs out or the stake ends, production stops — **redeem** → feed in the CowShed → stake again

While staked, the cow usually cannot breed, list, or do other conflicting actions.

***

## How rewards are calculated (mechanics)

Rough formula:

> Your reward ≈ daily milk pool × (your hashrate ÷ server total staked hashrate) × ranch-level bonus

* **Hashrate** comes mainly from the cow’s milk yield, milk rate, and similar stats
* The larger the **server total hashrate**, the smaller each cow’s share (competition)
* **Ranch level** adds a reward multiplier (see [03](03-cowshed-and-growth.md))
* Daily pool size is contract-configured (historically “release a set amount of IRT per day”; adjustable)

Exact numbers are on the in-game panel.

***

## Badge bonuses

The Milk Factory can equip a **badge** (usually only **one** at a time) for extra hashrate:

| Badge tier | Approx. hashrate bonus |
| ---------- | ---------------------- |
| Bronze     | +1000                  |
| Silver     | +2000                  |
| Gold       | +6000                  |
| Platinum   | +30000                 |
| Diamond    | +40000                 |
| Glory      | +60000                 |

Note: badges usually only apply after you have **at least 1 cow staked**.\
How to get and craft badges: [12 Backpack · Items · Skins · Badges](../social-and-daily/12-backpack.md).

***

## Tax

When you claim milk rewards (IRT), tax is auto-deducted at your bound planet’s **tax rate**:

* Tax amount counts as guild **contribution**
* Default rate is often about 20%; Home planet leaders can adjust within a band

Details: [08 Planets & Guilds](../combat-and-guilds/08-guild.md).

***

## FAQ

**Q: Why are my rewards so small?**\
A: High server stake, low personal hashrate, low ranch level, no badge, or claiming over a very short window all make rewards look small.

**Q: Can a staked cow breed?**\
A: Usually you must redeem first. Follow in-game prompts.

**Q: What happens when vitality hits zero?**\
A: Production stops. Redeem, feed, then stake again.

**Q: Do Genesis cows differ from Normal cows?**\
A: Higher stats usually mean stronger hashrate; Genesis also has the lifespan advantage. The mechanism is the same.

Next: [05 Breeding Institute](05-breeding.md) or [07 Arena](../combat-and-guilds/07-arena.md)
