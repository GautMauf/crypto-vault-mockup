# Vault Risk Passport — Concept Mockup

A concept prototype exploring how Morpho Vaults could make externalized risk **legible, comparable, and monitorable** for institutional allocators.

**Thesis:** the binding constraint on the next $10B of vault deposits isn't yield or protocol capability — it's the cost of trust. A standardized, per-vault risk & compliance disclosure — human-readable for risk committees, machine-readable via API — collapses that cost. The idea is to reuse what TradFi is doing correctly while improving it, and adapting it to DeFi.

## Live demo

- **Vault Risk Passport** → https://gautmauf.github.io/crypto-vault-mockup/
- **Vaults list UI concept** (current Morpho UX + a Risk layer) → https://gautmauf.github.io/crypto-vault-mockup/vaults.html

## What's in the Passport (`index.html`)

- **Passport grade** with sub-scores — every score decomposes into verifiable facts, never a terminal number
- **Noncustodial guarantees** as actually configured on-chain: timelock, in-kind redemptions, gates, exposure caps, role segregation, sentinel
- **Live exposure & concentration** with curator caps, drift alerts, and transitive-risk **look-through** (wrappers and adapters, scanned in depth)
- **Term exposure** for fixed-rate (Midnight) allocations: maturity ladder, weighted average maturity, overnight liquidity floor, maturity walls, fixed-book valuation policy
- **Yield provenance**: native vs incentivized APY, campaign end date, budget runway — organic yield reconciled on-chain against the displayed rate
- **Skin in the game**: curator first-loss capital and coded waterfall
- **Curator track record & audit lineage**
- **Committee view / API view toggle** — the same passport as JSON, for an allocator's internal risk stack
- A machine-readable **MRZ strip**, because it's a passport

## What's in the Vaults UI concept (`vaults.html`)

A faithful reproduction of the Morpho Vaults list with one addition: a **Risk column** (toggle it in the filter bar to compare with the current UX), concentration-drift flags, and yield-provenance tooltips on incentivized APYs. The grade on the first row opens the Passport.

## Access it

Open `index.html` or `vaults.html` in a browser — no build, no dependencies.
