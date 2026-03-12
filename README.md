# Java Blockchain - NoobChain

A simple blockchain implementation in Java, based on the tutorial by [CryptoKass](https://medium.com/programmers-blockchain/create-simple-blockchain-java-tutorial-from-scratch-6eeed3cb03fa).

## Features
- Blocks with SHA-256 digital signatures
- Proof of Work mining system
- Wallets with public/private key pairs (Elliptic Curve Cryptography)
- Signed transactions with ECDSA
- UTXO (Unspent Transaction Output) model
- Blockchain integrity validation
- Merkle root for transactions

## Tech Stack
- Java 11+
- Bouncy Castle (cryptography provider)
- Gson (JSON serialization)
- Gradle (build tool)

## How to Run
```bash
# Build
gradle build

# Run
gradle run
```

## Project Structure
```
src/main/java/noobchain/
├── Block.java              - Block with hash, mining, transactions
├── StringUtil.java         - SHA-256, ECDSA, Merkle root utilities
├── Transaction.java        - Transaction processing and signatures
├── TransactionInput.java   - References to unspent outputs
├── TransactionOutput.java  - Transaction output (who owns coins)
├── Wallet.java             - Key pair generation, balance, send funds
└── NoobChain.java          - Main class, blockchain, validation
```