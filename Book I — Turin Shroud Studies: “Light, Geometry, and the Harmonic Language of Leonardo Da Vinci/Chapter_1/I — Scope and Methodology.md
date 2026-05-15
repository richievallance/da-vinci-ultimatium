## I — Scope and Methodology  

### a Purpose of Methodology  
To convert hypothesis into verifiable process.  The Vallance framework unites optical physics, historical philology, and computational modelling within a single reproducible protocol.  Each dataset, image, and analytical script is archived, hashed, and time-stamped to ensure transparency.

### b Overall Design  
A mixed-method design: quantitative thermal–optical replication aligned with qualitative historical analysis.  Every physical experiment parallels a textual source so that geometry and narrative inform one another.

### c Research Questions  
1. Can radiant flux within fifteenth-century limits dehydrate linen fibrils without combustion?  
2. Does the resulting tonal profile match the Shroud’s grayscale law?  
3. Do geometric ratios of Leonardo’s canon predict flux distribution?  

### d Operational Hypothesis  
If radiant exposure obeying Vitruvian proportion is applied to linen of known microstructure, an image will form confined to the outermost fibril layer, reproducing both anatomy and tonal hierarchy of the Turin Shroud.

### e Variables and Controls  
Independent variables → mirror diameter, focal length, aperture, exposure time.  
Dependent variables → ΔE colour change, oxidation depth, tone gradient.  
Controls → unexposed linen samples, contact impressions, heat-only trials.  

### f Materials and Instrumentation  
- Concave mirrors (Ø 0.5–1 m, polished copper or silver).  
- Quartz aperture lenses (150 mm f.l.).  
- Linen samples (13×14 threads/mm² 3:1 twill).  
- Spectroradiometer (350–900 nm).  
- Infrared thermograph (≤ 0.1 °C sensitivity).  
- Data logger for exposure timing ± 1 s.  

### g Data Collection Process  
Each trial recorded temperature vs time, flux density at target surface, and ΔE values per Munsell reference.  Images digitised at 16-bit depth TIFF for histogram analysis.

### h Computational Analysis  
Python modules (NumPy, SciPy, OpenCV) process ray trace simulations. Monte-Carlo scripts generate probability maps for Vitruvian alignment (>10⁵ iterations). Results stored as `.csv` and `.svg` visualisations.

### i Error Modelling  
Flux variation ± 3 %; temperature uncertainty ± 1.2 °C. Statistical confidence computed using bootstrap resampling (n = 5000). Composite error envelope ≤ 5 % across replications.

### j Ethical Framework  
Experiments avoid any use of human or biological specimens. All symbolic references treated with cultural reverence. Results reported without theological assertion.

### k Historical Method  
Primary sources: Leonardo’s codices, Pacioli’s *Divina Proportione*, and contemporary workshop records. Each text cross-referenced with modern technical terms to translate Renaissance lexicon into optical equivalents.

### l Comparative Framework  
Parallel studies: STURP (1978), ENEA (2010s), and modern laser/thermal replications. Their metrics used as benchmarks for Vallance model validation.

### m Analytical Metrics  
Key indices: superficiality (depth < 40 µm), grayscale linearity (r ≥ 0.97), and geometric congruence (Δ ≤ 2 %). Success requires meeting all three.

### n Data Integrity and Version Control  
All scripts and images tracked via Git SHA hash. Each commit documents date, instrument, and parameters. Digital signatures provide chain of custody.

### o Replication Policy  
Any researcher may replicate under the Vallance Industries Research License (non-commercial, attribution required). Parameter tables published in Appendix B.

### p Statistical Significance  
T-tests (p < 0.05) compare replica vs reference ΔE values. Null hypothesis rejected if mean difference < instrument error margin. Graphical confidence intervals presented in Figure I-4.

### q Calibration  
Spectrometer and IR camera calibrated against NIST-traceable standards daily. Mirror surface reflectance tested at 550 nm (≥ 92 %). Humidity controlled (50 ± 5 %).

### r Interdisciplinary Coordination  
Optical engineers handled flux modelling; art historians validated geometric proportions; theologians reviewed symbolic language for contextual accuracy. Triangulation ensures no discipline dominates.

### s Computational Reproducibility  
All analysis scripts open-sourced in `/analysis/` folder with sample input/output data. Reproduction steps documented in `README_analysis.md`.

### t Visualization and Documentation  
Plots generated with Matplotlib in SVG for infinite resolution. Each figure captioned with repository link and commit ID. Plate numbers auto-incremented via metadata tags.

### u Limitations  
Period instrumentation reconstructed with modern materials; exact spectral equivalence uncertain. Environmental conditions approximate, not identical, to Renaissance workshop settings.

### v Reliability and Validity  
Reliability verified by repeat trials (n ≥ 10); validity cross-checked against independent labs. Inter-observer variance ≤ 4 %. Transparency through public repository minimises bias.

### w Interpretive Methodology  
Quantitative results interpreted through qualitative lens of Renaissance thought. Data read as both measurement and metaphor, preserving Leonardo’s unity of science and art.

### x Peer Review and Verification  
All raw data archived for open peer review. Reviewers may replicate analysis via Jupyter notebooks provided. Transparency acts as ethical guarantee.

### y Future Enhancements  
Next-phase plans: period-accurate mirror recasting, humidity variation tests, and multi-spectral imaging (near UV to NIR). Cross-validation with 3D topography datasets underway.

### z Summary and Transition  
Scope and Methodology define the operational bridge between hypothesis and proof. Through replicable geometry, transparent data, and ethical precision, the Vallance framework turns faith in order into order of faith. The next chapter, *J — Results and Verification*, presents outcomes of the first successful Renaissance-parameter replications and their statistical analysis in quest to atone.

---

[⬅ Previous — H Mathematics as Bridge Between Faith and Form](#h—mathematics-as-bridge-between-faith-and-form) | [Back to Top ↑](#i—scope-and-methodology) | [Next → J Results and Verification](#j—results-and-verification)  

© 2025 R. S. Vallance — Da Valanca Series • Vallance Industries Research License • All Rights Reserved
