# mfp-auto-trading
       ┌──────────────────────┐
       │   Market Data Stream │
       │   (WebSocket / API)  │
       └──────────┬───────────┘
                  │
                  ▼
       ┌──────────────────────┐
       │   Select Timeframe   │
       │  1m / 5m / 15m / 1h  │
       └──────────┬───────────┘
                  │
                  ▼
       ┌──────────────────────┐
       │   Calculate MACD     │
       │   MACD + Signal Line │
       │   Histogram          │
       └──────────┬───────────┘
                  │
                  ▼
       ┌──────────────────────┐
       │   Signal Detection   │
       │                      │
       │  MACD Cross Above    │
       │      → BUY           │
       │                      │
       │  MACD Cross Below    │
       │      → SELL          │
       └──────────┬───────────┘
                  │
                  ▼
       ┌──────────────────────┐
       │  Automated Trading   │
       │                      │
       │  Open / Close Orders │
       │  Manage Positions    │
       └──────────┬───────────┘
                  │
                  ▼
       ┌──────────────────────┐
       │   Broker / Exchange  │
       │   Order Execution    │
       └──────────────────────┘