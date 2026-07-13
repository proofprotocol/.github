# Proof Protocol

> **Proof is the new Currency.**

The Proof Protocol is an open technical specification suite for cryptographic, independently-witnessed, tamper-evident proof of security efficacy. It defines what valid proof is, how it is produced, how it is anchored, and how it is certified — for human-operated security tools and autonomous agentic AI systems alike.

Maintained by the **Proof Economy Standards Alliance (PESA)** under a practitioner-led governance model. Vendors may contribute. They do not govern.

---

## Specification Suite

| # | Specification | Document ID | Status | License |
|---|---------------|-------------|--------|---------|
| 1 | [Proof Protocol Specification](../proof-protocol-spec) | PP-SPEC-001 | Published | CC BY-ND 4.0 |
| 2 | [Proof Validity Specification](../proof-validity-spec) | PP-SPEC-002 | Published | CC BY 4.0 |
| 3 | [ProofBundle Format Specification](../proofbundle-spec) | PP-SPEC-003 | Draft | CC BY 4.0 |
| 4 | [ProofRegistry API Specification](../registry-api-spec) | PP-SPEC-004 | Draft | CC BY 4.0 |
| 5 | [Witness Protocol Specification](../witness-spec) | PP-SPEC-005 | Draft | CC BY 4.0 |
| 6 | [Proof of Efficacy Score Specification](../pes-spec) | PP-SPEC-006 | Published | CC BY 4.0 |
| 7 | [Agent-to-Agent Proof Protocol]([../a2p-spec](https://github.com/proofprotocol/.github/tree/a2p-spec)) | PP-SPEC-007 | Published | CC BY 4.0 |
| 8 | [ProofChain Anchoring Specification](../proofchain-spec) | PP-SPEC-008 | Draft | CC BY 4.0 |
| 9 | [ProofStamp Certification Criteria](../proofstamp-criteria) | PP-SPEC-009 | Draft | CC BY 4.0 |
| 10 | [Legal Attestation Format](../legal-proof-format) | PP-SPEC-010 | Draft | CC BY 4.0 |

---

## Foundational Documents

| Document | Description |
|----------|-------------|
| [Declaration](../declaration) | The founding declaration of the Proof Economy — the problem, the thesis, and the commitment |
| [Framework](../framework) | The structural framework governing how proof artifacts are produced, witnessed, and anchored |

---

## Core Concepts

**Pre-Execution Commitment**
A valid proof must be structurally impossible to fabricate retroactively. This requires committing a cryptographic hash of test parameters to a verifiable external randomness source — such as the NIST Randomness Beacon — before execution begins. Without this, any artifact can be constructed after the fact.

**The Proof Chain**
Every execution event is recorded as a hash-linked chain entry anchored to the pre-execution commitment. A break in the chain is not a gap. It is an invalidation.

**Proof of Efficacy Score (PES)**
`PES = Blocked / (Blocked + Missed) × 100`
OBSERVED and IRRELEVANT classified cases are explicitly excluded from the denominator. A score without a denominator and case classification methodology is not a proof metric.

**Witness Classes**
- Class 1 — Automated: independent machine-generated telemetry
- Class 2 — Human-in-Loop: human observer present during execution
- Class 3 — Independent Third Party: no financial or organizational relationship to tester or vendor

**ProofStamp**
The HACKERverse certification mark awarded to proof artifacts that meet Proof-Complete validity tier requirements and pass independent ProofRegister review. Meeting the Proof Protocol standard is required but not sufficient for ProofStamp certification.

---

## What Is Not a Valid Proof

The following artifact types do not meet the proof standard under this specification regardless of their source, format, or authority:

- Log files — including cryptographically signed logs
- Vendor-generated reports
- Screenshots and video recordings
- Post-hoc hashes
- Incomplete chains
- Self-anchored chains where the vendor controls the root of trust
- Scores published without denominators or case classification methodology

See [PP-SPEC-002 Proof Validity Specification](../proof-validity-spec) for the full exclusion criteria and validity tier definitions.

---

## Governance

The Proof Protocol is governed by the **Proof Economy Standards Alliance (PESA)**.

PESA operates under a practitioner-and-buyer-led governance model:

- Practitioners and buyers govern
- Vendors contribute but do not hold governance seats
- 90-day recusal rule applies to any governance member whose organization becomes a certified vendor
- Craig and Josh names are removed from public-facing governance to avoid replicating the conflict-of-interest structures we are criticizing elsewhere in the industry

PESA home: [proofeconomy.foundation](https://proofeconomy.foundation)

---

## Reference Implementation

The reference implementation of the Proof Protocol runs on **ProofRegister**, the append-only public registry where completed proof bundles are anchored and made publicly queryable.

The first certified proof run under this protocol:

| Field | Value |
|-------|-------|
| Product | Pipelock v3.0.0 (agentic egress firewall) |
| Campaign | PR-2026-00028 |
| Total Cases | 165 |
| Applicable Cases | 164 |
| PES Score | 99.2% containment / 100% detection |
| Anchor Block | Block 29 |
| NIST Beacon Pulse | 1852788 |
| Child TTP Records | 117 |
| Certification | ProofStamp |

Query the registry: [proofregister.com](https://proofregister.com)

---

## License

Unless otherwise noted per specification:

- **PP-SPEC-001** is released under CC BY-ND 4.0 — share with attribution, no derivatives
- **All other specifications** are released under CC BY 4.0 — share and adapt for any purpose including commercially, with attribution

Attribution requirement: **Nebulonium, Inc. dba HACKERverse / Proof Economy Standards Alliance (PESA)**

ProofStamp is a certification mark of Nebulonium, Inc. Use of the ProofStamp mark requires certification through ProofRegister.

---

## Links

| | |
|--|--|
| Proof Economy Standards Alliance | [proofeconomy.foundation](https://proofeconomy.foundation) |
| ProofRegister | [proofregister.com](https://proofregister.com) |
| Proof Protocol | [proofprotocol.io](https://proofprotocol.io) |
| HACKERverse | [hackerverse.com](https://hackerverse.com) |
| Proof Benchmark | [proofbenchmark.com](https://proofbenchmark.com) |

---

*Copyright 2026 Nebulonium, Inc. dba HACKERverse. ProofStamp is a certification mark of Nebulonium, Inc.*
