# 13 NFT Marketplace

The marketplace is for buying and selling **cattle, blind boxes, planets**, and other on-chain assets (escrow listings; settlement currencies follow the page).

The in-game “Marketplace” building usually jumps to the **portal** market page.

## What you can do

| Feature | Notes |
|---|---|
| Browse / filter & buy | Filter by bloodline, gender, form, stars, stats |
| List for sale | Pick asset, set price, approve, then list |
| My listings | View, delist |
| Trade history | Past buys and sells |

The platform takes a fee (rate follows the contract / page display).

---

## Filters (must-read for buyers)

Common filters:

- **Bloodline**: Genesis / Normal  
- **Gender**: bull / cow  
- **Form**: blind box / calf / adult  
- **Stars**: 0–3 (usually only meaningful for Normal adults)  
- **Stat ranges**: base / combat / milk, etc.  

Combination rules (concept):

- Bloodline, gender, form, and stars often combine with OR-style multi-select  
- Stat conditions are mostly AND  
- **Dead cattle** are auto-filtered out of normal lists  

> Even if the UI still has an “adult” form filter, **Normal adult cattle cannot be newly listed** (see below). Listings that look “adult” are mainly **Genesis cattle** (no lifespan; always tradable).

---

## Which cattle can be sold

This is an on-chain rule. If the portal detail page has no **Sell** button, it is usually this restriction — not a UI bug.

| Asset | Can list on NFT market | Notes |
|---|---|---|
| **Normal calf** (not adult) | Yes | Detail page shows Sell; **USDT listings must be at least 150 USDT** (contract `Price-288`) |
| **Normal adult cattle** | **No** | Cannot list after they grow up; **transfer** to another address is still allowed |
| **Genesis cattle** | Yes | Not blocked by adult status |
| **Boxes, planets, other NFTs** | By type | Follow the detail-page buttons and the contract |

So: trade Normal cattle **before adulthood**. After adulthood they are for your own play (milk / combat / breeding) or wallet transfer only.

---

## Listing tips

1. First **approve** the market contract in your wallet  
2. Confirm the correct network (don’t mix mainnet / testnet)  
3. **Normal adult cattle cannot be listed**; cattle that are staked, in combat, or on breeding CD may also fail to list  
4. Price with fees and liquidity in mind — avoid dead listings forever  

---

## Safety tips

- Enter the market only via the official portal  
- Verify contract addresses and domains  
- For large trades, test with a small amount first  

Related: cattle stats → [02](./02-tokens-and-assets.md); other portal features → [14](./14-portal.md)
