# CROSS_VOLUME_DEPENDENCY_MAP.md
## Cross-Document Dependency and Citation Map — Da Valenca Corpus

**Richard Steven Vallance (Da Valenca)** | Corpus Leonardianum Universale
© 2026 Richard Steven Vallance — All Intellectual Property Reserved

---

## Dependency Logic

An arrow A → B means: document A is required reading before or during document B.
A dashed arrow A ⇢ B means: document A provides useful context for B but is not strictly required.

---

## Primary Dependency Graph

```
TIER 1: FOUNDATION DOCUMENTS
├── DaValenca_Mechanica_WhitePaper_2026.md [PUB-01]
│   ├── DEPENDS ON: BNE Interactivo transcripts (external primary source)
│   ├── DEPENDS ON: Reti 1974 editorial apparatus
│   ├── ENABLES: Principia Omnium (Chapter VII cross-reference)
│   ├── ENABLES: Figura Ultima (Chapter 8.6, Appendix B)
│   └── ENABLES: Ch VIII-IX-X Extension [PUB-02]
│
├── Da_Vinci_Mechanica_Extension_Chapters_VIII_IX_X [PUB-02]
│   ├── DEPENDS ON: PUB-01 (Chapters I-VIII must be read first)
│   ├── DEPENDS ON: Windsor Collection anatomical folios (for Ch IX)
│   └── ENABLES: Chapter X ten-output-configuration model
│
├── PRINCIPIA_OMNIUM_Da_Valenca_2026.docx [PUB-03]
│   ├── DEPENDS ON: BNE Madrid II transcripts
│   ├── DEPENDS ON: Reti Vol. V footnote apparatus
│   ├── CITES: PUB-01 (Madrid I as mechanical spine — Ch VII)
│   └── REFERENCES: Yates, Art of Memory; Pacioli, Divina Proportione
│
└── SolarScorch [PUB-04]
    ├── DEPENDS ON: CA673 (Codex Atlanticus f.673r)
    ├── DEPENDS ON: Solar geometry calculations
    └── INDEPENDENT OF: Principia and Mechanica (standalone paper)

TIER 2: EXPERIMENTAL DOCUMENTS
├── FIGURA_ULTIMA_Full_Thesis [PUB-05]
│   ├── DEPENDS ON: PUB-01 (Appendix B mechanica cross-reference)
│   ├── DEPENDS ON: STURP 1981; Heller & Adler 1980; Rogers 2005
│   ├── CITES: Vitruvian Man proportions (bridges to PUB-01/03)
│   └── INDEPENDENT OF: SolarScorch
│
└── FIGURA_ULTIMA_Short_Thesis [PUB-06]
    ├── CONDENSED VERSION OF: PUB-05
    └── DEPENDS ON: PUB-05 for full footnotes and evidence
```

---

## Priority Claims Cross-Document Dependencies

| Priority Claim | Primary Document | Supporting Document | Independent Verification |
|---|---|---|---|
| PC-1: Flintlock | PUB-01 §6.2 | BNE 5907 transcript | Reti 1974 Vol. II (absence of identification) |
| PC-2: Resonant Impulse | PUB-01 §2.3 | BNE 5911 transcript | No known contemporary parallel documented |
| PC-3: Clock-Orrery | PUB-01 §3.2, §6.1, §6.5 | BNE 5890, 5902, 5906 | Gear ratio arithmetic (externally verifiable) |
| PC-4: Chiaravalle | PUB-01 §4.3 | BNE 5892 transcript | Abbey physical record (still standing) |
| PC-5: Seepage Method | PUB-01 §1.2 | INF-05 (continuity analysis) | No precedent in literature |
| PC-6: Toggle-Lock | PUB-01 §4.6 | BNE 5955 transcript | Engineering literature (250+ years later) |

---

## Key Internal Cross-References

The following cross-references are cited explicitly within the corpus text:

| Source Folio / Section | Citation | Cited In |
|---|---|---|
| BNE 5908 | 'nella 20ª del secondo' (Book II, Prop. 20) | PUB-01 Appendix A |
| BNE f.4v (Maesstra) | 'nel 5° del 9°' (Book IX, Prop. 5) | PUB-01 Appendix A |
| BNE f.43r | 'per la 60ª del 7°' (Book VII, Prop. 60) | PUB-01 §10.5 |
| Principia §7 | 'Madrid I as mechanical spine' | PUB-03 Ch. VII |
| Figura Ultima §8.6 | 'Archimedes mirror flash — optical production method' | PUB-05 Ch. 8 |
| Principia Claim Register | PC-012 'Cloth Image Convergence (Experimental)' | Bridge to PUB-05 |

---

*© 2026 Richard Steven Vallance. All intellectual property reserved.*
