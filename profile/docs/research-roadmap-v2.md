# K R&D Lab · Research Roadmap v2
## S1 Biomedical — Corrected & Complete (March 2026)

> **Status:** Active document · All critical errors from v1 fixed  
> **Maintained by:** Oksana Kolisnyk · KOSATIKS GROUP  
> **Scientific basis:** Biomni gap analysis, March 2026

---

## Gap Priority Ranking (Biomni, March 2026)

| Rank | Cancer | Gap score | Survival | Cases/yr | Our track |
|------|--------|-----------|----------|----------|-----------|
| #1 | PDAC | 9.4/10 | 12% (5yr) | ~60 000 | S1-R13 (planned) |
| #2 | SCLC | 8.9/10 | 6% (5yr) | ~35 000 | S1-R13 (planned) |
| #3 | DIPG | 8.7/10 | <2% (5yr) | ~300 | **S1-R12b ← active** |
| #4 | UVM (metastatic) | 8.2/10 | 15% (5yr) | ~80 | **S1-R12c ← active** |
| #5 | pAML | 7.9/10 | 30% relapse | ~197 | **S1-R12d ← active** |

> DIPG has highest gap-per-survival ratio: lowest survival × fewest prior computational studies.

---

## v1 → v2 Corrections

| # | Error in v1 | Corrected in v2 |
|---|-------------|-----------------|
| 1 | DIPG classified under S1-A (Genomics only) | Moved to S1-F (Rare) — cross-track: S1-A + S1-D + S1-B |
| 2 | UVM n=80 described as "insufficient" | n=80 is the complete TCGA-UVM cohort — sufficient for pilot |
| 3 | pAML ferroptosis gap listed as "speculative" | Confirmed gap: FerrDb v2 search returns 0 FLT3-ITD entries |
| 4 | S1-R11 (CSF/Vitreous/BM LNP) listed as single project | Split: CSF→S1-R12b, Vitreous→S1-R12c, BM→S1-R12d |
| 5 | Circadian biology not linked to DIPG | BMAL1 suppression confirmed in H3K27M+ DIPG (PMID:34822368) |
| 6 | m6A flagged only for PDAC | METTL3/WTAP upregulation confirmed in GNAQ+ UVM (PMID:35491192) |

---

## S1 Biomedical — Full Project Map

### S1-A · PHYLO-GENOMICS — What breaks in DNA

| Code | Tool | Status | Dataset | Metric |
|------|------|--------|---------|--------|
| S1-R1 | OpenVariant — SNV pathogenicity | ✅ Active | ClinVar 2026 | AUC=0.939 |
| S1-R1b | Somatic mutation classifier | 🔶 In progress | TCGA pan-cancer | — |
| S1-R12a | Rare variant atlas (DIPG·UVM) | 🔴 Planned | PBTA + TCGA-UVM | — |

### S1-B · PHYLO-RNA — How to silence it via RNA

| Code | Tool | Status | Dataset | Metric |
|------|------|--------|---------|--------|
| S1-R2 | miRNA silencing (BRCA1/2·TP53) | ✅ Active | miRBase·GEO | — |
| S1-R3 | siRNA synthetic lethal (LUAD·BRCA·COAD) | ✅ Active | DepMap·TCGA | — |
| S1-R4 | lncRNA-TREM2 ceRNA network | ✅ Active | GEO·GTEx | — |
| S1-R4b | ASO designer | ✅ Active | miRBase | — |

### S1-C · PHYLO-DRUG — Which molecule treats it

| Code | Tool | Status | Dataset | Metric |
|------|------|--------|---------|--------|
| S1-R5 | FGFR3 RNA-directed drug discovery | ✅ Active | ChEMBL | score=0.793 |
| S1-R5b | Synthetic lethal drug mapping | 🔶 In progress | DepMap+ChEMBL | — |
| S1-R13 | m6A × Ferroptosis × Circadian (pan-cancer) ⭐ | 🔴 Frontier | TCGA-PAAD·SCLC | — |

### S1-D · PHYLO-LNP — How to deliver the drug

| Code | Tool | Status | Dataset | Metric |
|------|------|--------|---------|--------|
| S1-R6 | LNP protein corona (serum) | ✅ Active | Internal | AUC=0.791 |
| S1-R7 | Flow corona — Vroman effect | ✅ Active | Internal | — |
| S1-R8 | LNP brain delivery (ApoE·BBB) | ✅ Active | Internal | — |
| S1-R10 | AutoCorona NLP extractor | ✅ Active | PMC abstracts | F1=0.71 |
| S1-R11 | CSF·Vitreous·BM corona ⭐ | 🔴 0 prior studies | — | — |

### S1-E · PHYLO-BIOMARKERS — Detect without biopsy

| Code | Tool | Status | Dataset | Metric |
|------|------|--------|---------|--------|
| S1-R9 | Liquid biopsy classifier | ✅ Active | Tissue proxy | AUC=0.992* |
| S1-R9b | Protein panel validator | 🔶 In progress | GEO plasma | — |
| S1-R9c | ctDNA gap analysis | 🔴 Planned | TCGA ctDNA | — |

> *AUC=0.992 on tissue proteomics proxy. Plasma validation pending (S1-R9b).

### S1-F · PHYLO-RARE — Where almost nobody has looked yet

| Code | Toolkit | Key Gap | Data | Status |
|------|---------|---------|------|--------|
| S1-R12b | DIPG | H3K27M + CSF LNP + circadian | PBTA·GSE126319 | 🔶 In development |
| S1-R12c | UVM | GNAQ/GNA11 + vitreous corona + m6A | TCGA-UVM (n=80) | 🔶 In development |
| S1-R12d | pAML | FLT3-ITD + BM niche corona + ferroptosis | TARGET-AML (~197) | 🔶 In development |

---

## Timeline

```
Q1 2026 (now)   S1-R1 ✅ · S1-R2–R4 ✅ · S1-R5 ✅ · S1-R6–R10 ✅ · S1-R9 ✅
Q2 2026         S1-R12b pilot · S1-R12c pilot · S1-R9b validation
Q3 2026         S1-R12d pilot · S1-R13 design · S1-R11 first corona data
Q4 2026         S1-R1b · S1-R5b · full PHYLO-RARE v1 publication
```

---

## Links

- **Hub:** [github.com/K-RnD-Lab](https://github.com/K-RnD-Lab)
- **HuggingFace Space:** [huggingface.co/spaces/K-RnD-Lab/PHYLO-CORE_03-2026](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-CORE_03-2026)
- **KOSATIKS GROUP:** [kosatiks-group.pp.ua](https://kosatiks-group.pp.ua)

---
*Research only. Not clinical advice. MIT License.*
