# The Withdrawal Process

Withdrawing your capital from a vault is a secure, two-stage process.

### Stage 1: Requesting a Vault Withdrawal (Platform Level)

When your vault position is unlocked (e.g., after the 1-month lock-in on the Core Vault), you can initiate a withdrawal from your [**Dashboard**](/dashboard).

1.  Click the "Withdraw" button on an unlocked vault position.
2.  A withdrawal request for the **entirety** of that position is created.
3.  The request is placed in a queue with a `PENDING` status. You can see this new pending transaction in your [**Wallet Page**](/wallet) activity history.

> 💡 **What happens now?**
> This request notifies our admin team and trading desk that your capital needs to be returned from Hyperliquid. This unwinding process is handled with care and can take up to 48 hours.

### Stage 2: Processing & Credit (Backend Process)

Once our trading desk has returned your capital, our automated system runs a processing job.

1.  The job finds your `PENDING` withdrawal request.
2.  It confirms the funds have been returned.
3.  The full amount of your withdrawal is credited to your main **"Available to Allocate" balance**.
4.  The status of your withdrawal request in the activity log is updated to `COMPLETED`.

Your capital is now liquid and available within the platform. You can either allocate it to a new vault or proceed to Stage 3 to withdraw it from the platform entirely.

### Stage 3: Withdrawing from the Platform (On-Chain)

To move funds from your HyperStrategies account to an external wallet (like MetaMask), you must use the "Withdraw Funds" feature on your [**Wallet Page**](/wallet). This is a separate, on-chain transaction that sends USDC from our system to your specified address.