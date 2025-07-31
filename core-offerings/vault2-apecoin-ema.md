# Vault2 — ApeCoin EMA Strategy

This vault provides fully automated, passive exposure to a rules-based trading system.

### Strategy

* Applies a dual-period Exponential Moving Average (EMA) crossover system on the APE/USDC pair to generate buy or sell signals.
* Orders are executed fully automatically through Hyperliquid vault APIs.
* A trailing stop loss is used to retain profits
* No user setup is required—the vault produces consistent, transparent trend-following exposure.

### Fees

```
Ape Vault fees are 10% Deposit (Credited as bonus points) and 40% performance fee
```

* Month 1: 50% performance fee
* Month 2: 40% performance fee
* Month 3+: 35% performance fee
