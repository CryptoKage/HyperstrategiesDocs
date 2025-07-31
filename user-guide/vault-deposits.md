# How Vault Deposits Work

Allocating your capital to a HyperStrategies vault is a straightforward process designed for transparency. Here's a step-by-step breakdown of what happens when you deposit.

### The Two-Step Process

All vault deposits follow a two-step settlement process for maximum security and efficiency.

**Step 1: The Allocation (Database Transaction)**

When you use the "Allocate Funds" modal on your dashboard, you are performing an instant, off-chain transaction within our internal ledger.

1.  The amount you specified is **subtracted** from your "Available to Allocate" balance.
2.  The platform calculates the **Deposit Fee** based on the specific vault and your [Account Tier](/user-guides/account-tiers.md).
3.  The fee amount is credited to your **Bonus Points** balance.
4.  The remaining capital is assigned to a new **Vault Position**, which now appears under "Your Positions" on the dashboard with a status of `active`.
5.  If the vault has a lock-in period (like the Core Vault), a **1-month timer** begins.

> 💡 At this point, your funds have been committed, but they have **not yet moved on the blockchain.** They are still safe in your personal deposit wallet.

**Step 2: The Sweep (On-Chain Transaction)**

Periodically, our automated system runs a "sweep" job (`processAllocations`) to settle all `active` positions.

1.  Our system sends a small amount of **ETH for gas** to your personal deposit wallet.
2.  It then initiates an on-chain transaction to **sweep the capital** (your Tradable Capital) from your wallet to our central trading desk wallet on Hyperliquid.
3.  Once the on-chain transaction is confirmed, the status of your vault position is updated to `in_trade`.

It is at this point that your capital is officially deployed and begins participating in the trading strategies. You will start earning time-weighted XP and become eligible for profit distributions.