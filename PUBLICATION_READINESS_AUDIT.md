# PUBLICATION_READINESS_AUDIT.md
## Publication Readiness Audit — DA_VALENCA_CORPUS_v1.0

**Richard Steven Vallance (Da Valenca)** | Corpus Leonardianum Universale
**Audit date:** May 2026
© 2026 Richard Steven Vallance — All Intellectual Property Reserved

---

## CURRENT STATUS

> **PEER REVIEW READY / PUBLICATION CANDIDATE PENDING REVIEW**

This status applies to the mechanica stream (da-vinci-mechanica) and solar analysis stream (solarscorch) only.

The Figura Ultima / Shroud stream is currently:
> **INTERNAL READY — ADVERSARIAL REVIEW REQUIRED BEFORE PEER REVIEW SUBMISSION**

---

## Audit Categories

### 1. Freeze Integrity

| Item | Status | Notes |
|---|---|---|
| Corpus freeze declared (v1.0) | ✓ COMPLETE | FREEZE_GOVERNANCE_v1.0.md in da-vinci-ultimatium |
| Version control protocol documented | ✓ COMPLETE | v1.1/v1.2/v2.0 triggers defined |
| No silent overwriting policy documented | ✓ COMPLETE | |
| Checksum manifest generated | ✗ NOT COMPLETE | Required before publication candidate status |

**Freeze Integrity:** PARTIAL — checksum manifest pending

---

### 2. Bibliography and Citation Status

| Item | Status | Notes |
|---|---|---|
| Master bibliography constructed (Chicago N&B) | ✓ COMPLETE | bibliography/MASTER_BIBLIOGRAPHY.md |
| Source reference register constructed | ✓ COMPLETE | bibliography/SOURCE_REFERENCE_REGISTER.md |
| All PENDING_VERIFICATION entries resolved | ✗ NOT COMPLETE | 4 entries pending: Manuscript D IIIF URL, Arundel folio-level, Barbet edition, RSV&French publication status |
| Windsor RCIN folio-level verification | ✗ NOT COMPLETE | Ch. IX anatomical folio citations unverified |
| Duplicate citations removed | ✓ COMPLETE | |
| BNE transcript citations complete (Batches 1–5) | ✓ COMPLETE | 36 entries verified |
| BNE gap (files 5916–5953) | ✗ PENDING | 38 folios held locally; PC-7–9 pending write-up |

**Bibliography:** PARTIAL — 4 verification flags unresolved

---

### 3. Evidential Firewall Compliance

| Item | Status | Notes |
|---|---|---|
| ECS five-type classification system documented | ✓ COMPLETE | evidence/ECS_EVIDENCE_CLASSIFICATION_REGISTER.md |
| Every major claim classified by evidence type | ✓ COMPLETE | All corpus claims registered |
| No TYPE_C presented as TYPE_A (audit needed) | ⚠ REQUIRES PASS | Mechanical audit of all document prose not yet done |
| Claim risk register complete | ✓ COMPLETE | evidence/CLAIM_RISK_REGISTER.md |
| Falsification protocols documented | ✓ COMPLETE | evidence/FALSIFICATION_PROTOCOLS.md |
| Language discipline (banned phrases) | ⚠ REQUIRES PASS | Mechanica stream likely compliant; Figura Ultima prose audit required |

**Evidential Firewall:** FRAMEWORK COMPLETE — prose audit still required

---

### 4. Figure Permissions

| Item | Status | Notes |
|---|---|---|
| Figure registry constructed | ✓ COMPLETE | figures/FIGURE_AND_PLATE_REGISTRY.md |
| BNE Interactivo research use confirmed | ✓ COMPLETE | Free for research use with attribution |
| Vitruvian Man permission | ✗ NOT CONFIRMED | Gallerie dell'Accademia contact required |
| Windsor anatomical RCIN permission | ✗ NOT CONFIRMED | Royal Collection Trust contact required |
| STURP images permission | ✗ NOT CONFIRMED | STURP / Diocese of Turin contact required |
| Enhanced images labelled PROVISIONAL | ✓ POLICY SET | Application to all existing enhanced images in docs pending |

**Figure Permissions:** REGISTRY COMPLETE — multiple permission confirmations outstanding

---

### 5. Lexicon Consistency

| Item | Status | Notes |
|---|---|---|
| Banned language list documented | ✓ COMPLETE | CLAIM_RISK_REGISTER.md language discipline section |
| 'Proof'/'definitively' in Figura Ultima removed | ⚠ REQUIRES PASS | Full prose audit needed |
| 'Candidate framework'/'testable model' language verified | ⚠ REQUIRES PASS | Audit of ECS-classified sections needed |
| 'Shroud attribution hypothesis' never stated as fact | ⚠ REQUIRES PASS | Critical before any public-facing release |

**Lexicon:** STANDARDS DOCUMENTED — compliance audit not yet run

---

### 6. Reviewer Packet Status

| Item | Status | Notes |
|---|---|---|
| Peer review infrastructure defined | ✓ COMPLETE | Pathway in PUBLICATION_SEQUENCE_MASTER.md |
| Adversarial review layer defined | ✓ COMPLETE | Figura Ultima: mandatory before peer review |
| Reader entry points created (8 pathways) | ✓ COMPLETE | navigation/READER_ENTRY_POINTS.md |
| Compression layer (500w / 5kw / 20kw summaries) | ✗ NOT COMPLETE | Flagship publication concept defined; text not written |
| Reviewer selection matrix | ✗ NOT COMPLETE | To be developed at PEER REVIEW READY stage |
| Checksum manifests | ✗ NOT COMPLETE | Required at publication candidate stage |
| Export zip | ✗ NOT COMPLETE | Required at publication candidate stage |

**Reviewer Infrastructure:** PARTIALLY COMPLETE

---

### 7. Unresolved Verification Flags

| Flag | Document | Status |
|---|---|---|
| Manuscript D IIIF URL | SOURCE_REFERENCE_REGISTER | PENDING_VERIFICATION |
| British Library Arundel folio-level | SOURCE_REFERENCE_REGISTER | PENDING_VERIFICATION |
| Barbet 1953 edition details | MASTER_BIBLIOGRAPHY | PENDING_VERIFICATION |
| Vallance & French "Real Engine" publication status | MASTER_BIBLIOGRAPHY | PENDING_VERIFICATION |
| Windsor RCIN folio-level (Ch. IX) | SOURCE_REFERENCE_REGISTER | PENDING_VERIFICATION |
| CA f.93r (viola organista alt. specification) | SOURCE_REFERENCE_REGISTER | PENDING_VERIFICATION |
| PC-7, PC-8, PC-9 | FREEZE_GOVERNANCE | PENDING — BNE 5916–5953 not yet deposited |

---

### 8. Release Governance

| Item | Status |
|---|---|
| DOI not assigned prematurely | ✓ CONFIRMED — DOI_REGISTRY.md |
| No implication of institutional endorsement | ✓ CONFIRMED |
| "Restricted specialist review" language in all peer review packets | ✓ POLICY SET |
| No public release approved | ✓ CONFIRMED |
| Turin-shroud-white-paper rebuild pending | ✓ CONFIRMED — repo marked reserved |

---

## Publication Readiness Summary by Stream

| Stream | Current Status | Gate to Next Level |
|---|---|---|
| da-vinci-mechanica (mechanica) | **PEER REVIEW READY** | Confirmation of content from RSV; GitHub release + Zenodo DOI |
| solarscorch | **PEER REVIEW READY** | Full paper adversarial review; resolve 156.4° anomaly documentation |
| principia-mechanica | **INTERNAL READY** | Binary docx deposit; Windsor/CA folio verification |
| corpus-leonardianum | **INFRASTRUCTURE COMPLETE** | No independent DOI needed |
| figura-ultima | **INTERNAL READY — ADVERSARIAL REVIEW REQUIRED** | Mandatory specialist adversarial review; full prose language audit |
| turin-shroud-white-paper | **NOT READY — REBUILD REQUIRED** | Write controlled-hypothesis paper from selected Figura Ultima sections |

---

## Allowed Final Statuses

| Status | Meaning |
|---|---|
| NOT READY | Significant structural or evidential deficiencies remain |
| INTERNAL READY | Suitable for private sharing and self-review only |
| PEER REVIEW READY | Suitable for restricted specialist review; not for public distribution |
| PUBLICATION CANDIDATE | All flags resolved; peer review underway or completed |
| PUBLIC RELEASE APPROVED | Specialist review completed; unresolved flags addressed; permissions confirmed |

**Current corpus status:** PEER REVIEW READY (mechanica, solarscorch) / INTERNAL READY (principia, figura-ultima)

**Do not authorize PUBLIC RELEASE APPROVED until:**
- Specialist review completed
- All PENDING_VERIFICATION flags resolved
- Figure permissions confirmed (Vitruvian Man, Windsor, STURP)
- Full prose language audit completed for Figura Ultima
- Reviewer responses integrated
- Checksum manifests generated

---

*© 2026 Richard Steven Vallance. All intellectual property reserved.*
*Da Valenca Leonardo Project, United Kingdom.*
