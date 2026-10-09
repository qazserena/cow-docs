# 09 Guild Battle

Guild Battle (GVG) is a weekly showdown between Home guilds: attack the enemy **guardian**, heal your own, and after 30 minutes the guardian with more HP wins; the winner loots the loser's guild battle pool.

## Schedule (configurable by ops)

One cycle per week in four phases:

| Phase | What happens | Current beta config |
|---|---|---|
| **Sign-up** | Leader signs up in "Guild Events → Guild BOSS Battle" | Tuesday 00:00 – 23:00 |
| **Roster** | After signing up until battle start, the leader picks fighters | Tuesday after sign-up → Wednesday 00:00 |
| **Battle** | Members attack / heal for **30 minutes** | Wednesday 00:00 – 00:30 |
| **Settlement** | Result and points settled immediately | At battle end |

- Only **Home planets** can sign up; Frontier / Federation cannot (Federation members fight with the mother planet)  
- Guilds that didn't sign up sit out; a signed-up guild with no opponent (bye) gets no result and no point change  
- Exact times follow the countdown on the in-game "Guild Events" page  

---

## Matchmaking

- Divisions by guild battle **points ranking**: **TOP** (1 – 10), **MIDDLE** (11 – 50), **ENTRY** (51+)  
- Random pairing within a division; an odd guild out gets a bye  
- Guild battle points use ELO: win up, loss down, draw unchanged; new guilds start at a default score  

---

## The guardian

Each guild has one guardian: **HP 1,000,000, Attack 5000, Defense 5000**.

- The leader can equip **Guardian Armor** (guild shop, 500 IRT) for **+20% defense** this period  
- Guardian reduced to 0 HP → **immediate loss**, the enemy wins on the spot, with a server-wide "lethal blow" marquee  
- If neither falls within 30 minutes → **more remaining HP wins**; equal is a draw  

---

## What you can do in battle

Entry: your guild signed up, you are on the leader's roster, the battle phase is on. Bring a bull or a cow:

| Fighter | Action | Contribution |
|---|---|---|
| **Bull** | Card battle against the enemy guardian; basic-attack damage goes straight to its HP | Damage dealt |
| **Cow** | Heals your guardian on each action: Normal cow **+100**, Genesis cow **+500** | Healing done |

- At most **10 cows** per guild healing at once; more get "team is full"  
- Entering guild battle **costs no combat energy**; re-enter as often as you like  
- Card rules (including Spirit) match the Arena, see [07](./07-arena.md); the guardian has innate crit, and crits trigger a server-wide marquee  
- **Power Potion** (item 20006): for 24 h all your fielded cattle get ATK +4000 / DEF +3000 / STA +5000; stacking extends duration  
- Skin bonuses apply too  

---

## Points and rankings

| Board | Period | Notes |
|---|---|---|
| Guild battle points | Permanent | Guild strength; decides next division |
| Guild battle damage | Weekly | Personal attack contribution, settled Monday 00:00 |
| Guild battle healing | Weekly | Personal healing contribution, settled Monday 00:00 |

Personal contribution (damage + healing) sets your tier for this period's **loot benefits**.

---

## How loot is paid

1. After settlement the winning **leader** claims in the guild events page: both guilds' battle pools for the period (30% of tax) merge into the winner's, wallet confirm  
2. In "Guild Benefits → Loot", the leader decides how much goes to the member pool; **the rest goes to the leader's wallet**  
3. The leader sets four tier ratios (contribution ranks 1 – 5 / 6 – 10 / 11 – 20 / 21 – 50) and distributes  
4. Members claim by their rank tier (tax-free, to the Rewards Center) **before the next guild battle starts**  

"Not victorious / nothing to claim" means this week's result doesn't qualify.

---

## Leader checklist

- [ ] Sign up during Tuesday's window (upgrade a Frontier planet to Home first)  
- [ ] Set the roster before battle; at most 10 cows healing at once  
- [ ] Buy and equip Guardian Armor in advance  
- [ ] After settlement: claim loot, set ratios, distribute  
- [ ] Remind members to claim before expiry  

## Member checklist

- [ ] Confirm you are on the roster  
- [ ] Be online during the battle window to attack / heal (no combat energy cost — go several rounds)  
- [ ] Drink a Power Potion beforehand if needed  
- [ ] Claim loot benefits afterwards (if any)  

Related: guild basics → [08](./08-guild.md); card combat → [07](./07-arena.md)
