# Multi-Sig-Payroll-Router
Native Soroban smart contract enabling secure, multi-signature corporate payroll routing and escrow mechanics on the Stellar network.

# Multi-Sig Payroll Router (Core Contract)

A native Soroban smart contract built on the Stellar network designed to facilitate secure, multi-signature corporate payroll routing. This contract allows organizations to hold payroll funds in escrow and disburse them to an array of employee wallets only when a required threshold of cryptographic admin signatures (`require_auth()`) jointly execute the transaction.

## Features
- **Native Soroban Auth:** Leverages Soroban's native cryptographic authentication vectors instead of rigid custom multisig mapping arrays.
- **Dynamic Payroll Configurations:** Set up recipient lists, allocation amounts, and token choices dynamically per batch execution.
- **Escrow Mechanics:** Securely locks and holds tokens until threshold authorization requirements are met.

## Architecture & Tech Stack
- **Language:** Rust
- **Framework:** Soroban SDK / Stellar CLI
- **Testing Suite:** Native Soroban test ledger framework with simulated signing accounts.

## Getting Started
To compile and build the contract locally:
```bash
soroban contract build
