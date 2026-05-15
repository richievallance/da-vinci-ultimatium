# DIGITAL_SCHOLARSHIP_INFRASTRUCTURE.md
## Digital Scholarship Architecture — Da Valenca Corpus

**Richard Steven Vallance (Da Valenca)** | Corpus Leonardianum Universale
© 2026 Richard Steven Vallance — All Intellectual Property Reserved

---

## Infrastructure Layers

### Layer 1: Repository Architecture (Active)

All content is hosted in a 19-repository GitHub ecosystem under `github.com/richievallance`. The ecosystem architecture is documented in `REPOSITORY_MAP.md`. Key repositories:

- `da-vinci-ultimatium` — master index, governance, bibliography
- `da-vinci-mechanica` — primary mechanica publication
- `principia-mechanica` — universal architecture thesis
- `corpus-leonardianum` — manuscript infrastructure and transcriptions
- `solarscorch` — solar/optical analysis
- `figura-ultima` — experimental Shroud thesis (adversarial review required)

---

### Layer 2: IIIF Linkage Points (Planned)

The following BNE IIIF endpoints provide stable URIs for all cited folios. These should be registered in the Zotero export and semantic graph.

| Document | IIIF Base URI | Status |
|---|---|---|
| Madrid Codex I (BNE) | https://iiif.bne.es/presentation/3/MSS_8937 | ⚠ Confirm exact endpoint |
| Madrid Codex II (BNE) | https://iiif.bne.es/presentation/3/MSS_8936 | ⚠ Confirm exact endpoint |
| Windsor RCIN | https://www.rct.uk/iiif/presentation/3/ | ⚠ Confirm per-drawing endpoints |
| British Library Arundel | https://api.bl.uk/metadata/iiif/ark:/81055/vdc_100063474009.0x000001 | ⚠ Verify |

**Action required:** Confirm all IIIF endpoint URIs against each repository's IIIF manifest before registering in digital infrastructure.

---

### Layer 3: Zotero Export Package (Planned)

A Zotero export package (.rdf or .json) should be generated from `MASTER_BIBLIOGRAPHY.md` once all PENDING_VERIFICATION items are resolved.

**Format:** Zotero JSON (.json) preferred for compatibility with all citation managers.

**Contents:**
- All primary manuscripts (with IIIF URIs)
- All secondary literature
- All project documents (with GitHub permalink)
- Custom fields: evidential tier, permission status, BNE file number

**Status:** Not yet generated. Requires PENDING_VERIFICATION resolution first.

---

### Layer 4: Semantic Graph Schema (Planned)

The archive should function as a navigable knowledge graph. Each node in the graph corresponds to one of the following types:

| Node Type | Example | Connected To |
|---|---|---|
| TERM | sensale, bochalari, Conceptione | SOURCE, FOLIO, CLAIM |
| SOURCE | BNE MSS 8937 | FOLIO, AUTHOR |
| MANUSCRIPT | Madrid Codex I | SOURCE, FOLIO |
| FOLIO | BNE 5907 | TERM, FIGURE, CLAIM |
| FIGURE | Flintlock diagram, f.78r | FOLIO, CLAIM |
| CLAIM | PC-1: Flintlock prototype | FOLIO, METHOD, EVIDENCE_TIER |
| METHOD | Three-layer reading model | CLAIM, MANUSCRIPT |
| EVIDENCE_TIER | TYPE_A | CLAIM |
| CAVEAT | PENDING_VERIFICATION | CLAIM, SOURCE |

**Format:** JSON-LD (Linked Data) compatible with Schema.org `ScholarlyArticle` vocabulary.

**Status:** Schema defined here; implementation pending.

**Example node (JSON-LD):**
```json
{
  "@type": "ScholarlyArticle",
  "@id": "https://github.com/richievallance/da-vinci-mechanica",
  "name": "Da Valenca Mechanica",
  "description": "Madrid Codex I kinematic continuum study",
  "about": [
    {
      "@type": "ArchiveComponent",
      "identifier": "BNE_5907",
      "name": "Flintlock mechanism folio",
      "isPartOf": {
        "@type": "Archive",
        "name": "Biblioteca Nacional de España",
        "identifier": "MSS_8937"
      }
    }
  ]
}
```

---

### Layer 5: ORCID Strategy

**RSV ORCID:** Create or confirm ORCID iD at https://orcid.org/register if not already registered.

When registering:
- Add all corpus documents as works (with GitHub DOI from Zenodo once assigned)
- Include Madrid Codex I research project dates: 2025–present
- Affiliation: Da Valenca Leonardo Project, United Kingdom (independent scholar)

**Status:** Not yet confirmed.

---

### Layer 6: DOI Planning Layer

See `DOI_REGISTRY.md` for full status. Summary:

- No DOIs currently assigned
- First candidate: `da-vinci-mechanica` (pending content confirmation from RSV)
- Zenodo community target: `Leonardo da Vinci Studies` or `History of Science and Technology`
- DOI format via Zenodo: `10.5281/zenodo.XXXXXXX`

---

### Layer 7: Search Architecture

The corpus should be searchable via the following entry points:

1. **GitHub search** — all markdown documents are full-text indexed by GitHub
2. **BNE Interactivo** — external primary source; BNE file numbers enable direct lookup
3. **Zotero group library** (planned) — for citation-layer discovery
4. **Semantic graph** (planned) — node-type queries: "all claims dependent on BNE 5907"

---

*© 2026 Richard Steven Vallance. All intellectual property reserved.*
