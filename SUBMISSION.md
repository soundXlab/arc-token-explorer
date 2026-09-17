# Arc Token Explorer — Microgrant Submission

## Live Demo
**https://arc-dashboard-sepia.vercel.app**

## GitHub
**https://github.com/soundXlab/arc-token-explorer**

---

## What it does

Arc Token Explorer is a **real-time analytics dashboard** for Arc Mainnet tokens. It tracks 20 tokens across utility and meme categories, pulling live data from two independent sources:

- **GeckoTerminal API** — prices, FDV, 24h volume, market cap, token images
- **DexScreener API** — transaction counts (buys/sells), liquidity, pair creation time

The dashboard automatically refreshes every 60 seconds and presents the data in three views:
1. **Tokens** — sorted by market cap with price, change, volume
2. **Top Movers** — ranked by 24h price change (gainers first)
3. **Volume Leaders** — ranked by 24h trading volume

Clicking any token opens a detail modal with:
- Interactive price chart (TradingView Lightweight Charts)
- Full stats: MCap, FDV, Vol, Buys/Sells ratio, 6h change
- Direct links to DexScreener, GeckoTerminal, and Arc Explorer

## Why this matters for Arc

Arc Mainnet launched September 16, 2026. The ecosystem has:
- 20+ tokens with measurable liquidity
- Active DEX trading on Uniswap v3/v4 forks
- NFT projects (ArcLand, 132/2500 parcels claimed)

But there's **no simple way to see what's happening on Arc** without knowing which DEX to check. This tool solves that.

## Technical highlights

- **Zero dependencies** — vanilla HTML/CSS/JS, one CDN for charts
- **No wallet required** — read-only, works for anyone
- **Double-source validation** — GeckoTerminal + DexScreener, cross-checked
- **Responsive** — works on mobile and desktop
- **Fail-open** — if one API is down, the other still shows data

## What I learned building this

- Arc has a real, active token ecosystem with $5M+ daily volume
- GeckoTerminal blocks anonymous requests; DexScreener is more reliable
- The "no RPC needed" approach works well for read-only tools
- Token metadata (images, descriptions) lives in GeckoTerminal, not DexScreener

## What's next (if funded)

1. **Historical klines** — fetch 7d/30d price history from DexScreener
2. **Price alerts** — browser notifications when a token moves >10%
3. **Portfolio tracker** — users add their holdings, see total PnL
4. **ArcLand NFT map** — integrate parcel data from app.arcworld.io
5. **New pair alerts** — monitor for freshly created DEX pairs

## Stack

- Frontend: Vanilla HTML/CSS/JS
- Charts: TradingView Lightweight Charts v4
- Data: DexScreener API + GeckoTerminal API
- Hosting: Vercel (free tier)
- Repo: GitHub

## Eligibility

- ✅ Deployed and working on Arc Mainnet
- ✅ Public repo with README
- ✅ No prior funding from Circle/Arc programs
- ✅ One submission, one project
