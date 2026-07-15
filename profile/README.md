# Proof Protocol

> **Zenodo DOI:** [10.5281/zenodo.21379780](https://doi.org/10.5281/zenodo.21379780) — Published 2026-07-15


> **Agents and humans do not trust agents. They trust proof.**

The Proof Protocol is an open technical specification suite for cryptographic, independently-witnessed, tamper-evident proof of AI and security system behavior. It defines what valid proof is, how it is produced, how it is anchored, and how it is certified - for human-operated security tools and autonomous agentic AI systems alike.

**Proof Protocol is not a blockchain.** No token. No wallet. No chain. No gas fees. Proof is anchored to the NIST Randomness Beacon - federal infrastructure operated by the National Institute of Standards and Technology. The stamp is earned, not minted.

The agentic economy settles on crypto rails. It trusts on proof rails. ProofRegister is the trust oracle. ProofStamp is the signal.

Maintained by the **Proof Economy Standards Alliance (PESA)** under a practitioner-led governance model. Vendors may contribute. They do not govern.

---

## Specification Suite

| # | Specification | Document ID | Status | License |
|---|---------------|-------------|--------|---------|
| 1 | [Proof Protocol Specification](https://github.com/proofprotocol/Defensible-Knowledge-Proof) | PP-SPEC-001 | Published | CC BY-ND 4.0 |
| 2 | [Proof Validity Specification](https://github.com/proofprotocol/Proof-Validity-Specification) | PP-SPEC-002 | Published | CC BY 4.0 |
| 3 | [ProofBundle Format Specification](https://github.com/proofprotocol/proofbundle-spec) | PP-SPEC-003 | Published | CC BY 4.0 |
| 4 | [ProofRegistry API Specification](https://github.com/proofprotocol/registry-api-spec) | PP-SPEC-004 | Published | CC BY 4.0 |
| 5 | [Witness Protocol Specification](https://github.com/proofprotocol/witness-spec) | PP-SPEC-005 | Published | CC BY 4.0 |
| 6 | [Proof of Efficacy Score Specification](https://github.com/proofprotocol/pes-spec) | PP-SPEC-006 | Published | CC BY 4.0 |
| 7 | [Agent-to-Agent Proof Protocol](https://github.com/proofprotocol/a2p-spec) | PP-SPEC-007 | Published | CC BY 4.0 |
| 8 | [ProofChain Anchoring Specification](https://github.com/proofprotocol/proofchain-spec) | PP-SPEC-008 | Published | CC BY 4.0 |
| 9 | [ProofStamp Certification Criteria](https://github.com/proofprotocol/proofstamp-criteria) | PP-SPEC-009 | Published | CC BY 4.0 |
| 10 | [Legal Attestation Format](https://github.com/proofprotocol/legal-proof-format) | PP-SPEC-010 | Published | CC BY 4.0 |
| 11 | [Proof Provenance Specification](https://github.com/proofprotocol/provenance-spec) | PP-SPEC-011 | Published | CC BY 4.0 |
| 12 | [Proof Protocol Domain Framework](https://github.com/proofprotocol/domain-framework) | PP-SPEC-012 | Published | CC BY 4.0 |
| 13 | [Proof of Performance](https://github.com/proofprotocol/Proof-of-Performance) | PP-SPEC-013 | Published | CC BY 4.0 |
| 14 | [Proof of Efficacy](https://github.com/proofprotocol/Proof-of-Efficacy) | PP-SPEC-014 | Published | CC BY 4.0 |

---

## Foundational Documents

| Document | Description |
|----------|-------------|
| [Declaration](https://github.com/proofprotocol/declaration) | The founding declaration of the Proof Economy - the problem, the thesis, and the commitment |
| [Framework](https://github.com/proofprotocol/framework) | The structural framework governing how proof artifacts are produced, witnessed, and anchored |
| [Threat Model](https://github.com/proofprotocol/threat-model) | The living catalog of threat categories the Proof Protocol covers - pre-dated, continuous, and adversarially executed |

---

## Core Concepts

**Pre-Execution Commitment**
A valid proof must be structurally impossible to fabricate retroactively. This requires committing a cryptographic hash of test parameters to the NIST Randomness Beacon before execution begins. Without this, any artifact can be constructed after the fact.

**The Proof Chain**
Every execution event is recorded as a hash-linked chain entry anchored to the pre-execution commitment. A break in the chain is not a gap. It is an invalidation.

**Proof of Efficacy Score (PES)**
`PES = Blocked / (Blocked + Missed) × 100`
OBSERVED and IRRELEVANT classified cases are explicitly excluded from the denominator. A score without a denominator and case classification methodology is not a proof metric.

**Witness Classes**
- Class 1 - Automated: independent machine-generated telemetry
- Class 2 - Human-in-Loop: human observer present during execution
- Class 3 - Independent Third Party: no financial or organizational relationship to tester or vendor

**AgenTwin**
The shadow attestation layer that witnesses agent runtime behavior from outside the agent trust boundary. Assembles receipt + pubkey + verifier output into a ProofBundle. The agent cannot forge its own receipt.

**ProofStamp**
The HACKERverse certification mark awarded to proof artifacts that meet Proof-Complete validity tier requirements and pass independent ProofRegister review. Meeting the Proof Protocol standard is required but not sufficient for ProofStamp certification. The stamp is earned. Not minted. Not self-declared.

---

## What Is Not a Valid Proof

The following artifact types do not meet the proof standard under this specification regardless of their source, format, or authority:

- Log files - including cryptographically signed logs
- Vendor-generated reports
- Screenshots and video recordings
- Post-hoc hashes
- Incomplete chains
- Self-anchored chains where the vendor controls the root of trust
- Scores published without denominators or case classification methodology
- Self-attesting benchmarks where the vendor controls the execution environment

See [PP-SPEC-002 Proof Validity Specification](https://github.com/proofprotocol/Proof-Validity-Specification) for the full exclusion criteria and validity tier definitions.

---

## Governance

The Proof Protocol is governed by the **Proof Economy Standards Alliance (PESA)**.

PESA operates under a practitioner-and-buyer-led governance model:

- Practitioners and buyers govern
- Vendors contribute but do not hold governance seats
- 90-day recusal rule applies to any governance member whose organization becomes a certified vendor

PESA home: [proofeconomy.foundation](https://proofeconomy.foundation)

---

## Reference Implementation

The reference implementation of the Proof Protocol runs on **ProofRegister**, the canonical public append-only registry where completed proof bundles are anchored and made publicly queryable. Not a blockchain. NIST Beacon anchored.

The first certified proof run under this protocol:

| Field | Value |
|-------|-------|
| Product | Pipelock v3.0.0 (agentic egress firewall) |
| Campaign | PR-2026-00028 |
| Total Cases | 165 |
| Applicable Cases | 164 |
| PES Score | 99.2% containment / 100% detection |
| NIST Beacon Pulse | 1852788 |
| Child TTP Records | 117 |
| Certification | ProofStamp PS-2026-00001 |

Query the registry: [api.proofregister.com/v1/records](https://api.proofregister.com/v1/records)

---

## License

Unless otherwise noted per specification:

- **PP-SPEC-001** is released under CC BY-ND 4.0 - share with attribution, no derivatives
- **All other specifications** are released under CC BY 4.0 - share and adapt for any purpose including commercially, with attribution

Attribution requirement: **Nebulonium, Inc. dba HACKERverse / Proof Economy Standards Alliance (PESA)**

ProofStamp is a certification mark of Nebulonium, Inc. Use of the ProofStamp mark requires certification through ProofRegister.

---

## Links

| | |
|--|--|
| Proof Economy Standards Alliance | [proofeconomy.foundation](https://proofeconomy.foundation) |
| ProofRegister | [proofregister.com](https://proofregister.com) |
| ProofRegister API | [api.proofregister.com/v1](https://api.proofregister.com/v1/) |
| Proof Protocol | [proofprotocol.io](https://proofprotocol.io) |
| HACKERverse | [hackerverse.ai](https://hackerverse.ai) |
| Proof Benchmark | [proofbenchmark.com](https://proofbenchmark.com) |

---

*Copyright 2026 Nebulonium, Inc. dba HACKERverse. ProofStamp is a certification mark of Nebulonium, Inc.*
