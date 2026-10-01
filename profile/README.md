# Proof Protocol

> **Zenodo DOI:** [10.5281/zenodo.21379780](https://doi.org/10.5281/zenodo.21379780) — Published 2026-07-15

> **Agents and humans do not trust agents. They trust proof.**

The Proof Protocol is an open technical specification suite for cryptographic, independently witnessed, tamper-evident proof of AI and security-system behavior. It is **open to implement and extend**, while the foundational architecture in **PP-SPEC-001** is preserved as the canonical, non-derivative specification under **CC BY-ND 4.0**. Implementation, interoperability, and framework-mapping specifications may use more permissive licenses, including **CC BY 4.0**, so the ecosystem can adapt, integrate, and build on the protocol without fragmenting its foundational definition.

Proof Protocol defines what valid proof is, how evidence is captured, how proof is assembled, how it is anchored, and how efficacy is measured across human-operated security tools and autonomous agentic AI systems.

**Proof Protocol is not a blockchain.** No token. No wallet. No chain. No gas fees. Proof is anchored using trusted external infrastructure, including the NIST Randomness Beacon. The stamp is earned, not minted.

The agentic economy may settle on crypto rails. It trusts on proof rails. ProofRegister is the public registry. ProofStamp is the certification signal.

Maintained under the emerging governance of the **Proof Economy Standards Alliance (PESA)**, with practitioner-led, vendor-neutral intent. Vendors may contribute. They do not govern.

---

## Specification Suite

Proof Protocol uses a numbered specification family. The suite separates the **canonical protocol architecture** from supporting technical specifications, architectural and economic papers, and **framework interoperability mappings**.

### Core Protocol & Architecture

| # | Specification | Document ID | Status | License | Visibility |
|---|---|---|---|---|---|
| 1 | [Proof Protocol Specification](https://github.com/proofprotocol/Proof-Protocol-Specification) | PP-SPEC-001 | Published | CC BY-ND 4.0 | Public |
| 2 | [Proof Validity Specification](https://github.com/proofprotocol/Proof-Validity-Specification) | PP-SPEC-002 | Published | CC BY 4.0 | Public |
| 3 | [ProofBundle Format Specification](https://github.com/proofprotocol/proofbundle-spec) | PP-SPEC-003 | Published | CC BY 4.0 | Public |
| 4 | [ProofRegistry API Specification](https://github.com/proofprotocol/registry-api-spec) | PP-SPEC-004 | Published | CC BY 4.0 | Public |
| 5 | [Witness Protocol Specification](https://github.com/proofprotocol/witness-spec) | PP-SPEC-005 | Published | CC BY 4.0 | Public |
| 6 | [Proof of Efficacy Score Specification](https://github.com/proofprotocol/pes-spec) | PP-SPEC-006 | Published | CC BY 4.0 | Public |
| 7 | [Agent-to-Agent Proof Protocol](https://github.com/proofprotocol/a2p-spec) | PP-SPEC-007 | Published | CC BY 4.0 | Public |
| 8 | [ProofChain Anchoring Specification](https://github.com/proofprotocol/proofchain-spec) | PP-SPEC-008 | Published | CC BY 4.0 | Public |
| 9 | [ProofStamp Certification Criteria](https://github.com/proofprotocol/proofstamp-criteria) | PP-SPEC-009 | Published | CC BY 4.0 | Public |
| 10 | [Legal Attestation Format](https://github.com/proofprotocol/legal-proof-format) | PP-SPEC-010 | Published | CC BY 4.0 | Public |
| 11 | [Proof Provenance Specification](https://github.com/proofprotocol/provenance-spec) | PP-SPEC-011 | Published | CC BY 4.0 | Public |
| 12 | [Proof Protocol Domain Framework](https://github.com/proofprotocol/domain-framework) | PP-SPEC-012 | Published | CC BY 4.0 | Public |
| 13 | Proof of Performance | PP-SPEC-013 | Draft (internal) | CC BY 4.0 | Private |
| 14 | Proof of Efficacy | PP-SPEC-014 | Draft (internal) | CC BY 4.0 | Private |
| 15 | [ProofTwin — Agent Behavioral Attestation Layer](https://github.com/proofprotocol/prooftwin-spec) | PP-SPEC-015 | Draft | CC BY 4.0 | Public |
| 16 | [AgenTwin — Configurable Agent Under Test](https://github.com/proofprotocol/agentwin-spec) | PP-SPEC-016 | Draft | CC BY 4.0 | Public |
| 17 | [PP-MCP Interface Standard](https://github.com/proofprotocol/pp-mcp-spec) | PP-SPEC-017 | Draft | CC BY 4.0 | Public |
| 18–22 | *Reserved* | PP-SPEC-018 – PP-SPEC-022 | — | — | — |

### Architectural, Integrity & Economic Specifications

| # | Specification | Document ID | Status | License | Visibility |
|---|---|---|---|---|---|
| 23 | [Structural Independence and the Fidelity-at-Capture Requirement](https://github.com/proofprotocol/Fidelity-at-Capture) | PP-SPEC-023 | Published | CC BY-ND 4.0 | Public |
| 24 | [The Self-Attestation Oxymoron](https://github.com/proofprotocol/Self-Attestation-Oxymoron) | PP-SPEC-024 | Published | CC BY-ND 4.0 | Public |
| 25 | Funding Tier Disclosure Oxymoron | PP-SPEC-025 | Draft — held pending release | CC BY-ND 4.0 | Private |
| 26 | [Proof-Derived Value and the Speculative Token Fallacy](https://github.com/proofprotocol/Proof-Derived-Value-and-the-Speculative-Token-Fallacy) | PP-SPEC-026 | Published | CC BY-ND 4.0 | Public |
| 27 | [Proven Efficacy and the Third Axis](https://github.com/proofprotocol/proven-efficacy) | PP-SPEC-027 | Published | CC BY-ND 4.0 | Public |
| 28–31 | *Reserved* | PP-SPEC-028 – PP-SPEC-031 | — | — | — |
| 32 | Non-Blocking Valid Proof | PP-SPEC-032 | Published — embargoed until 2026-10-31 | CC BY-ND 4.0 | Private |
| 33 | [Proof of Efficacy Mapping to the NIST AI RMF](https://github.com/proofprotocol/nist-ai-rmf-mapping) | PP-SPEC-033 | Published (v0.1.2) | CC BY-ND 4.0 | Public |

### Framework Interoperability Mappings

Threat and control frameworks are **pluggable inputs** to Proof Protocol. They can identify **what to test**. Proof Protocol independently establishes **whether the control worked and what evidence proves the result**.

A mapping establishes interoperability — **not architectural dependency**.

| # | Framework Mapping | Document ID | Status | License |
|---|---|---|---|---|
| 34 | [OWASP AIVSS](https://github.com/proofprotocol/PP-SPEC-034-owasp-aivss-mapping) | PP-SPEC-034 | Draft v0.1 | CC BY 4.0 |
| 35 | [ORCHIDEAS](https://github.com/proofprotocol/PP-SPEC-035-orchideas-mapping) | PP-SPEC-035 | Draft v0.1 | CC BY 4.0 |
| 36 | [AAGATE](https://github.com/proofprotocol/PP-SPEC-036-aagate-mapping) | PP-SPEC-036 | Draft v0.1 | CC BY 4.0 |
| 37 | [A2AS BASIC](https://github.com/proofprotocol/PP-SPEC-037-a2as-basic-mapping) | PP-SPEC-037 | Draft v0.1 | CC BY 4.0 |
| 38 | [Agent Name Service (ANS)](https://github.com/proofprotocol/PP-SPEC-038-ans-mapping) | PP-SPEC-038 | Draft v0.1 | CC BY 4.0 |
| 39 | [MITRE ATLAS](https://github.com/proofprotocol/PP-SPEC-039-mitre-atlas-mapping) | PP-SPEC-039 | Draft v0.1 | CC BY 4.0 |
| 40 | [NIST AI 100-2 — Adversarial Machine Learning](https://github.com/proofprotocol/PP-SPEC-040-nist-ai-100-2-mapping) | PP-SPEC-040 | Draft v0.1 | CC BY 4.0 |
| 41 | [OWASP Top 10 for Agentic Applications](https://github.com/proofprotocol/PP-SPEC-041-owasp-agentic-top10-mapping) | PP-SPEC-041 | Draft v0.1 | CC BY 4.0 |
| 42 | NIST SP 800-207 — Zero Trust Architecture | PP-SPEC-042 | Draft v0.1 | CC BY 4.0 | Public |
| 43 | EU AI Act | PP-SPEC-043 | Draft v0.1 | CC BY 4.0 | Public |
| 44 | SOC 2 / Trust Services Criteria | PP-SPEC-044 | Draft v0.1 | CC BY 4.0 | Public |
| 45 | ISO/IEC 42001 — AI Management Systems | PP-SPEC-045 | Draft v0.1 | CC BY 4.0 | Public |
| 46 | NIST SP 800-207A — Cloud-Native Zero Trust | PP-SPEC-046 | Draft v0.1 | CC BY 4.0 | Public |

### How the pieces fit

**Threat / control framework → test case → evidence → proof → efficacy result**

Frameworks provide taxonomy and context. Proof Protocol provides the evidence model, validity requirements, witnessing, packaging, anchoring, and efficacy semantics required to turn an assertion into independently examinable proof.

No external framework is required. A Proof Protocol implementation may use one framework, several frameworks, a proprietary threat model, or a sufficiently defined test condition with no external framework.

### Licensing model

**PP-SPEC-001 is the canonical architectural root.** It is published under **CC BY-ND 4.0** so the foundational definition can be redistributed and implemented without competing modified editions being distributed as variants of the specification.

Implementation, interoperability, and mapping specifications may use **CC BY 4.0** where adaptation is desirable. The framework-mapping series **PP-SPEC-034 through PP-SPEC-041** uses CC BY 4.0.

The license applies to the specification text, not ownership of external frameworks or their underlying intellectual property. Referenced frameworks retain their respective upstream rights and licenses.

### Domain implementations

PP-SPEC numbers identify **Proof Protocol specifications**. Domain implementations use their own numbering families rather than consuming PP-SPEC numbers.

For example, **DKP-SPEC-001 (Defensible Knowledge Proof)** is a domain implementation for agentic AI and cybersecurity. Other domains can define their own implementations while relying on the same Proof Protocol architecture.


---

## Foundational Documents

| Document | Description |
|---|---|
| [Declaration](https://github.com/proofprotocol/DECLARATION) | Founding declaration of the Proof Economy — the problem, thesis, and commitment |
| [Framework](https://github.com/proofprotocol/FRAMEWORK) | Structural framework governing how proof artifacts are produced, witnessed, and anchored |
| [Threat Model](https://github.com/proofprotocol/threat-model) | Living catalog of threat categories addressed by Proof Protocol |
| [License](https://github.com/proofprotocol/LICENSE) | Licensing policy and specification-level license terms |

---

## Core Concepts

### Evidence → Proof

Evidence is not automatically proof. Proof Protocol defines how evidence is captured, bounded, witnessed, assembled, validated, and registered so that claims can be examined independently.

### Proof of Efficacy

The operative question is:

> **Was there a control, and did it work?**

A control's presence, configuration, activation, detection event, and actual efficacy are different facts. Where a claim depends on a downstream protected outcome, proof requires evidence from the target, application, SIEM, vendor integration, or equivalent source sufficient to complete the evidence round trip.

### Framework-Agnostic Testing

Proof Protocol does not require a specific threat framework. MITRE ATLAS, NIST, OWASP, AIVSS, AAGATE, ORCHIDEAS, A2AS BASIC, ANS, proprietary threat models, or other frameworks may be used as test inputs without becoming dependencies of the Proof Protocol architecture.

### ProofBundle

A ProofBundle packages the proof record, evidence references, metrics, corpus manifest, environment context, timestamps, and related artifacts needed to examine a result.

### ProofStamp

ProofStamp is a certification mark awarded to qualifying proof artifacts under the applicable certification criteria. Meeting the Proof Protocol standard may be necessary, but certification is a separate determination.

### ProofRegister

ProofRegister is the registry layer for issued proof records and artifacts.

### Structural Independence

Evidence capture must be structurally independent from the party whose claims are being measured where the proof class requires independent witnessing. See PP-SPEC-023.

### Fidelity-at-Capture

Tamper evidence after the fact is not enough. Proof must also address whether the evidence faithfully represented what occurred at the time of capture. See PP-SPEC-023.

---

## What Is Not Automatically Proof

The following artifacts may be useful evidence, but by themselves do not establish a complete Proof Protocol result:

- log files, including signed logs;
- vendor-generated reports;
- screenshots or video;
- post-hoc hashes;
- incomplete evidence chains;
- self-controlled roots of trust;
- scores without disclosed denominator and case-classification methodology; and
- self-attesting benchmarks where the measured party controls the execution and evidence boundary.

See [PP-SPEC-002 — Proof Validity Specification](https://github.com/proofprotocol/Proof-Validity-Specification) for the applicable validity requirements.

---

## Governance

The Proof Protocol specification suite is currently maintained by **Nebulonium, Inc. (dba HACKERverse®)** as founding sponsor while the **Proof Economy Standards Alliance (PESA)** governance structure is being established.

The intended governance model is practitioner-led and vendor-neutral:

- practitioners and buyers govern;
- vendors may contribute;
- certification authority is separated from vendor self-attestation; and
- governance, recusal, disclosure, and integrity requirements are defined separately from technical interoperability.

PESA: [proofeconomy.foundation](https://proofeconomy.foundation)

---

## Reference Implementation

The reference implementation uses **ProofRegister** as a public registry for proof artifacts and **ProofStamp** as the certification signal.

The first published proof run referenced by this project:

| Field | Value |
|---|---|
| Product | Pipelock v3.0.0 |
| Campaign | PR-2026-08338 |
| Total Cases | 164 |
| Applicable Cases | 164 |
| PES Score | 73.2% containment / 100% detection |
| Anchor Block | 8339 |
| Child TTP Records | 164 |
| Certification | ProofStamp PS-2026-00001 |

Registry API: [api.proofregister.com/v1/records](https://api.proofregister.com/v1/records)

---

## Licensing

Licensing is defined per specification. The authoritative license is the license declared in the individual repository/specification.

The framework-mapping series **PP-SPEC-034 through PP-SPEC-041** is licensed under **CC BY 4.0**. External frameworks, identifiers, trademarks, and source materials retain their own upstream ownership and licensing.

Copyright: **Nebulonium, Inc. (dba HACKERverse®)**

Attribution: When sharing or adapting material under CC BY 4.0, credit the applicable author / Nebulonium, Inc. (dba HACKERverse®) and indicate changes where required by the license.

Creative Commons licensing does not grant trademark rights in **Proof Protocol™**, **ProofStamp™**, **ProofRegister™**, **Proof Economy™**, or related marks.

---

## Links

| | |
|---|---|
| Proof Economy Standards Alliance | [proofeconomy.foundation](https://proofeconomy.foundation) |
| ProofRegister | [proofregister.com](https://proofregister.com) |
| ProofRegister API | [api.proofregister.com/v1](https://api.proofregister.com/v1/) |
| Proof Protocol | [proofprotocol.io](https://proofprotocol.io) |
| HACKERverse | [hackerverse.ai](https://hackerverse.ai) |
| Proof Benchmark | [proofbenchmark.com](https://proofbenchmark.com) |

---

*Copyright 2026 Nebulonium, Inc. dba HACKERverse®. ProofStamp™ is a certification mark of Nebulonium, Inc.*
