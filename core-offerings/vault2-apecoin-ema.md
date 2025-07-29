# Vault2 — ApeCoin Dual EMA Strategy

This vault provides fully automated, passive exposure to a rules-based trading system.

### Strategy
- Applies a dual-period Exponential Moving Average (EMA) crossover system on the APE/USDC pair to generate buy or sell signals.
- Orders are executed fully automatically through Hyperliquid vault APIs.
- A trailing stop loss is used to retain profits in sideways markets. 
- No user setup is required—the vault produces consistent, transparent trend-following exposure.

### Fees
    On Ape Vault only performance fees apply, reduced over time in the system. 
- Month 1: 50% performance fee
- Month 2: 40% performance fee
- Month 3+: 35% performance fee

