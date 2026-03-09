<div align="center">

# 🧬 K R&D Lab

**Open-Source Research Infrastructure by [Oksana Kolisnyk](https://kosatiks-group.pp.ua)**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HuggingFace](https://img.shields.io/badge/🤗_HuggingFace-K--RnD--Lab-orange)](https://huggingface.co/K-RnD-Lab)
[![GitHub Org](https://img.shields.io/badge/GitHub-K--RnD--Lab-181717?logo=github)](https://github.com/K-RnD-Lab)

*Computational biology · Biomarker discovery · Plant science · Data analytics · Open science*

> ⚠️ All models are hypothesis-generating. Results labeled SIMULATED require experimental validation before any clinical or agricultural application.

</div>

---

## 🗺️ Research Ecosystem

K R&D Lab is organized into three independent series.
Each series has its own scope, methods, and target audience.

| Series | Domain | First repo | Status |
|--------|--------|------------|--------|
| 🧬 **PHYLO** | Computational oncology & RNA therapeutics | PHYLO-DEMO | 🟢 Active |
| 🌿 **BIO** | Systems biology · Plant science · Biochemistry | BIO-PLANT | 🟡 In development |
| 📊 **ANALYTICS** | Health data · Behavioral & marketing analytics | ANALYTICS-HEALTH | 🔵 Planned |

---

## 🧬 PHYLO Series — Computational Oncology

> *Investigating cancer biology through computational lenses:
> genomics, RNA therapeutics, nanoparticle delivery, biomarkers, and rare cancers.*

PHYLO is a branded series — not a standard phylogenetics term.
Each sub-project is an independent, reproducible research module with
its own dataset, methods, and interactive Gradio demo on HuggingFace.

### 🚪 Entry Point

| Space | Description | Link |
|-------|-------------|------|
| **PHYLO-DEMO** | All 10 tools · Beginner-friendly · Learning Sandbox | [![HF](https://img.shields.io/badge/🤗-PHYLO--DEMO-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-DEMO) |

---

### 📁 PHYLO Sub-Projects

#### 🔷 A — Genomics & Variants
> *"What breaks in DNA — and how pathogenic is it?"*

| Repo | Tool | Key Finding | Status |
|------|------|-------------|--------|
| [PHYLO-GENOMICS](https://github.com/K-RnD-Lab/PHYLO-GENOMICS) | OpenVariant v2 | AUC=0.939 on ClinVar 2026 | ✅ Active |
| | Somatic mutation classifier | BRCA1/2, TP53, EGFR, ALK panels | 🔶 In progress |
| | Rare variant explorer | DIPG H3K27M · UVM GNAQ/GNA11 | 🔴 Planned |

**Research question:** Which single-nucleotide variants are pathogenic, and why does position matter less than amino acid identity?

---

#### 🔷 B — RNA Therapeutics
> *"How to silence what's broken — through RNA"*

| Repo | Tool | Key Finding | Status |
|------|------|-------------|--------|
| [PHYLO-RNA](https://github.com/K-RnD-Lab/PHYLO-RNA) | miRNA predictor | hsa-miR-148a-3p top silenced in BRCA2-mut | ✅ Active |
| | siRNA synthetic lethal | SPC24, BUB1B, CDC45 — novel targets in LUAD | ✅ Active |
| | lncRNA-TREM2 network | CYTOR→miR-138-5p→AKT1 in neuroinflammation | ✅ Active |
| | ASO designer | GAS5, CYTOR — HIGH priority candidates | ✅ Active |

**Research question:** Which RNA molecules can selectively silence cancer-driving genes without existing drug alternatives?

---

#### 🔷 C — Drug Discovery
> *"Which small molecule fits the RNA target?"*

| Repo | Tool | Key Finding | Status |
|------|------|-------------|--------|
| [PHYLO-DRUG](https://github.com/K-RnD-Lab/PHYLO-DRUG) | FGFR3 RNA-directed compounds | CHEMBL1575701 — score 0.793, near-zero toxicity | ✅ Active |
| | Synthetic lethal drug mapping | PLK1, CDK1 — clinical-stage compounds | 🔶 In progress |
| | m6A × Ferroptosis × Circadian ⭐ | Cross-cancer triad — never studied as system | 🔴 Frontier |

**Research question:** Can we identify small molecules that target RNA structures directly, bypassing protein-level resistance?

---

#### 🔷 D — Nanoparticle Delivery & LNP Corona
> *"How does the drug reach the tumor — and what changes along the way?"*

| Repo | Tool | Key Finding | Status |
|------|------|-------------|--------|
| [PHYLO-LNP](https://github.com/K-RnD-Lab/PHYLO-LNP) | Corona predictor (serum) | CHL/HL/PEG ratios dominate efficacy (AUC=0.791) | ✅ Active |
| | Flow Corona — Vroman effect | Blood flow accelerates albumin→ApoE exchange 3–4× | ✅ Active |
| | BBB / ApoE predictor | pKa 6.2–6.8 + zeta ±5 mV → ApoE >20% | ✅ Active |
| | AutoCorona NLP | F1=0.71 extracting corona data from PMC abstracts | ✅ Active |
| | **CSF / Vitreous / Bone Marrow** ⭐ | Corona in non-serum biofluids — 0 published studies | 🔴 Frontier |

**Research question:** How does LNP protein corona differ in CSF (DIPG), vitreous humor (UVM), and bone marrow niches (pAML) vs. standard serum?

---

#### 🔷 E — Biomarkers & Diagnostics
> *"How to detect cancer without tissue biopsy?"*

| Repo | Tool | Key Finding | Status |
|------|------|-------------|--------|
| [PHYLO-BIOMARKERS](https://github.com/K-RnD-Lab/PHYLO-BIOMARKERS) | Liquid Biopsy classifier | CTHRC1+FHL2+LDHA panel — AUC=0.992* | ✅ Active |
| | Protein panel validator | Weight-based logistic model | 🔶 In progress |
| | ctDNA gap analysis | Zero validated panels in 7/10 rare cancers | 🔴 Planned |

*\*AUC reflects tissue proteomics proxy — plasma validation pending.*

**Research question:** Which protein combinations can distinguish cancer from healthy in a blood test — without expensive sequencing?

---

#### 🔷 F — Rare Cancers (Frontier)
> *"Where almost nobody has looked yet"*

| Repo | Tool | Key Gap | Status |
|------|------|---------|--------|
| [PHYLO-RARE](https://github.com/K-RnD-Lab/PHYLO-RARE) | DIPG toolkit | H3K27M variants + CSF LNP delivery | 🔴 In development |
| | UVM toolkit | GNAQ/GNA11 + vitreous corona | 🔴 In development |
| | pAML toolkit | FLT3-ITD + bone marrow niche corona | 🔴 In development |

**Research question:** Can computational methods generate testable hypotheses for cancers with <300 cases/year and 1% 5-year survival?

**Scientific basis:** Biomni gap analysis (March 2026) — PDAC, SCLC, DIPG identified as highest-priority underserved cancers.
Full roadmap: [`docs/research-roadmap-v2.md`](docs/research-roadmap-v2.md)

---

## 🌿 BIO Series — Systems Biology & Life Sciences

> *Broader biomedical and life sciences research beyond oncology —
> from plant biochemistry to soil microbiomes to neurodegeneration.*

### 📁 BIO Sub-Projects

#### 🌱 Plant Science & Phytochemistry
> *"What bioactive compounds do plants produce — and what can we do with them?"*

| Repo | Focus | Data sources | Status |
|------|-------|--------------|--------|
| [BIO-PLANT](https://github.com/K-RnD-Lab/BIO-PLANT) | Phytochemical profiling · Bioactivity prediction | UNPD, KNApSAcK, Phytozome | 🟡 In development |

**Research question:** Which plant-derived compounds have predicted bioactivity against cancer or microbial targets — verifiable from public databases?

---

#### 🌾 Agricultural Biology & Biofertilizers
> *"How do soil microbiomes support plant growth — and how can we engineer them?"*

| Repo | Focus | Data sources | Status |
|------|-------|--------------|--------|
| [BIO-AGRO](https://github.com/K-RnD-Lab/BIO-AGRO) | Biofertilizer efficacy · Rhizosphere microbiome | EBI MGnify, NCBI SRA | 🟡 In development |

**Research question:** Which microbial combinations in rhizosphere consistently improve crop yield — and what metabolic pathways explain the effect?

---

#### ⚗️ Biochemistry & Metabolomics
> *"What metabolic signatures distinguish healthy from diseased states?"*

| Repo | Focus | Data sources | Status |
|------|-------|--------------|--------|
| [BIO-BIOCHEM](https://github.com/K-RnD-Lab/BIO-BIOCHEM) | Metabolite profiling · Pathway analysis | HMDB, MetaboLights, Reactome | 🔴 Planned |

---

#### 🧠 Neurodegeneration
> *"What computational patterns predict Alzheimer's and Parkinson's progression?"*

| Repo | Focus | Status |
|------|-------|--------|
| [BIO-NEURO](https://github.com/K-RnD-Lab/BIO-NEURO) | lncRNA networks · neuroinflammation · TREM2 axis | 🔴 Planned |

---

#### 🛡️ Immunology & Aging *(future)*

```
BIO-IMMUNO   ← immune evasion mechanisms · checkpoint biology
BIO-AGING    ← longevity biomarkers · epigenetic clocks
```

*Target: Q3–Q4 2026*

---

## 📊 ANALYTICS Series — Data Science & Applied Analytics

> *Evidence-based analytics across health, behavior, and open data.*

| Repo | Focus | Status |
|------|-------|--------|
| [ANALYTICS-HEALTH](https://github.com/K-RnD-Lab/ANALYTICS-HEALTH) | Population health · epidemiology datasets | 🔵 Planned |
| [ANALYTICS-BEHAVIOR](https://github.com/K-RnD-Lab/ANALYTICS-BEHAVIOR) | Marketing analytics · behavioral modeling | 🔵 Planned |
| [ANALYTICS-OPEN](https://github.com/K-RnD-Lab/ANALYTICS-OPEN) | Open government · social data | 🔵 Planned |

*First repo target: Q4 2026*

---

## 🧭 How to Navigate

```
New to computational biology?
→ Start here:  PHYLO-DEMO  (no coding required)
→ Follow:      Learning Sandbox — Beginner → Intermediate → Advanced

Researcher / scientist?
→ Each repo contains:  report.md · execution_trace.ipynb · data/ · figures/
→ All hypotheses are labeled with confidence level (HIGH / MEDIUM / LOW)

Pharma or biotech?
→ PHYLO-DRUG     — RNA-directed compounds & synthetic lethal targets
→ PHYLO-LNP      — LNP formulation & delivery predictions
→ PHYLO-BIOMARKERS — liquid biopsy protein panels
→ All findings require experimental validation before application

Agriculture / food science?
→ BIO-PLANT — phytochemical bioactivity
→ BIO-AGRO  — biofertilizer & soil microbiome analysis

Developer?
→ CONTRIBUTING.md · Issues labeled [good first issue] · MIT License
```

---

## 📖 Citation

```bibtex
@misc{kolisnyk2026krdlab,
  author    = {Kolisnyk, Oksana},
  title     = {K R\&D Lab: Open-Source Computational Research Infrastructure},
  year      = {2026},
  publisher = {GitHub},
  url       = {https://github.com/K-RnD-Lab},
  note      = {Three series: PHYLO (oncology), BIO (life sciences),
               ANALYTICS (data science). All results are hypothesis-generating.}
}
```

---

## ⚠️ Disclaimer

All computational models are **research-grade and experimental**.
Results labeled `SIMULATED` are hypothesis-generating only and require
experimental validation before any clinical, pharmaceutical, or agricultural application.
This work does not constitute medical or agronomic advice.

---

<div align="center">

Built with Python · Gradio · scikit-learn · matplotlib · pandas

© 2026 Oksana Kolisnyk · [KOSATIKS GROUP](https://kosatiks-group.pp.ua) · MIT License

</div>
