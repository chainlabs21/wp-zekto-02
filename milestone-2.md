# Milestone 2 – June 2026: Scalability, Security, and User Abstraction

## 4.1 Privacy Phase 1

The first privacy phase introduces **selective data confidentiality** mechanisms, including partial transaction privacy and reduced metadata exposure. These features address core enterprise needs for confidentiality while preserving auditability.

Privacy Phase 1 focuses on **practical confidentiality** rather than full anonymity.

### Implemented Mechanisms

* Selective encryption of transaction payload fields
* Reduced on-chain exposure of sensitive metadata
* Separation of business logic data from settlement-critical state

### Policy-Driven Privacy Controls

Privacy controls are policy-driven, allowing:

* Enterprise-specific confidentiality configurations
* Controlled visibility for auditors and regulators
* Gradual introduction of cryptographic privacy without breaking existing tooling

This phased approach ensures compatibility with compliance frameworks such as financial reporting, audit trails, and lawful disclosure requirements.

---

## 4.2 Native Multisignature Support

KONET integrates **native multisignature functionality at the protocol level**, rather than relying solely on smart contracts. This delivers:

* Simplified key management
* Lower operational risk
* Enhanced security for institutional asset custody and governance

### Key Properties

* Multisig validation occurs during transaction verification, before execution
* Signature thresholds and signer sets are defined at the account level
* Reduced gas costs and attack vectors compared to contract-based multisig wallets

### Enabled Use Cases

This enables:

* Institutional-grade custody models
* Governance-controlled treasury accounts
* Secure validator and administrative operations

Native multisig significantly lowers operational complexity and reduces smart contract risk for high-value accounts.

---

## 4.3 Account Abstraction

Account Abstraction decouples user experience from traditional externally owned account (EOA) limitations. On KONET, this enables:

* Flexible authentication and recovery models
* Gas fee abstraction and sponsorship
* Web2-like user experience for Web3 applications

### Key Capabilities

* Custom validation logic (multi-factor auth, biometrics, hardware keys)
* Social and institutional recovery mechanisms
* Fee sponsorship and meta-transactions
* Application-specific account logic

### System Perspective

From a system perspective:

* Transactions are validated against abstracted account rules
* Gas payment responsibility can be delegated or pooled
* Wallet logic becomes upgradeable without protocol forks

This architecture enables **Web2-like user experiences** while maintaining blockchain-level security guarantees.

---

## 4.4 ZK Rollup Adoption

ZK Rollups introduce **cryptographic validity proofs**, enabling faster finality, stronger privacy guarantees, and improved scalability. Milestone 2 marks KONET's transition toward ZK-based execution as a core scalability layer.

ZK Rollups replace fraud-based guarantees with **cryptographic validity proofs**.

### Technical Benefits

* Immediate finality once proofs are verified
* No dispute windows
* Stronger privacy through proof-based state transitions

### Integration Design

KONET's ZK Rollup integration is designed to:

* Support multiple proving systems over time
* Allow hardware-accelerated proving
* Integrate privacy and scalability into a unified execution layer

This positions ZK Rollups as the long-term scalability backbone of the network.

