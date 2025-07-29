# Visualizing Performance

This section describes how Hyper‑Strategies visualizes vault performance, trading metrics, and strategy health to provide users with confidence and transparency.

### Dashboard Components
| Dashboard Area | Key Metrics Displayed | User Benefit |
| :--- | :--- | :--- |
| **Portfolio View** | Real-time PnL, asset allocation, lock-up status | Transparent snapshot of vault health |
| **Trade Activity** | Trade volume, order fills, entry/exit timestamps | Insight into execution and strategy behavior |
| **Performance** | Win rate, avg. return, drawdown, Sharpe ratio | Quantitative strategy performance indicators |
| **Token Rewards** | HYPE points earned, builder-fee income, buffer status | Reflects protocol and performance alignment |

### Data Sources & Architecture
- **On-Chain & API Data:** Utilizes Hyperliquid's Info API and WebSocket feeds (`WebData`, `User`, `AllMids`, `Candle`) to populate real-time frontend metrics.
- **Backend Analytics Engine:** Tracks executed trades, computes performance metrics, and stores historical data for graphing and comparisons.
- **Data Visualization Stack:** Charts and tables are rendered with modern libraries to provide interactive, easy-to-read visuals.

### Key UI Features
- **Historical Charting:** Line charts for cumulative return, drawdown, and weekly performance.
- **Strategy Health Panel:** Simple indicators such as win/loss ratio and trailing stop execution.
- **Tier and Buffer Indicator:** Displays your tier level, bonus buffer usage, and remaining fee-free allowance.
- **Reward Tracker:** Shows recent builder-fees earned and HYPE point accumulation per vault.

<details>
<summary>View Example Wireframe Concept</summary>

- **Top Bar:** Vault name, lock-up end date, tier level
- **Panel A:** Cumulative NAV line chart (X-axis: time; Y-axis: portfolio value)
- **Panel B:** Recent trades list with PnL, volume, and timestamp
- **Panel C:** Core statistics, including win rate, average trade return, max drawdown
- **Panel D:** Token rewards widget showing HYPE points and builder-fee accumulation
- **Panel E:** Bonus buffer gauge with remaining fee-free deposit allowance

</details>
