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

### Bonus-Based Reinvestment Phase:
- Any subsequent deposit up to the **$1,000** buffer limit will trigger **no deposit fee**.
- The entire amount of this new deposit is immediately deployed into the vault.

### Buffer Reset Rule:
- Any new deposit that *exceeds* the current buffer (e.g., a $1,200 deposit when the buffer is $1,000) triggers a fee **only on the excess amount** ($200).
- The total buffer then recalibrates based on the latest total deposit size.

### Performance Fee Logic:
Performance fees are separate from deposit fees and apply only to trading profits.
- **20%** for a 1-month lock-up period.
- **15%** for a lock-up period of 3 months or more.

</details>

### Tier & Fee Summary
| Tier | Deposit Fee | Bonus Buffer | Performance Fee |
| :--- | :--- | :--- | :--- |
| **1** | 20% | Full deposit value | 20% / 15% |
| **2** | 18% | Full deposit value | Same |
| **3** | 15% | Full deposit value | Same |
| **4** | 10% | Full deposit value | Same |

### Why This Approach Matters
- **Encourages Reinvestment:** The buffer logic incentivizes subsequent deposits by eliminating immediate fees.
- **Rewards User Loyalty:** The tiered structure lowers friction for high-frequency or long-term users.
- **Keeps UI Simple:** A quick-view summary with an expandable section for advanced users.
- **Aligns Incentives:** Deposit fees fund operations (via bonus points), while performance fees align with successful long-term strategy execution.