# Vault2 — ApeCoin Dual EMA Strategy

This vault provides fully automated, passive exposure to a rules-based trading system.

### Strategy
- Applies a dual-period Exponential Moving Average (EMA) crossover system on the APE/USDC pair to generate buy or sell signals.
- Orders are executed fully automatically through Hyperliquid vault APIs.
- No user setup is required—the vault produces consistent, transparent trend-following exposure.

### Configurable Risk Modes
- **Conservative:** Smaller position size, tighter stop-loss, and slower compounding.
- **Aggressive:** Larger position size, wider stop levels, and faster exposure compounding.