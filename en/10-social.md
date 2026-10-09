# 10 Friends & Social

## Friends

Entry: sidebar "Friends" → Friend Management (Friend List / Add Friend / Requests).

1. Search a player by nickname and send a request (they get a prompt)  
2. They accept under "Requests" and you become friends; rejections are notified too  
3. Friend cards offer: chat, invite to team, view profile, form a bond, delete  

The list shows last online time, planet, and intimacy. The portal "Social → My Friends" shows the same list (add / accept happens in game).

---

## Chat channels

| Channel | Use |
|---|---|
| **Guild chat** | Planet members: coordination, teaming, guild-battle calls; Federation members share the mother planet's channel |
| **Federation channel** | Inside a Federation planet |
| **Private chat** | One-on-one with friends, with history |

- Max **120** characters per message  
- Rate limit: 5 in a burst, then 1 per second; too fast returns "duplicate request"  
- Banned words are replaced with `*`, the message still goes through  
- Team invites appear as messages / pop-ups; accept to join the team  

---

## Bonds (on-chain relationships)

Four kinds (no gender restriction): **Best Friend, Lover, Confidante, Bro**.

### Reaching bondable

1. **Team up** with a friend in 3v3 Match, 5v5 Match, or 5v5 Ladders; each match adds **+10** intimacy between teammates who are friends, win or lose  
2. At **200** intimacy (the cap) you can propose a bond under "Friend Management → Bond"  
3. Both accept → **on-chain bond** (wallet confirm, server-signed; one relationship per pair of addresses)  

> Only multi-player team battles raise intimacy: PVE, solo Match, chat, and sharing a guild do not. 0 → 200 takes 20 matches together.

### Benefits

- Match wins with a bonded friend on your team add **+20%** to weighted wins (affects win chests and report shares, see [07](./07-arena.md))  
- Guild achievement "form a bond with a guild member" pays 1000 IRG + Supreme Battery  
- Shown in the profile  

### Unbonding

Either party can dissolve the bond on-chain (wallet confirm); intimacy must be rebuilt before bonding again.

---

## Profile

Tap your avatar:

| Item | Notes |
|---|---|
| Nickname | **First rename is free**; afterwards use a **Rename Card** (300 IRT) from the backpack first; no punctuation, no duplicate of the current name, word filter |
| Avatar / frame | Switch to an **avatar NFT** you hold (issued automatically at birth / adulthood); transferring the NFT away resets the avatar |
| Motto | Click to edit, publicly shown |
| Farm EXP | Current level and progress, see [03](./03-cowshed-and-growth.md) |
| Cattle stats | Bulls / cows / Genesis / bred / dead |
| Income stats | Cumulative IRT / IRG income |
| Planet, bonds | Click to jump |

---

## Teaming tips

- Invite from the friend list or guild channel for 3v3 / 5v5; the team disbands if the captain leaves  
- Guild quests often require "team with guild members" — team with guild friends first  
- When bonded friends boost income, queue together  

Quests: [11](./11-daily.md); combat: [07](./07-arena.md)
