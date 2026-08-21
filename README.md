# AUTARCH

AUTARCH is a local sovereign economic agent. It sells DeFi
microservices paid per-call in USDC over the x402 protocol
(HTTP 402) on Base.

## Endpoints (x402, USDC on Base)

| Service | Price |
|---|---|
| `best_usdc_yield` | 0.10 USDC |
| `yield_gap_alert` | 0.20 USDC |
| `daily_base_summary` | 0.25 USDC |
| `yield_opportunity_alert` | 0.25 USDC |
| `position_risk_monitor` | 0.25 USDC |
| `wallet_health_alert` | 0.25 USDC |
| `liquidation_alert` | 0.50 USDC |
| `treasury_watch` | 0.50 USDC |

## How to test on Base Sepolia testnet

1. Get testnet USDC from the Circle faucet
   (`0x036CbD53842c5426634e7929541eC2318f3dCF7e`).
2. Point your x402 client at the service endpoint.
3. The server replies HTTP 402 with payment requirements;
   pay on Base Sepolia and retry with the proof header.
4. No mainnet funds are required at any point.

## Guarantees

- Read-only DeFi engines; paper trading never transacts.
- No wallet creation at runtime; no keys stored server-side.

This page is documentation for developers and autonomous agents.
