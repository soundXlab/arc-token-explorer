# Arc Microgrant Submission

## Project: Arc Token Explorer

**Live URL:** https://arc-dashboard-sepia.vercel.app

**GitHub:** Code available at `MEXC/tools/arc-dashboard/` (can be extracted as standalone repo)

## What the project does

Arc Token Explorer is a live dashboard that monitors 20 tokens on Arc Mainnet in real-time. It fetches price data, market caps, FDV, 24h volume, and price changes from DexScreener's API and displays them in a clean, auto-refreshing interface.

The project demonstrates:
- Real-time data consumption from Arc ecosystem APIs
- Understanding of Arc token diversity (utility + meme tokens)
- Clean, framework-free frontend implementation

## Why this matters for Arc

Arc Mainnet launched on September 16, 2026. This tool helps:
1. **New users** understand what tokens exist on Arc
2. **Builders** see that the ecosystem has active tokens with liquidity
3. **Researchers** track Arc token performance alongside their existing tools

## Tech stack
- Vanilla HTML/CSS/JavaScript (no frameworks)
- DexScreener API for token data
- Vercel for hosting
- Zero wallet dependency (read-only)

## Arc integration
- Queries Arc chain token data via DexScreener
- Shows Arc-native tokens: TOLLY, ARGUS, LONG, ASTRA, ADEX, ARCLAND, etc.
- All data is live from Arc Mainnet

## What I learned building this
- Arc has an emerging token ecosystem with both utility and meme tokens
- GeckoTerminal API had rate limits; DexScreener proved more reliable
- The "no wallet" approach makes the tool accessible to anyone
- Real-time dashboards are valuable for early-stage chain adoption

## What's next
- Add more Arc tokens as they launch
- Integrate ArcLand NFT data
- Add historical price charts
- Connect to Arc mainnet RPC for on-chain data (when RPC access is available)
