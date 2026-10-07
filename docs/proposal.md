# KaiPay

_AI-powered agent that automates cross-border stablecoin remittances for migrant workers_

## Summary

KaiPay is an AI agent that lets migrant workers set up recurring, rule-based stablecoin transfers to family abroad, automatically converting local fiat on-ramps into USDC and delivering it via Solana Pay to a recipient's phone number. The agent monitors FX rates and splits payments across bills, savings, and cash-out to minimize fees and maximize value received.

## Target users

Migrant workers sending remittances and their families receiving funds in emerging markets

## Problem

Traditional remittance services charge 5-10% fees and require manual, repetitive transfers with little flexibility for recipients.

## Solution

An AI agent with a non-custodial Solana wallet automates recurring stablecoin transfers, phone-number-based delivery, and smart allocation rules set once by the sender.

## MVP features

- Solana Pay integration for phone-number-based USDC transfers
- AI agent that schedules and splits recurring remittances by rule
- Local on/off-ramp simulation for fiat-to-USDC conversion in MVP
- Dashboard showing fee savings vs traditional remittance services
- SMS/WhatsApp notification stub for recipients without crypto knowledge

## Chains

Solana

## Tech

Solana Pay, Rust/Anchor, USDC, React, Node.js, OpenAI API, Twilio (mock)

## Category

Payments

## Why now

Stablecoin remittance volume on Solana is growing fast due to near-zero fees and sub-second settlement, making AI-automated recurring transfers newly viable.

## Roadmap

- Partner with a local fiat on/off-ramp provider for real payouts
- Add multi-currency support and recipient-side cash-out network
- Launch pilot with a diaspora community for real remittance flows
