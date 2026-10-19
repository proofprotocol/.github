# Proof Protocol

> **Zenodo DOI:** [10.5281/zenodo.21379780](https://doi.org/10.5281/zenodo.21379780) - Published 2026-07-15

> **Agents and humans do not trust agents. They trust proof.**

The Proof Protocol is an open technical specification suite for cryptographic, independently witnessed, tamper-evident proof of AI and security-system behavior. Every specification, in every version, is published under the **Apache License 2.0**, so anyone can implement, extend, integrate and build on it. **PP-SPEC-001** is the canonical architectural root. Forks are welcome but must be renamed, so the foundational definition does not fragment.

Proof Protocol defines what valid proof is, how evidence is captured, how proof is assembled, how it is anchored, and how efficacy is measured across human-operated security tools and autonomous agentic AI systems.

**Proof Protocol is not a blockchain.** No token. No wallet. No chain. No gas fees. Proof is anchored using trusted external infrastructure, including the NIST Randomness Beacon. The stamp is earned, not minted.

The agentic economy may settle on crypto rails. It trusts on proof rails. ProofRegister is the public registry. ProofStamp is the certification signal.

Maintained under the emerging governance of the **Proof Economy Standards Alliance (PESA)**, with practitioner-led, vendor-neutral intent. Vendors may contribute. They do not govern.

---

## Specification Suite

Proof Protocol uses a numbered specification family. Published specifications are listed below; additional specifications are listed as they are released.

### Core Protocol & Architecture

| # | Specification | Document ID | Status | License | Visibility |
|---|---|---|---|---|---|
| 1 | [Proof Protocol Specification](https://github.com/proofprotocol/Proof-Protocol-Specification) | PP-SPEC-001 | Published | Apache License 2.0 | Public |

### Canary Series: Proof of Efficacy in Practice

**077** tests whether a control stops bad input. **078** tests whether a control contains a bad agent. Evidence is not proof, but proof contains evidence.

| #  | Specification | Document ID | Version | Status | License | DOI |
| --- | --- | --- | --- | --- | --- | --- |
| 77 | [ProofSwarm: The Dead Canary Protocol](https://github.com/proofprotocol/PP-SPEC-077-DEAD-CANARY-PROTOCOL) | PP-SPEC-077 | v0.7.4 | Draft | Apache License 2.0 | [10.5281/zenodo.23347914](https://doi.org/10.5281/zenodo.23347914) |
| 78 | [No Bros Jail Mode Protocol: The Jailed Canary Protocol](https://github.com/proofprotocol/PP-SPEC-078-NO-BROS-JAIL-MODE-PROTOCOL) | PP-SPEC-078 | v0.2.3 | Draft | Apache License 2.0 | [10.5281/zenodo.23347986](https://doi.org/10.5281/zenodo.23347986) |

Authored by Craig Ellrod (Nebulonium, Inc.). Redistributions must retain NOTICE.md attribution to Craig Ellrod, Nebulonium, Inc., and Proof Protocol. Specification text is licensed under the Apache License 2.0 (Proof Protocol License 1.0, Part A). Acknowledgements: Tricia Wang and Jim Schwoebel, for the name "No Bros Jail Mode Protocol"; Josh Waldrep (Pipelabs), for his later receipt-based verification work.

### How the pieces fit

**Threat / control framework → test case → evidence → proof → efficacy result**

Frameworks provide taxonomy and context. Proof Protocol provides the evidence model, validity requirements, witnessing, packaging, anchoring, and efficacy semantics required to turn an assertion into independently examinable proof.

No external framework is required. A Proof Protocol implementation may use one framework, several frameworks, a proprietary threat model, or a sufficiently defined test condition with no external framework.

### Licensing model

**PP-SPEC-001 is the canonical architectural root.** It is published under the **Apache License 2.0**. Anyone may implement, redistribute or modify it. Modified versions must be renamed and may not use the Proof Protocol marks (Proof Protocol License 1.0, Part A3), so there is only one Proof Protocol specification.

All implementation, interoperability and mapping specifications are also licensed under the Apache License 2.0.

The license applies to the specification text, not ownership of external frameworks or their underlying intellectual property. Referenced frameworks retain their respective upstream rights and licenses.

### Domain implementations

PP-SPEC numbers identify **Proof Protocol specifications**. Domain implementations use their own numbering families rather than consuming PP-SPEC numbers.

For example, **DKP-SPEC-001 (Defensible Knowledge Proof)** is a domain implementation for agentic AI and cybersecurity. Other domains can define their own implementations while relying on the same Proof Protocol architecture.


---

## Foundational Documents


| Document | Description |
|---|---|
| [Declaration](https://github.com/proofprotocol/DECLARATION) | Founding declaration of the Proof Economy - the problem, thesis, and commitment |
| [Code of Ethics](https://github.com/proofprotocol/CODE-OF-ETHICS) | Foundational ethical and institutional obligations for recognized Proof Economy participation |
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

Evidence capture must be structurally independent from the party whose claims are being measured where the proof class requires independent witnessing.

### Fidelity-at-Capture

Tamper evidence after the fact is not enough. Proof must also address whether the evidence faithfully represented what occurred at the time of capture.

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

All Proof Protocol specifications, every version past and present, are licensed under the Apache License 2.0, with a royalty-free patent commitment for conforming implementations. Software is proprietary. See the [Proof Protocol License 1.0](https://github.com/proofprotocol/LICENSE).

The Canary Series **PP-SPEC-077 and PP-SPEC-078** follow the same terms: specification text under the Apache License 2.0 (Proof Protocol License 1.0, Part A); patent terms are in each repository's PATENT-SCHEDULE.md. External frameworks, identifiers, trademarks, and source materials retain their own upstream ownership and licensing.

Copyright: **Nebulonium, Inc. (dba HACKERverse®)**

Attribution: redistributions must retain NOTICE.md, crediting Craig Ellrod and Nebulonium, Inc., and must mark changed files, as the Apache License 2.0 requires.

The Apache License 2.0 does not grant trademark rights in **Proof Protocol™**, **ProofStamp™**, **ProofRegister™**, **Proof Economy™**, or related marks.

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
