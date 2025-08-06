# Withdrawal & Reinvestment Logic (Core1)

This system is designed to reward user loyalty and encourage reinvestment of capital.

### How It Works (Quick Overview)
- **Initial Deposit Fee:** A deposit triggers a fee (tier-dependent discounts available).
- **Active Allocation:** 80% of the deposit is deployed into Core1 trading; the remaining portion is issued as bonus points.
- **Bonus Buffer Mechanic:** An "effectively fee-free buffer" between 0% and 100% of the deposit value allows reinvested capital without further initial fees—up to the buffer size.
- **Tiered Fee Discounts:** Users in higher tiers pay lower initial deposit fees (down to 10%), reducing the bonus-point allocation accordingly.

<details>
<summary>Expand for Detailed Mechanics & Examples</summary>

### Initial Deposit Example:
- A User (Tier 1) deposits **$1,000**.
- A 20% fee (**$200**) is credited to the user as bonus points.
- **$800** is deployed into the trading vault.
- The user's "Bonus Buffer" is now set to **$1,000**.


### Performance Fee:
Performance fees are separate from deposit fees and apply only to trading profits.
- **20%** for a 1-month lock-up period.
- **15%** for a lock-up period of 3 months or more.

