## ✨ User Guide / Getting Started

### 1. Install & Connect Wallet

**Step-by-step wallet integration:**

1. Install **MetaMask** (or another EVM-compatible wallet).
2. Add the **HyperEVM** network:
   - RPC: `https://rpc.hyperliquid.xyz/evm`  
   - Chain ID: `999`  
   - Currency Symbol: `HYPE`
3. Confirm the connection and select the appropriate account when prompted.

---

### 2. Bridge & Deposit Assets

- Bridge assets (e.g. USDC or HYPE) onto HyperEVM.
- Once your wallet shows the correct balance, navigate to the **Core1** or **Vault2** deposit page.
- Choose your deposit amount and select a lock-up tier (1-month or 3-month+).
- Click **“Deposit”** and confirm the transaction in your wallet.

---

### 3. Dashboard & Strategy Overview

After depositing:

- Visit the **Dashboard**:
  - View **cumulative PnL**, **strategy allocation**, and **lock-up status**.
  - See your **tier level** and **bonus buffer remaining**.
  - Track performance metrics: **Sharpe ratio**, **drawdown**, **win rate**.
- Visit the **Rewards** panel:
  - Shows **$HYPE points earned**, **builder-fee income**, and **bonus buffer usage**.

---

### 4. Managing Strategy & Profits

**Auto-compound Logic:**

- Toggle **Auto Compound**:
  - **ON**: Profits stay in Hyperliquid and are redeployed in the next trades.
  - **OFF**: Profits are withdrawn to Hyper‑Strategies and are available for user withdrawal.

**Withdrawals & Buffer Logic:**

<details>
<summary>How withdrawals and bonus buffer work</summary>

- First deposit incurs a **deposit fee**, which becomes your **bonus buffer** (e.g. a 20% fee = bonus buffer = initial deposit).
- **Reinvest within buffer**: Your next deposit up to that buffer amount is **fee-free** and fully deployed.
- Deposits above buffer incur a new deposit fee on the excess only.
- Performance fees apply only on trading profit (20% for 1-month lock, 15% for 3-month+).
</details>

---

### 5. Using Strategy Tool Templates

When available:

- Navigate to the **Tools** section.
- Choose a strategy template (e.g. dual-EMA, trailing stop-loss).
- Connect using MetaMask and **approve builder fee usage**.
- Fund and deploy the strategy; trades will execute using Hyperliquid vault accounts.
- Builder fees (~0.01–0.1%) accrue to Hyper‑Strategies automatically.

---

### 6. Monitoring & Support

- View real-time **performance charts**, **trade fills**, and **PnL updates**.
- Track your **tier benefits**, **reward points**, and **token incentives**.
- Access **support** via:
  - Discord / Telegram
  - GitHub Discussions
  - Feedback forms in-app
