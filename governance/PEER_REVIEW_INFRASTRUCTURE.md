# Peer Review Infrastructure
## DA_VALENCA_CORPUS_v1.0

**Richard Steven Vallance (Da Valenca)** | Da Valenca Leonardo Project
© 2026 Richard Steven Vallance — All Intellectual Property Reserved

---

> **DISTRIBUTION NOTICE**
> *This material is submitted for specialist critique only. It does not carry institutional endorsement, DOI registration, or public validation. It does not imply academic acceptance.*
> **Peer review state: RESTRICTED SPECIALIST REVIEW — NOT PUBLIC VALIDATION**

---

## Infrastructure Status

| Component | Status | Notes |
|---|---|---|
| Reviewer packets | ✗ NOT YET BUILT | To be assembled after governance complete |
| Adversarial review layer — Figura Ultima | ✗ NOT YET | Critical path before any public release |
| Reviewer response tracker | TEMPLATE READY | See below |
| Checksum manifests | ⚠ PARTIAL | `hashes.txt` in `da-vinci-mechanica`; others pending |
| Export zip | ✗ NOT YET | After binary deposits complete |
| Reviewer selection matrix | DRAFT | See below |

---

## Reviewer Response Tracker Template

For each reviewer, the following must be logged:

```
REVIEWER: [Anonymous ID or name if consented]
DATE SENT: 
DATE RECEIVED: 
DOCUMENT REVIEWED: 
RESPONSE SUMMARY: 
CLAIM CHALLENGES: 
  - [Claim]: [Challenge]: [RSV response]:
METHODOLOGY CHALLENGES:
  - [Method]: [Challenge]: [RSV response]:
RECOMMENDED CHANGES:
  - [Change]: [Priority]: [Status]:
INTEGRATION STATUS: [PENDING / IN PROGRESS / INTEGRATED / REJECTED WITH JUSTIFICATION]
VERSION TRIGGERED: [v1.1 / v1.2 / v2.0 / no change]
```

---

## Reviewer Selection Matrix

### Priority 1 — Mechanics / History of Technology
Target specialists with expertise in:
- Renaissance mechanical manuscripts (Reti tradition)
- History of clockmaking and precision instruments
- Tribology and friction history
- RWTH Aachen or similar Leonardo mechanical studies groups

Suggested institutions: Cambridge History of Science, Max Planck Institute for the History of Science, Istituto e Museo di Storia della Scienza (Florence).

### Priority 2 — Codicology / Manuscript Studies
Target specialists with expertise in:
- Italian Renaissance manuscript codicology
- BNE collections
- Ink migration and physical manuscript analysis

### Priority 3 — Optics / Digital Humanities (SolarScorch)
Target specialists with expertise in:
- Renaissance optics and mirror technology
- Solar geometry and astronomical computation
- GIS-based art history

### Priority 4 — Shroud Studies (Figura Ultima — Adversarial Review)
Adversarial framing required. Target specialists who:
- Are committed to rigorous falsification standards
- Have expertise in textile science, forensic imaging, or radiocarbon dating
- Have no prior public position on Shroud authorship

**The adversarial reviewer packet for Figura Ultima must lead with the strongest possible objections to the thesis and require RSV to respond to each in writing before release.**

---

## Checksum Manifest Template

For each deposited file, record:

```
FILE: [filename]
REPOSITORY: [repo name]
PATH: [full path]
SHA256: [to be computed]
FILE_SIZE_BYTES: [size]
DATE_FROZEN: [date]
FROZEN_VERSION: v1.0
NOTES: [any processing notes]
```

To be populated using `sha256sum` across all frozen files before release.

---

## Reviewer Packet Contents

Each reviewer packet must contain:
1. Cover letter stating: "RESTRICTED SPECIALIST REVIEW — NOT PUBLIC VALIDATION"
2. The relevant section(s) of the corpus
3. A targeted question list for the reviewer
4. The relevant section of `ECS_EVIDENCE_CLASSIFICATION_REGISTER.md`
5. The relevant section of `FALSIFICATION_PROTOCOLS.md`
6. The relevant section of `CLAIM_RISK_REGISTER.md`
7. A blank Reviewer Response form (template above)

**No reviewer packet implies academic acceptance, institutional endorsement, or prior validation.**

---

*© 2026 Richard Steven Vallance. All intellectual property reserved.*
