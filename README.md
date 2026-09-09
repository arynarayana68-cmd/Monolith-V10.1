## The Monolith V10.1 & Vanguard Reserve Utility Infrastructure

> Sovereign, edge-native microservice architecture and ERC-4337 closed-loop retail settlement engine deployed on Base.

---

## Executive Overview
The Monolith V10.1 is an ultra-lightweight daemon designed to eliminate SaaS rent and payment interchange drag (2.5%–3.5%) for brick-and-mortar retail merchants. Built for low-footprint, high-reliability edge execution, the system processes point-of-sale telemetry, validates merchant ingress payloads, and batches non-speculative loyalty states on Base Layer-2.

## Core Architectural Pillars

* **Ultra-Low Memory Footprint**: Single-file Node.js/Express ingress gateway (`monolith.js`) running under a strict `<15MB` RAM ceiling with automated PM2 process isolation and self-healing.
* **Cryptographic Ingress Security**: Sub-millisecond HMAC-SHA256 signature verification with nonce replay protection and constant-time string comparison.
* **Resilient Ingress Buffering**: Autonomous Dead-Letter Queue (DLQ) with stream-based payload rotation, preventing dropped events during network disruptions.
* **Frictionless Consumer Passkeys**: ERC-4337 account abstraction on Base Mainnet. Consumers scan countertop QR codes and redeem rewards via mobile browser passkeys in `<5 seconds` with zero gas fees.
* **Closed-Loop Compliance**: Governed by the True Face BPS model as a strict, non-speculative commercial loyalty utility (zero external secondary market trading).

---

## Technical Specifications

| Parameter | Specification |
|---|---|
| **Settlement Layer** | Base L2 (EVM Equivalence) |
| **Ingress Daemon** | Node.js / Express / PM2 Cluster |
| **RAM Utilization** | `<15MB` baseline operational ceiling |
| **Verification Latency** | `<500ms` point-of-sale verification SLA |
| **Gas Policy** | Pre-flight ceiling check (`<100 gwei`) via grant paymaster |
| **Telemetry Encryption**| SHA-256 one-way hashing & data minimization |

---

## Repository Structure
├── monolith.js          # Core ingress daemon & POS webhook listener
├── controller/          # Base L2 telemetry & gas relayer balancing
├── dlq/                 # Dead-Letter Queue rotation & redrive scripts
└── config/              # Ingress configuration & HMAC secret handling
