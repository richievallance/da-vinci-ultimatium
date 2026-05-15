# DA_VALENCA_CORPUS_v1.0 — Freeze Governance Declaration
## Corpus Leonardianum Universale — Version Control Framework

**Richard Steven Vallance (Da Valenca)** | Da Valenca Leonardo Project | United Kingdom
© 2026 Richard Steven Vallance — All Intellectual Property Reserved

---

## CORPUS FREEZE STATUS

**Corpus designation:** DA_VALENCA_CORPUS_v1.0
**Freeze declared:** May 2026
**Freeze scope:** All manuscripts, white papers, datasets, theses, and infrastructure files in the da-vinci-ultimatium ecosystem

---

## Frozen Content Inventory

| Repository | Document | Frozen Version | Freeze Date |
|---|---|---|---|
| da-vinci-mechanica | DaValenca_Mechanica_WhitePaper_2026.md | v1.0 | May 2026 |
| da-vinci-mechanica | Da_Vinci_Mechanica_Extension_Chapters_VIII_IX_X_RSV_2026.md | v1.0 | May 2026 |
| principia-mechanica | PRINCIPIA_OMNIUM_Da_Valenca_2026.docx | v1.0 | May 2026 |
| solarscorch | SolarScorch_SpectralAnalysis_RSV_2026.docx | v1.0 | May 2026 |
| figura-ultima | FIGURA_ULTIMA_Full_Thesis_RSV_2026.docx | v1.0 | May 2026 |
| figura-ultima | FIGURA_ULTIMA_Thesis_RSV_2026.docx | v1.0 | May 2026 |
| corpus-leonardianum | CorpusLeonardianum_MadridII_WhitePaper_RSV_2026.docx | v1.0 | May 2026 |
| corpus-leonardianum | All infrastructure and transcription files | v1.0 | May 2026 |

---

## Permitted Post-Freeze Changes

Only the following categories of change are permitted to frozen files:

1. **Citation corrections** — correcting erroneous shelfmarks, folio references, or author names
2. **Bibliography additions** — adding newly identified relevant secondary literature
3. **Figure normalisation** — standardising caption format, resolution metadata, permission status
4. **Appendix harmonisation** — aligning appendix format across volumes
5. **Reviewer-response integration** — incorporating specialist reviewer corrections
6. **Errata tracking** — logging confirmed errors without silent overwriting
7. **Formatting stabilisation** — resolving typographic or structural inconsistencies
8. **Verification auditing** — updating PENDING_VERIFICATION flags as sources are confirmed

---

## Prohibited Actions

The following are explicitly prohibited against v1.0 frozen files:

- Silent overwriting of any frozen document
- Uncontrolled manuscript expansion beyond the current scope
- Addition of new substantive claims without version bump
- Removal of existing caveats or evidential tier designations
- Alteration of Priority Claims wording without new version declaration

---

## Version Control Protocol

All changes post-freeze must follow this protocol:

| Change Type | Version Designation | Trigger |
|---|---|---|
| Citation / formatting corrections | v1.1 | ≥1 verified correction |
| Reviewer-response integration | v1.2 | Post specialist review |
| Substantive new content or claims | v2.0 | New scholarship or Priority Claim |
| New primary source incorporation | v2.0 | BNE batch uploads beyond Batch 5 |

### Version Declaration Format

Every version bump requires:

1. A git commit message of the form: `FREEZE_BUMP v1.x → v1.y: [reason]`
2. An entry in this document's Version History table (below)
3. No overwriting — the prior version commit must remain accessible in git history
4. A corresponding entry in `ERRATA_AND_CORRECTIONS.md` (to be created at v1.1)

---

## Version History

| Version | Date | Scope | Author |
|---|---|---|---|
| v1.0 | May 2026 | Initial corpus freeze — Batches 1–5 complete, 6 Priority Claims established | RSV |

---

## Scope Boundaries

The v1.0 freeze covers:

**IN SCOPE (frozen):**
- Madrid Codex I: f.0r–f.25r (Batches 1–5, ~26% of 192-folio codex)
- Six formally established Priority Claims (PC-1 through PC-6)
- Principia Omnium Universale (complete)
- Figura Ultima full and short thesis (complete)
- CA673 SolarScorch analysis and datasets
- All corpus infrastructure and transcription files

**NOT YET IN SCOPE (pending Batch 6+):**
- Madrid Codex I f.25v onward (friction laws, lubrication, rack-and-pinion)
- BNE files 5916–5953 (38 folios held locally)
- PC-7, PC-8, PC-9 (identified, formal write-up pending)
- Codex Atlanticus cross-reference integration
- German translation (RWTH Aachen) systematic integration

---

## Freeze Integrity Verification

To verify freeze integrity, run a SHA-256 checksum against each frozen file and compare against the `CHECKSUM_MANIFEST.md` (to be generated at publication candidate stage). Any deviation from the registered checksum constitutes a freeze violation and must be documented as an errata entry.

---

*© 2026 Richard Steven Vallance. All intellectual property reserved.*
*Da Valenca Leonardo Project, United Kingdom.*
