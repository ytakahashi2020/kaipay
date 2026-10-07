# KaiPay
![KaiPay logo](assets/logo.png)

AI-powered agent that automates cross-border stablecoin remittances for migrant workers.

## Overview

KaiPay is an AI agent that lets migrant workers set up recurring, rule-based stablecoin transfers to family abroad. It automatically converts local fiat on-ramps into USDC and delivers it via Solana Pay to a recipient's phone number. The agent monitors FX rates and splits payments across bills, savings, and cash-out to minimize fees and maximize value received.

## Problem

Traditional remittance services charge 5-10% fees and require manual, repetitive transfers with little flexibility for recipients. Migrant workers often repeat the same transfer every month by hand, and recipients have no control over how funds are allocated once received.

## Solution

An AI agent with a non-custodial Solana wallet automates recurring stablecoin transfers, phone-number-based delivery, and smart allocation rules set once by the sender. The sender configures the rules a single time, and the agent handles scheduling, conversion, splitting, and delivery going forward.

## Features (MVP)

- Solana Pay integration for phone-number-based USDC transfers
- AI agent that schedules and splits recurring remittances by rule
- Local on/off-ramp simulation for fiat-to-USDC conversion in MVP
- Dashboard showing fee savings vs traditional remittance services
- SMS/WhatsApp notification stub for recipients without crypto knowledge

## Tech stack

Solana Pay, Rust/Anchor, USDC, React, Node.js, OpenAI API, Twilio (mock)

## How it works

```
Sender --> [Set recurring rules once]
            |
            v
     AI Agent (Node.js + OpenAI API)
      - monitors FX rates
      - schedules transfers
      - splits: bills / savings / cash-out
            |
            v
Local fiat on-ramp (simulated) --> USDC
            |
            v
   Solana (Rust/Anchor programs)
            |
            v
     Solana Pay --> Recipient (by phone number)
            |
            v
  SMS/WhatsApp notification (Twilio mock)
```

## Roadmap

- Partner with a local fiat on/off-ramp provider for real payouts
- Add multi-currency support and recipient-side cash-out network
- Launch a pilot with a diaspora community for real remittance flows

## Pitch

See [docs/pitch.pdf](docs/pitch.pdf) for the one-page pitch deck and [docs/pitch-script.md](docs/pitch-script.md) for the 1-minute spoken pitch script.

## Team

- Name — Role (placeholder)
- Name — Role (placeholder)
- Name — Role (placeholder)

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://ytakahashi2020.github.io/kaipay/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.
