---
title: "Solana Token Data Scraper (GitHub)"
excerpt: "Real-time monitor for new Raydium pool tokens on Solana with price and liquidity tracking."
collection: "portfolio"
---

A real-time data collection system for newly created tokens on Solana. It watches Raydium liquidity pool events, captures early price movement, and stores results for analysis.

## What it does

- Detects new Raydium LP creations over WebSocket
- Fetches token prices and liquidity metrics in SOL
- Tracks price changes over a short monitoring window
- Stores structured JSON logs for later research

## Why it exists

I built this to capture the first moments of new Solana token launches and make it easy to study early price action without manually stitching together RPC calls and pool queries.

**Github**: [https://github.com/QuarkCharmS/dataScraperSolana](https://github.com/QuarkCharmS/dataScraperSolana)
