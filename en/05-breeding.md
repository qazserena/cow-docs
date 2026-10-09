# 05 Breeding Institute

The Breeding Institute handles **breeding**: pair a bull and a cow to get an **embryo box (cattle box)**; open it for a new cattle or shards.

## Breeding your own

### Requirements

- An **adult bull** + an **adult cow**, both in the shed  
- Both have **breed count** left (5 per cattle; Genesis can add more with breed cards)  
- Neither is in **breeding cooldown** (3 days after breeding; tech can cut it to 2)  
- Both have **1000 energy** (deducted at breeding)  
- Pay the breeding fee (IRT + IRG, both burned)  

### Fees (current config)

Each cattle's tier is its **own breeding count**; the two are averaged:

| Breeding no. | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| IRT | 100 | 200 | 300 | 400 | 500 |
| IRG | 100k | 200k | 300k | 400k | 500k |

Breeding tech "Thrifty" at max level gives **50% off** (see [06](./06-academy.md)). Each breeding grants +20 farm EXP.

### Flow

1. Open **Breeding Institute → Select Breeding**  
2. Pick the bull and cow, confirm the fee, confirm in wallet  
3. You receive 1 box; both cattle enter cooldown and lose one breed count  
4. Open it under the "Cattle Box" tab  

### How offspring are rolled

- Life, Energy cap, Growth: parents' average × 0.9 – 1.1  
- Bull calf's Attack / Stamina / Defense = father's × 0.9 – 1.1; cow calf's milk stats = mother's Milk × 0.9 – 1.1  
- 50/50 gender; better parents → better calves  

---

## Rental market (rent a stud)

For when you lack a pair, or want to rent out an idle stud.

### List for rent

1. Pick the cattle (adult, in shed, energy ≥ 1000, breed count left, not in cooldown)  
2. Set the stud fee (IRT)  
3. List it; cancel any time  

### Rent someone else's

1. Filter by bloodline / gender / count / price  
2. Pay: **stud fee (to the owner) + your own cattle's tier fee (burned)**; only your cattle loses 1000 energy  
3. The box is yours; the owner's cattle also loses a breed count and enters cooldown; the listing is removed  

The stud fee is taxed at **your planet rate** into the guild tax pool (and counts toward your contribution); the owner receives fee − tax. There is no extra platform fee.

---

## Opening boxes

Open breeding boxes at the Breeding Institute:

- **Normal calf 90%** (stats follow parents when recorded)  
- **Cattle shards 9.99%** (4 or 5 per open)  
- **Genesis 0.01%** (1 in 10,000)  

**10** shards craft a Normal cattle at the Academy. Full drop tables for IGO, CattleMart, and skin boxes: **[16](./16-blind-box.md)**.

---

## Referral rewards (on-chain, automatic)

After binding a referrer (who must hold at least one cattle; one-time, permanent):

- Every **5** successful breedings by you earn the referrer **1 embryo box + 1 breed card**, with a system mail  
- The referrer benefits **passively**; your fees are unchanged  

This on-chain referral is separate from the portal's **beta invite points** — see [17](./17-beta.md).

---

## Tips

- Breed with high-stat parents for better calves; Genesis parents give higher base stats  
- Fees rise with count, the 5th is the most expensive; watch cooldowns so key cattle aren't locked out  
- Listing for rent does not lock the cattle: it can still feed, milk, and fight; count and cooldown apply only when actually rented  

Related: star-up & shard crafting → [06](./06-academy.md); odds → [16](./16-blind-box.md)
