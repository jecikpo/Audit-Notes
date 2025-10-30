# Audit Notes
Some notes on web3 audits

# Fuel and Sway Resources

- Main Fuel [documentation resource](https://docs.fuel.network/docs/intro/what-is-fuel/)
- [The Sway Book](https://fuellabs.github.io/sway/v0.60.0/book/index.html)
- Fuel's [Rust SDK Docs](https://docs.rs/fuels/latest/fuels/all.html)
- [Sway Standards](https://github.com/FuelLabs/sway-standards/tree/v0.5.0)
- [Sway by Example](https://www.swaybyexample.com/)

## Blog Posts and Articles

- [Fuel VM Binary analysis](https://jtriley.substack.com/p/fuel-vm-binary-analysis) by jtriley.eth
- [Fuel Virtual Machine Architecture](https://substack.com/home/post/p-83088192) by jtriley.eth
- [Introduction to the Sway Language Security Audit](https://exvul.com/introduction-to-the-sway-language-security-audit/) by ExVul
- [A detailed write-up of a solo critical vulnerability discovered during the Immunefi Attackathon](https://github.com/minato7namikazi/Fuel-Blockchain-Critical-Vulnerability) by [Minato7namikazi](https://x.com/minato7namikazi)
- [Exploring the FuelVM](https://medium.com/blockchain-capital-blog/exploring-the-fuelvm-86cf9ccdc159) by Ryan Sproule

## Tools

- [Fuel Explorer](https://app.fuel.network/)
- [Fuel Bridge](https://app.fuel.network/bridge?from=eth&to=fuel)
- [Testnet Faucet](https://faucet-testnet.fuel.network/)
- [Fuel Disassembler](https://github.com/otrho/fuel-dis)
- [Fuel Debugger](https://github.com/fuellabs/fuel-debugger)
- [Sway Static Analyzer](https://github.com/ourovoros-io/sway-analyzer) and an [article explaining usage](https://medium.com/@angelos404/mastering-sway-analyzer-27379d7903db).

## JecikPo's Notes

- [FuelVM Storage](https://github.com/jecikpo/Audit-Notes/blob/main/Sway-storage.md) - Notes on Storage Design in FuelVM.

## JecikPo's tutorials

- [SRC20 Tutorial](https://github.com/jecikpo/Tutorial-Fuel-SRC20) - Step-by-step tutorial on how to create a simple SRC20 smart contract with some Rust tests.
- [UniswapV2 in Sway Tutorial](https://github.com/jecikpo/Tutorial-Sway-UniswapV2) - Tutorial explaining how to build a UniswapV2 clone (FuniswapV2) in Sway on Fuel.

# General Solana Resources

- [Ottersec Reports](https://ottersec.notion.site/Sampled-Public-Audit-Reports-a296e98838aa4fdb8f3b192663400772) - A great collection of public reports by OtterSec
- [Token-2022 Security Best Practices - Part 1](https://blog.offside.io/p/token-2022-security-best-practices-part-1) - Mint and Token Account by Offsite Labs
- [Token-2022 Security Best Practices - Part 2](https://blog.offside.io/p/token-2022-security-best-practices-part-2) - Extensions by Offsite Labs
- [Common Attack Vectors](https://github.com/Ackee-Blockchain/solana-common-attack-vectors/) - common issues related to mishandling of accounts by Ackee
- [Solana Program Security Course](https://github.com/solana-foundation/developer-content/tree/main/content/courses/program-security) - Basic Account Security by Solana Foundation
## Solana Internals

- [Under the Hood of Solana Program Execution From Rust Code to SBF Bytecode](https://ubermensch.blog/under-the-hood-of-solana-program-execution-from-rust-code-to-sbf-bytecode#heading-during-execution-vm-enforcement) - Basic info on SBF, compilation and Solana Bytecode by Farouk ELALEM
- [The Solana eBPF Virtual Machine](https://www.anza.xyz/blog/the-solana-ebpf-virtual-machine) by Joe Caulfield
- [Solana Bytecode / Instruction Set Architecture](https://github.com/solana-labs/rbpf/blob/57139e9e1fca4f01155f7d99bc55cdcc25b0bc04/doc/bytecode.md)

## Solana Fuzzing

- [A Practical Guide to Fuzzing Solana Smart Contracts with Honggfuzz](https://zokyo.io/blog/guide-to-fuzzing-solana/) - by Zokyo

## Solana Reverse Engienering

- [Reverse Engineering Solana with Binary Ninja](https://osec.io/blog/2022-08-27-reverse-engineering-solana) - An introduction to our open-source Binary Ninja plugin for blackbox Solana program analysis along with an executive reference to the Solana runtime by Harrison Green (Aug 27, 2022)
- [Reverse Engineering Solana Programs: A Practical Guide to Unpacking Closed-Source BPF](https://medium.com/@evansaboladed/reverse-engineering-solana-programs-a-practical-guide-to-unpacking-closed-source-bpf-6994c1eaa33c) - Tools, Techniques, and Challenges for Analyzing On-Chain Solana Logic by DeepW

# Hyperliquid Resources

- [Implementation and Security Pitfalls of LST on Hyperliquid](https://medium.com/@talfao_94085/implementation-and-security-pitfalls-of-lst-on-hyperliquid-b83b8fd42713) - by Talfao