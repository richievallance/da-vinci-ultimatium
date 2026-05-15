# Digital Scholarship Infrastructure
## DA_VALENCA_CORPUS_v1.0 — Semantic Graph and Archive Architecture

**Richard Steven Vallance (Da Valenca)** | Da Valenca Leonardo Project
© 2026 Richard Steven Vallance — All Intellectual Property Reserved

---

## Architecture Overview

The Da Valenca corpus is designed to function as a navigable scholarly architecture, not merely a document collection. This file specifies the planned digital infrastructure.

---

## Semantic Graph Schema

Each node in the graph represents one of the following types:

| Node Type | Examples |
|---|---|
| TERM | sensale, vite perpetua, maesstra, bochalari, Conceptione |
| SOURCE | BNE 5907, Windsor RL 19074r, Reti 1974 footnote 1127 |
| MANUSCRIPT | Madrid Codex I, Madrid Codex II, Codex Atlanticus |
| FOLIO | f.0r, f.183v, f.141v |
| FIGURE | Undulating wheel f.0v, Ball bearing f.0r, Flintlock BNE 5907 |
| CLAIM | PC-1 Flintlock, PC-2 Resonant Impulse, PC-3 Clock-Orrery |
| METHOD | Three-layer reading model, Seepage registration, BNE transcript analysis |
| EVIDENCE_TIER | TYPE_A, TYPE_B, TYPE_C, TYPE_D, TYPE_E |
| CAVEAT | PENDING_VERIFICATION, HOLD_BACK, PROVISIONAL |

### Edge Types

| Edge | Meaning |
|---|---|
| CITED_IN | Term → Source |
| APPEARS_ON | Source → Folio |
| SUPPORTS | Source → Claim |
| DERIVED_FROM | Claim → Method |
| CLASSIFIED_AS | Claim → Evidence_Tier |
| SUBJECT_TO | Claim → Caveat |
| CROSS_REFERENCES | Folio → Folio |

---

## JSON Registry Schema

Priority claims are stored in machine-readable format:

```json
{
  "claim_id": "PC-1",
  "title": "Flintlock Prototype",
  "bne_source": "BNE 5907",
  "folio": "Corresponds to f.~25r region",
  "evidence_tier": "TYPE_A",
  "confidence": "HIGH",
  "precedence_years": 115,
  "reference_date_our": "c.1493-1497",
  "reference_date_prior": "c.1610-1615",
  "prior_attribution": "Marin le Bourgeoys",
  "falsification_pathway": "Earlier complete specification predating c.1493",
  "status": "FORMALLY_ESTABLISHED",
  "caveat": null,
  "repository": "da-vinci-mechanica"
}
```

Full JSON registry to be built as `PRIORITY_CLAIMS_REGISTRY.json` in `da-vinci-ultimatium`.

---

## IIIF Linkage System

For every primary source folio cited, the following IIIF data is to be documented:

| Field | Example |
|---|---|
| Repository | Biblioteca Nacional de España |
| Collection | Madrid Codex I (Ms. 8937) |
| BNE viewer URL | https://leonardo.bne.es |
| BNE image number | 5907 |
| IIIF manifest | PENDING — BNE IIIF manifest URL |
| Folio reference | f.~25r (BNE numbering inverse) |

Full IIIF linkage document: `IIIF_LINKAGE_REGISTER.md` — to be built.

---

## Zotero Export Strategy

The `MASTER_BIBLIOGRAPHY.md` is formatted in Chicago N&B and will be converted to:
- Zotero RDF export
- BibTeX (`.bib` file)
- CSL-JSON

These formats enable citation managers to import the full bibliography.

**Action item:** Build `bibliography.bib` from `MASTER_BIBLIOGRAPHY.md` entries.

---

## ORCID Strategy

**RSV ORCID:** To be registered at orcid.org if not already held.

All deposited documents should include RSV's ORCID identifier in metadata once registered.

---

## DOI Planning Layer

See `DOI_REGISTRY.md` for current readiness status.

DOI strategy:
- Zenodo for preprint / data deposits
- Target communities: Leonardo da Vinci Studies; History of Technology; Digital Humanities
- Versioned DOIs: each major version (v1.0, v1.1, v2.0) gets its own DOI
- Dataset DOIs: CSV and KML files in `solarscorch` to be deposited separately as a dataset

---

## Semantic Search Architecture

**Target:** The corpus should be searchable by:
- Folio reference (e.g., "f.183v" returns all claims and analysis from that folio)
- BNE image number (e.g., "5907" returns PC-1 and all related material)
- Claim ID (e.g., "PC-3" returns all supporting material)
- Evidence tier (e.g., "TYPE_D" returns all speculative claims)
- Term (e.g., "sensale" returns all occurrences across the corpus)

**Implementation path:** GitHub search currently provides keyword search. Full semantic search requires a dedicated index — to be built in a future phase using the JSON registry as the data source.

---

*© 2026 Richard Steven Vallance. All intellectual property reserved.*
