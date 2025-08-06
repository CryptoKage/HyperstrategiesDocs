# How Vault Deposits Work

Allocating your capital to a Hyper-Strategies vault is a straightforward process designed for transparency. Here's a step-by-step breakdown of what happens when you deposit.

### The Two-Step Process

All vault deposits follow a two-step settlement process for maximum security and efficiency.

**Step 1: The Allocation (Database Transaction)**

When you use the "Allocate Funds" modal on your dashboard, you are performing an instant, off-chain transaction within our internal ledger.

1.  The amount you specified is **subtracted** from your "Available to Allocate" balance.
2.  The platform calculates the **Deposit Fee** based on the specific vault and your [Account Tier](/user-guides/account-tiers.md).
3.  The fee amount is credited to your **Bonus Points** balance.
4.  The remaining capital is assigned to a new **Vault Position**, which now appears under "Your Positions" on the dashboard with a status of `active`.
5.  If the vault has a lock-in period (like the Core Vault), a **1-month timer** begins.

