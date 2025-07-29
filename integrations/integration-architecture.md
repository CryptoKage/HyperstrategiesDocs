# Integration with Hyperliquid

### Why Hyperliquid Is Ideal for Integration
Hyperliquid is built on a high-speed, on-chain central limit order book designed for derivatives trading. With one-block finality, zero gas fees, and throughput supporting hundreds of thousands of orders per second, it is uniquely suited for our automated strategy execution.

### Integration Architecture
Our system leverages Hyperliquid's powerful and secure APIs for all operations.

#### API Wallets & Vault Accounts
Hyperliquid offers vault-level sub-accounts and API agent wallets with trading permissions only (no withdrawal access). This enables secure client execution without exposing user funds to unnecessary risk.

#### Info Endpoint (Market + User Data)
Provides marketplace data (`AllMids`, `Candle`, orderbook) as well as vault/account status like `user_state`, `open_orders`, and builder fee approvals.

#### Exchange Endpoint (Execution API)
Handles placement, modification, and cancellation of orders—including TWAP, scaled orders, and builder fee embedding via payload fields for revenue attribution.

#### WebSocket Feeds
Real-time data streams are available for:
- **Market data:** `AllMids`, `L2Book`, `Candle`
- **User data:** `WebData` (fills), `User` (account updates)

#### Builder Code System
Hyperliquid allows users to pre-approve a "builder" address and a maximum fee. Our strategy orders used through our front end or various tools can then include a payload to attribute the trade volume to us.