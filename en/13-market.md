# 13 NFT Marketplace

The marketplace trades **cattle, boxes, planets** and other on-chain assets (escrow listings, settled in IRT or USDT).

The in-game "Marketplace" building jumps to the **portal** marketplace (cowgalaxy.com/nftMarket).

## What you can do

| Function | Notes |
|---|---|
| Browse / filter / buy | Filter by bloodline, gender, form, stars, stats; sort by newest / lowest / highest price |
| List for sale | Card Package → NFT detail → Sell: pick currency (IRT / USDT), set price, approve, list |
| My listings | View, delist |
| History | Past trades |

Platform fee **2%** (deducted from the seller's proceeds). Bought NFTs go to the buyer's wallet; cattle must be put back in the shed to use.

---

## Filters (buyers, read this)

- **Bloodline**: Genesis / Normal; **Gender**: bull / cow; **Form**: box / calf / adult; **Stars**: 0 – 3  
- **Stat ranges**: base / combat / milk; Normal cattle show values already scaled by the star multiplier  
- **Dead cattle** are filtered out automatically  

> Even with an "adult" filter, **Normal adults cannot be newly listed** (next section). Adults you can buy are mostly **Genesis**.

---

## Which cattle can be sold / transferred

Hard on-chain rules. When the portal detail page has no "Sell" button, this is usually why — not a broken page.

| Asset | List on marketplace | Direct wallet transfer | Notes |
|---|---|---|---|
| **Normal calf** (not adult) | Yes | **No** | When priced in USDT, **minimum 150 USDT** |
| **Normal adult** | **No** | **No** | After adulthood: own use only (milk / combat / breeding / star-up material) |
| **Genesis** | Yes | Yes | No adulthood restriction |
| **Boxes, planet cards, skins, badges, vouchers** | By category | Yes | Frontier planet cards are not tradable |

Normal cattle (adult or not) can only be moved by game contracts, so wallet / portal "Transfer" fails for them. To trade a Normal cattle, list it **before adulthood**.

---

## Listing notes

1. **Approve** the marketplace contract in your wallet first  
2. Check the network (mainnet / testnet)  
3. **Normal adults cannot be listed**; cattle in the shed (staking / fighting / feeding / cooldown) must be removed to your wallet first  
4. Price with the 2% fee and liquidity in mind; delisting is free  

---

## Safety

- Use only the official portal entry  
- Verify contract address and domain  
- Test with a small trade before large ones  

Related: cattle stats → [02](./02-tokens-and-assets.md); other portal features → [14](./14-portal.md)
