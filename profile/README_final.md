<div align="center">

# 🔬 K R&D Lab

**Open-Source Computational Research Hub by [Oksana Kolisnyk](https://kosatiks-group.pp.ua)**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HuggingFace](https://img.shields.io/badge/🤗_HuggingFace-K--RnD--Lab-orange)](https://huggingface.co/K-RnD-Lab)
[![GitHub](https://img.shields.io/badge/GitHub-K--RnD--Lab-181717?logo=github)](https://github.com/K-RnD-Lab)

*Computational research across science, technology, and analytics*

> ⚠️ All models are hypothesis-generating and require experimental or empirical validation.

</div>

---

## 🌐 Three Research Spheres

```
K R&D Lab
│
├── 🧪 SCIENCE      — biology, medicine, plant science, ecology, chemistry
├── 💻 TECH         — ML tools, bioinformatics pipelines, open infrastructure
└── 📊 ANALYTICS    — health data, marketing, behavioral, open social data
```

**How findings are meant to be used:**
- Scientists → take hypotheses into wet-lab or field validation
- Pharma / Agro / Tech → evaluate leads for applied development
- Students & researchers → replicate, extend, cite

---

## 🧪 SPHERE I — SCIENCE

Computational approaches to natural sciences.
Methods: bioinformatics, cheminformatics, statistical modeling, network analysis.

---

### 🩺 S1 — Biomedical & Oncology

> *Computational models for cancer biology, RNA therapeutics, nanoparticle delivery,
> biomarkers, and rare cancers.*

Organized into 6 sub-directions, each with its own GitHub repo and HuggingFace Space:

```
S1 — Biomedical & Oncology
│
├── 🧬 S1-A · PHYLO-GENOMICS     ← Genomics & Variants
├── 🔬 S1-B · PHYLO-RNA          ← RNA Therapeutics
├── 💊 S1-C · PHYLO-DRUG         ← Drug Discovery
├── 🧪 S1-D · PHYLO-LNP          ← Nanoparticle Delivery
├── 🩸 S1-E · PHYLO-BIOMARKERS   ← Biomarkers & Diagnostics
└── 🧠 S1-F · PHYLO-RARE         ← Rare Cancers / Frontier
```

**Entry point (all 10 tools, beginner demo):**
[![Demo](https://img.shields.io/badge/🤗-S1_DEMO-orange)](https://huggingface.co/spaces/K-RnD-Lab/S1-Demo)
[![Repo](https://img.shields.io/badge/GitHub-S1--Demo-181717?logo=github)](https://github.com/K-RnD-Lab/S1-Demo)

---

#### 🧬 S1-A · PHYLO-GENOMICS — Genomics & Variants
> *"What breaks in DNA — and how pathogenic is it?"*

[![Repo](https://img.shields.io/badge/GitHub-PHYLO--GENOMICS-181717?logo=github)](https://github.com/K-RnD-Lab/PHYLO-GENOMICS)
[![Space](https://img.shields.io/badge/🤗-PHYLO--GENOMICS-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-GENOMICS)

| Code | Tool | Key Finding | Data | Status |
|------|------|-------------|------|--------|
| S1-R1 | **OpenVariant v2** | AUC=0.939 · matches AlphaMissense without deep learning | ClinVar 2026 · gnomAD | ✅ Active |
| S1-R1b | Somatic mutation classifier | BRCA1/2 · TP53 · EGFR · ALK panels | TCGA-BRCA · TCGA-LUAD | 🔶 In progress |
| S1-R12a | Rare variant explorer | DIPG H3K27M · UVM GNAQ/GNA11 · ACC MYB-NFIB | PBTA · TCGA-UVM | 🔴 Planned |

---

#### 🔬 S1-B · PHYLO-RNA — RNA Therapeutics
> *"How to silence what's broken — through RNA"*

[![Repo](https://img.shields.io/badge/GitHub-PHYLO--RNA-181717?logo=github)](https://github.com/K-RnD-Lab/PHYLO-RNA)
[![Space](https://img.shields.io/badge/🤗-PHYLO--RNA-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-RNA)

| Code | Tool | Key Finding | Data | Status |
|------|------|-------------|------|--------|
| S1-R2 | **miRNA predictor** (BRCA1/2, TP53) | hsa-miR-148a-3p top silenced in BRCA2-mut | TCGA-BRCA · miRBase | ✅ Active |
| S1-R3 | **siRNA synthetic lethal** (20+ cancers) | SPC24, BUB1B, CDC45 — no existing drugs in LUAD | DepMap CERES · GEO | ✅ Active |
| S1-R4 | **lncRNA-TREM2** network | CYTOR→miR-138-5p→AKT1 controls neuroinflammation | LNCipedia · miRBase | ✅ Active |
| S1-R4b | ASO designer | GAS5 pos.119 · CYTOR pos.507 — accessibility >0.65 | RNAfold · literature | ✅ Active |

---

#### 💊 S1-C · PHYLO-DRUG — Drug Discovery
> *"Which small molecule fits the RNA target?"*

[![Repo](https://img.shields.io/badge/GitHub-PHYLO--DRUG-181717?logo=github)](https://github.com/K-RnD-Lab/PHYLO-DRUG)
[![Space](https://img.shields.io/badge/🤗-PHYLO--DRUG-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-DRUG)

| Code | Tool | Key Finding | Data | Status |
|------|------|-------------|------|--------|
| S1-R5 | **FGFR3 RNA-directed compounds** | CHEMBL1575701 — RNA score 0.793, near-zero toxicity | ChEMBL · RNAfold | ✅ Active |
| S1-R5b | Synthetic lethal drug mapping | PLK1, CDK1 — clinical-stage compounds in LUAD/BRCA | DepMap · ChEMBL | 🔶 In progress |
| S1-R13 | **m6A × Ferroptosis × Circadian** ⭐ | Pan-cancer triad — **never studied as integrated system** | TCGA-PAAD · GEO | 🔴 Frontier |

---

#### 🧪 S1-D · PHYLO-LNP — Nanoparticle Delivery & Corona
> *"How does the drug reach the tumor — and what proteins coat it along the way?"*

[![Repo](https://img.shields.io/badge/GitHub-PHYLO--LNP-181717?logo=github)](https://github.com/K-RnD-Lab/PHYLO-LNP)
[![Space](https://img.shields.io/badge/🤗-PHYLO--LNP-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-LNP)

| Code | Tool | Key Finding | Data | Status |
|------|------|-------------|------|--------|
| S1-R6 | **Corona predictor (serum)** | CHL/HL/PEG ratios dominate efficacy — AUC=0.791 | Literature proteomics | ✅ Active |
| S1-R7 | **Flow Corona — Vroman effect** | Blood flow accelerates albumin→ApoE exchange 3–4× | Kinetic models | ✅ Active |
| S1-R8 | **BBB / ApoE brain predictor** | pKa 6.2–6.8 + zeta ±5 mV → ApoE corona >20% | Literature | ✅ Active |
| S1-R10 | **AutoCorona NLP** | F1=0.71 extracting size/zeta/proteins from PMC | PubMed abstracts | ✅ Active |
| S1-R11 | **CSF / Vitreous / Bone Marrow** ⭐ | Corona in non-serum biofluids — **0 published studies globally** | PBTA · TARGET-AML | 🔴 Frontier |

---

#### 🩸 S1-E · PHYLO-BIOMARKERS — Biomarkers & Diagnostics
> *"How to detect cancer without tissue biopsy?"*

[![Repo](https://img.shields.io/badge/GitHub-PHYLO--BIOMARKERS-181717?logo=github)](https://github.com/K-RnD-Lab/PHYLO-BIOMARKERS)
[![Space](https://img.shields.io/badge/🤗-PHYLO--BIOMARKERS-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-BIOMARKERS)

| Code | Tool | Key Finding | Data | Status |
|------|------|-------------|------|--------|
| S1-R9 | **Liquid Biopsy classifier** | CTHRC1+FHL2+LDHA panel — AUC=0.992* | TCGA proteomics · CPTAC | ✅ Active |
| S1-R9b | Protein panel validator | CTHRC1 weight=0.18 dominates cancer score | TCGA · GEO plasma | 🔶 In progress |
| S1-R9c | ctDNA gap analysis | Zero validated panels in 7/10 rare cancers | ClinVar · GEO | 🔴 Planned |

*\*AUC reflects tissue proteomics proxy — plasma validation pending*

---

#### 🧠 S1-F · PHYLO-RARE — Rare Cancers (Frontier)
> *"Where almost nobody has looked yet — <300 cases/year, <5% survival"*

[![Repo](https://img.shields.io/badge/GitHub-PHYLO--RARE-181717?logo=github)](https://github.com/K-RnD-Lab/PHYLO-RARE)
[![Space](https://img.shields.io/badge/🤗-PHYLO--RARE-orange)](https://huggingface.co/spaces/K-RnD-Lab/PHYLO-RARE)

| Code | Toolkit | Key Gap | Data | Status |
|------|---------|---------|------|--------|
| S1-R12b | **DIPG toolkit** | H3K27M variants + CSF LNP + circadian biology | PBTA · GSE126319 | 🔴 In development |
| S1-R12c | **UVM toolkit** | GNAQ/GNA11 + vitreous humor corona + m6A | TCGA-UVM (n=80) | 🔴 In development |
| S1-R12d | **pAML toolkit** | FLT3-ITD + bone marrow niche corona + ferroptosis | TARGET-AML (~197) | 🔴 In development |

**Scientific basis:** Biomni gap analysis (March 2026) — PDAC #1, SCLC #2, DIPG highest gap per survival.
Corrected roadmap (v2, all critical errors fixed): [`docs/research-roadmap-v2.md`](docs/research-roadmap-v2.md)

---

### 🌿 S2 — Plant Science & Phytochemistry

> *"What bioactive compounds do plants produce — and what can they do?"*

[![Repo](https://img.shields.io/badge/GitHub-S2--Plant-181717?logo=github)](https://github.com/K-RnD-Lab/S2-Plant)

```
S2 — Plant Science
│
├── S2-R1  Phytochemical Profiler     ← compound → bioactivity (UNPD, KNApSAcK)
├── S2-R2  Plant Genome Browser       ← Arabidopsis, tomato, medicinal — Phytozome, TAIR
└── S2-R3  Anti-cancer Screener       ← plant compounds vs cancer targets (ChEMBL)
```

| Code | Tool | Status |
|------|------|--------|
| S2-R1 | Phytochemical Profiler | 🟡 In development |
| S2-R2 | Plant Genome Browser | 🔴 Planned |
| S2-R3 | Anti-cancer Screener | 🔴 Planned |

---

### 🌾 S3 — Agricultural Biology & Biofertilizers

> *"How do soil microbiomes support plant growth — and how can we engineer them?"*

[![Repo](https://img.shields.io/badge/GitHub-S3--Agro-181717?logo=github)](https://github.com/K-RnD-Lab/S3-Agro)

```
S3 — Agricultural Biology
│
├── S3-R1  Rhizosphere Microbiome     ← 16S community profiling (EBI MGnify, NCBI SRA)
├── S3-R2  Biofertilizer Predictor    ← microbial mix → yield improvement score
└── S3-R3  Soil Metabolomics          ← rhizosphere metabolite → pathway analysis
```

| Code | Tool | Status |
|------|------|--------|
| S3-R1 | Rhizosphere Microbiome | 🟡 In development |
| S3-R2 | Biofertilizer Predictor | 🔴 Planned |
| S3-R3 | Soil Metabolomics | 🔴 Planned |

---

### ⚗️ S4 — Biochemistry & Metabolomics

> *"What metabolic signatures distinguish healthy from diseased states?"*

[![Repo](https://img.shields.io/badge/GitHub-S4--Biochem-181717?logo=github)](https://github.com/K-RnD-Lab/S4-Biochem)

```
S4 — Biochemistry
│
├── S4-R1  Metabolite Profiler        ← HMDB compound → pathway mapping (Reactome, KEGG)
└── S4-R2  Pathway Enrichment         ← metabolomics data → enriched pathways
```

---

### 🧠 S5 — Neuroscience & Aging

> *"What computational patterns predict neurodegeneration and aging?"*

[![Repo](https://img.shields.io/badge/GitHub-S5--Neuro-181717?logo=github)](https://github.com/K-RnD-Lab/S5-Neuro)

```
S5 — Neuroscience & Aging
│
├── S5-R1  Neuroinflammation lncRNA   ← lncRNA-TREM2 extended network (Alzheimer)
├── S5-R2  Epigenetic Aging Clock     ← methylation-based biological age predictor
└── S5-R3  Immune Checkpoint Atlas    ← tumor immune evasion mechanisms
```

---

### 🌍 S6 — Ecology & Environmental Science *(target: 2027)*

```
S6 — Ecology
│
├── S6-R1  Environmental Microbiome   ← soil/water/air community analysis
├── S6-R2  Biodiversity Indices       ← public biodiversity datasets
└── S6-R3  Climate × Health           ← environmental exposure correlations
```

---

## 💻 SPHERE II — TECH

Computational tools, ML pipelines, and open bioinformatics infrastructure.
Methods: machine learning, NLP, statistical modeling, software engineering.

---

### 🤖 T1 — Machine Learning & Bioinformatics Tools

> *Reusable ML models and pipelines for life sciences data.*

[![Repo](https://img.shields.io/badge/GitHub-T1--MLTools-181717?logo=github)](https://github.com/K-RnD-Lab/T1-MLTools)

```
T1 — ML Tools
│
├── T1-R1  OpenVariant Engine          ← variant classifier, no deep learning (AUC=0.939)
├── T1-R2  Corona ML Pipeline          ← LNP formulation → efficacy prediction
├── T1-R3  AutoCorona NLP              ← PMC abstract → structured JSON
└── T1-R4  Synthetic Lethal Finder     ← multi-cancer SL target identification pipeline
```

| Code | Tool | Key result | Status |
|------|------|------------|--------|
| T1-R1 | OpenVariant Engine | AUC=0.939, no DL required | ✅ Active |
| T1-R2 | Corona ML Pipeline | AUC=0.791, PEG/lipid features dominate | ✅ Active |
| T1-R3 | AutoCorona NLP | F1=0.71, protein extraction from PMC | ✅ Active |
| T1-R4 | Synthetic Lethal Finder | 20+ cancers, DepMap CERES scoring | 🔶 In progress |

---

### 📈 T2 — Statistical Methods & Reproducibility

> *Frameworks, scoring systems, and open methodology for computational research.*

```
T2 — Statistical Methods
│
├── T2-R1  Research Gap Scoring       ← priority matrix: burden × gap × feasibility
└── T2-R2  Confidence Labeling        ← standardized HIGH/MEDIUM/LOW evidence labels
```

---

### 🧰 T3 — Open Research Infrastructure *(target: 2027)*

```
T3 — Infrastructure
│
├── T3-R1  Gradio Space Templates     ← reusable biology research UI templates
├── T3-R2  Literature Gap Detection   ← automated PubMed gap analysis pipeline
└── T3-R3  Rare Cancer Dataset Registry ← curated public datasets for rare cancers
```

---

## 📊 SPHERE III — ANALYTICS

Applied data analytics across health, behavior, and society.
Methods: statistical analysis, visualization, predictive modeling, A/B testing.

---

### 🏥 A1 — Health & Epidemiology Analytics

[![Repo](https://img.shields.io/badge/GitHub-A1--Health-181717?logo=github)](https://github.com/K-RnD-Lab/A1-Health)

```
A1 — Health Analytics
│
├── A1-R1  Population Health Patterns  ← mortality · incidence · epidemiology
└── A1-R2  Health Equity Analysis      ← demographic disparities in treatment access
```

---

### 🎯 A2 — Marketing & Behavioral Analytics

[![Repo](https://img.shields.io/badge/GitHub-A2--Marketing-181717?logo=github)](https://github.com/K-RnD-Lab/A2-Marketing)

```
A2 — Marketing & Behavioral
│
├── A2-R1  Consumer Behavior Modeling  ← behavioral data → purchase prediction
├── A2-R2  Campaign Effectiveness      ← A/B testing frameworks + attribution models
└── A2-R3  Audience Segmentation       ← clustering approaches for user personas
```

---

### 🗂️ A3 — Open & Social Data

[![Repo](https://img.shields.io/badge/GitHub-A3--OpenData-181717?logo=github)](https://github.com/K-RnD-Lab/A3-OpenData)

```
A3 — Open Data
│
├── A3-R1  Open Government Data        ← Ukraine + EU public datasets
└── A3-R2  Social Trend Analysis       ← public discourse and behavioral patterns
```

---

## 🗂️ Repository & Naming Convention

```
Naming pattern:  SPHERE-DIRECTION_RN_MonthYear

Examples:
  S1-Biomedical_R1_03-2026    ← OpenVariant (S1-A · PHYLO-GENOMICS)
  S1-Biomedical_R11_06-2026   ← LNP in CSF  (S1-D · PHYLO-LNP)
  S2-Plant_R1_09-2026         ← Phytochemical profiler
  A2-Marketing_R1_12-2026     ← Campaign analytics

Standard repo structure:
  README.md              ← research question · methods · key findings
  report.md              ← full findings + confidence labels (HIGH/MEDIUM/LOW)
  CITATION.cff           ← citation metadata
  LICENSE                ← MIT
  requirements.txt       ← Python dependencies
  app.py                 ← Gradio interactive demo (if applicable)
  data/raw/              ← original public datasets or download scripts
  data/processed/        ← cleaned, analysis-ready data
  figures/               ← all plots and visualizations
  execution_trace.ipynb  ← reproducible Jupyter notebook
```

---

## 🧭 Navigation

```
New to the lab?
  → S1 Demo Space — interactive, no coding, Learning Sandbox
  → Learning Mode: Beginner → Intermediate → Advanced (6 guided cases)

Scientist / researcher?
  → report.md in each repo — confidence labels + datasets + hypotheses
  → All claims labeled HIGH / MEDIUM / LOW confidence

Pharma / biotech?
  → S1-C PHYLO-DRUG   — RNA-directed small molecules
  → S1-D PHYLO-LNP    — LNP formulation & delivery predictions
  → S1-E PHYLO-BIOMARKERS — non-invasive protein panels

Agriculture / food science?
  → S2 Plant — phytochemical bioactivity
  → S3 Agro  — biofertilizer & rhizosphere microbiome

Data scientist / analyst?
  → T1 ML Tools · A1–A3 Analytics

Developer / contributor?
  → CONTRIBUTING.md · Issues labeled [good first issue] · MIT License
```

---

## 📖 Citation

```bibtex
@misc{kolisnyk2026krdlab,
  author    = {Kolisnyk, Oksana},
  title     = {K R\&D Lab: Open-Source Computational Research Hub},
  year      = {2026},
  publisher = {GitHub},
  url       = {https://github.com/K-RnD-Lab},
  note      = {Three spheres: Science (S), Tech (T), Analytics (A).
               All results are hypothesis-generating.}
}
```

---

## ⚠️ Disclaimer

All computational models are **research-grade and experimental**.
Results labeled `SIMULATED` require validation before clinical, pharmaceutical,
agricultural, or commercial application.
This work does not constitute medical, agronomic, or business advice.

---

<div align="center">

Built with Python · Gradio · scikit-learn · pandas · matplotlib

© 2026 Oksana Kolisnyk · [KOSATIKS GROUP](https://kosatiks-group.pp.ua) · MIT License

*Place this file at `.github/profile/README.md` inside the K-RnD-Lab GitHub organization*

</div>
