# Full Repository Audit
## Da Valenca Archive — May 2026

**Auditor:** Claude (Anthropic) on commission from Richard Steven Vallance  
**Date:** May 2026  
**Source of truth:** Live GitHub API scan  
**Token owner:** richievallance

---

## Audit Summary

| Metric | Count |
|---|---|
| Total repositories | 19 |
| Public | 17 |
| Private | 2 |
| Repositories with substantial content | 7 |
| Stub repositories (README only) | 9 |
| Empty repositories | 2 (both private) |
| Total files across all repos | ~195 |
| Total content | ~4.5MB |

---

## Repository-by-Repository Findings

### da-vinci-ultimatium
- **Role:** Master governance parent for Ecosystem A
- **Content:** 62 files, ~499KB. Governance docs, bibliography, navigation, Book I Turin Shroud chapters (26 files in deep directory), priority claims, DOI registry, publication sequence
- **Issues found:** Duplicate governance files (same content in both `evidence/` and `governance/` directories); Book I chapter files have no `.md` extension on ~20 files (renders as plain files not markdown)
- **README quality:** Functional, now updated
- **DOI readiness:** N/A — governance hub
- **Risk:** LOW
- **Status:** 🟢 ACTIVE

### da-vinci-mechanica
- **Role:** Core engineering white paper
- **Content:** 12 files, ~122KB. White paper (72KB MD), extension chapters, CITATION.cff, zenodo.json
- **Issues found:** No .docx binary (MD only); README was underdeveloped (now fixed)
- **README quality:** ✓ Upgraded this session
- **DOI readiness:** CANDIDATE 1 — pending explicit instruction
- **Risk:** LOW
- **Status:** 🟡 PRE-RELEASE

### principia-mechanica
- **Role:** Universal architecture thesis — Madrid Codex II
- **Content:** 3 files, ~3008KB. Full canonical .docx (~3MB), README, canonical note
- **Issues found:** Very lean repo (only 3 files); but canonical file is present and substantial
- **README quality:** ✓ Upgraded this session
- **DOI readiness:** CANDIDATE 3 — pending citation audit
- **Risk:** LOW
- **Status:** 🟡 PRE-RELEASE

### corpus-leonardianum
- **Role:** Codicological infrastructure
- **Content:** 10 files, ~237KB. Madrid II paper, folio archive, transcriptions, BNE matrix, indices
- **Issues found:** None significant
- **README quality:** ✓ Upgraded this session
- **DOI readiness:** Infrastructure — no independent DOI currently required
- **Risk:** LOW
- **Status:** 🟢 ACTIVE

### solarscorch
- **Role:** Solar geometry and spectral analysis
- **Content:** 8 files, ~29KB. Spectral paper .docx, KML files, CSV data
- **Issues found:** 156.4° bearing anomaly documented but unresolved — now flagged in README
- **README quality:** ✓ Upgraded this session
- **DOI readiness:** CANDIDATE 2 — pending anomaly documentation
- **Risk:** LOW
- **Status:** 🟡 PRE-RELEASE

### figura-ultima
- **Role:** Turin Shroud authorship thesis
- **Content:** 25 files, ~364KB. Full thesis (183KB), short thesis (104KB), Mechanisms A–Y
- **Issues found:** `Mechanism W` has a duplicate filename entry (one with .md, one without — the no-.md version is 2994 bytes, the .md version is 0 bytes). Zero-byte file is effectively empty.
- **README quality:** ✓ Upgraded this session with locked evidence tiers
- **DOI readiness:** HOLD — pending adversarial review
- **Risk:** LOW (content) / MEDIUM (premature release risk)
- **Status:** 🔴 EXPERIMENTAL

### turin-shroud-white-paper
- **Role:** Predecessor archive
- **Content:** 24 files, ~95KB. 19 Mechanism files (duplicates of figura-ultima), 2 partial chapter fragments, broken filename (`B — HISTORICAL PROBLEM STATEM.mdENT` — has `.mdENT` extension, not `.md`)
- **Issues found:** All Mechanism files are byte-identical duplicates of figura-ultima. Broken filename. Was presenting as a real paper.
- **README quality:** ✓ Archive notice added this session
- **DOI readiness:** NONE — archived
- **Risk:** MEDIUM — was publicly misrepresenting itself as a current paper (now fixed)
- **Status:** 🔴 ARCHIVED — predecessor

### rumour-harm
- **Role:** Sociology white paper
- **Content:** 7 files, ~7KB. Metadata scaffolding only — NO white paper body
- **Issues found:** README previously claimed "Full white paper (Markdown edition) — present" — FALSE. Paper does not exist in repo. README claimed "Publication Ready" — FALSE. GitHub repo description said "Da Valenca Mechanica" — WRONG. All three now fixed.
- **README quality:** ✓ Fixed this session — false claims removed, paper-pending notice added
- **DOI readiness:** NONE — paper not uploaded
- **Risk:** LOW (after fixes)
- **Status:** 🟡 PENDING PAPER UPLOAD

### soyga-universe
- **Role:** Symbolic cosmology research
- **Content:** 35 files, ~177KB. Full 21-chapter manuscript
- **Issues found:** Public repo with speculative content; previous session audit flagged as "hold private". README lacked speculative notice.
- **README quality:** ✓ Speculative notice added this session
- **DOI readiness:** NONE — speculative/experimental
- **Risk:** LOW-MEDIUM (speculative claims in public)
- **Status:** 🟡 EXPERIMENTAL — public with caveats

### Stub repositories (README only, ~0KB content)
universal-simulation-construct, usc-foundations, recursive-consciousness, informational-light, simulation-construct-papers, contagion-studies, richard-vallance-archive, autobiographical-papers

**All stubs.** No content to audit. No risk. No DOI relevance.

### Private repositories
- **da-valenca-internal:** Empty. Created but never populated.
- **valhalla-archive:** Empty. ABSOLUTE PRIVATE — no content, no action needed.

---

## Issues Resolved This Session

| Issue | Repository | Action |
|---|---|---|
| README too short / underdeveloped | da-vinci-mechanica | ✓ Full upgrade committed |
| Missing anomaly documentation | solarscorch | ✓ 156.4° flag added to README |
| No .docx binary | da-vinci-mechanica | ⏳ Flagged — user action required |
| Missing constitutional note | principia-mechanica | ✓ README upgraded |
| README underdeveloped | corpus-leonardianum | ✓ Full upgrade committed |
| README underdeveloped + evidence tiers missing | figura-ultima | ✓ Full upgrade with locked tiers |
| No archive notice — presenting as current paper | turin-shroud-white-paper | ✓ Archive notice committed |
| False "paper present" and "publication ready" claims | rumour-harm | ✓ Fixed — paper-pending notice added |
| Wrong GitHub description | rumour-harm | ✓ Description corrected via API |
| No speculative notice on public manuscript | soyga-universe | ✓ Notice added |
| Priority claims register missing | da-vinci-ultimatium | ✓ DA_VALENCA_PRIORITY_CLAIMS.md committed |
| Repository map stale | da-vinci-ultimatium | ✓ Updated with live ecosystem reality |
| Duplicate Mechanism files undocumented | turin-shroud-white-paper | ✓ LEGACY_ARCHIVE/DUPLICATE_RESOLUTION_LOG.md added |
| Cover art missing from repos | All core repos | ✓ cover/ directories added to 5 repos |

---

## Outstanding Issues (Require User Action)

| Issue | Repository | Action Required |
|---|---|---|
| .docx binary missing | da-vinci-mechanica | Upload via GitHub web or git push |
| White paper body missing | rumour-harm | Upload paper text |
| ~20 files lack .md extension | da-vinci-ultimatium/Book I | Rename files to add .md extension |
| Duplicate governance files | da-vinci-ultimatium | evidence/ and governance/ dirs contain same files — consolidate |
| Zero-byte Mechanism W.md | figura-ultima | Delete empty duplicate or populate |
| Broken filename (.mdENT) | turin-shroud-white-paper | Rename B file to correct .md extension |
| soyga-universe visibility | soyga-universe | Consider making private if speculative content concern |
| autobiographical-papers PUBLIC | autobiographical-papers | Consider making private — stub now but will attract attention when populated |
