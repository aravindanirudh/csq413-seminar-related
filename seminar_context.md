# CSQ413 Seminar: Comprehensive Project Context and Continuation Guide

This document provides complete project context, metadata, structural breakdowns, academic constraints, and compilation instructions for the CSQ413 B.Tech Seminar. It enables seamless continuation in a new conversation session.

---

## 1. Project and Student Metadata

- **Student Name:** Aravind A Kamath (ARAVIND A KAMATH)
- **Candidate Code / Register Number:** CEC23CS041
- **Class / Batch:** S7 B.Tech Computer Science and Engineering (Class Roll Number: 20)
- **Course:** CSQ413 Seminar (2019 Scheme, APJ Abdul Kalam Technological University / KTU)
- **Seminar Guide:** Mrs. Jayasree K, Assistant Professor, Department of CSE
- **Seminar Coordinators:** Mrs. Deepa C G, Mrs. Seethamol S, Mrs. Vidya S Mony (Assistant Professors, Dept. of CSE)
- **Head of Department (HoD):** Dr. Preetha Theresa Joy, Professor, Dept. of CSE
- **Principal:** Dr. Jaya V L
- **Department:** Department of Computer Science and Engineering
- **Institution:** College of Engineering, Pallippuram P O, Cherthala, Alappuzha Pin: 688541 (CECTL)
- **Academic Session / Date:** September 2026

---

## 2. Base Research Paper Details

- **Title:** Generative Agents in Agent-Based Modeling: Overview, Validation, and Emerging Challenges
- **Authors:** Carlo Adornetto, Adrian Mora, Kai Hu, Leticia Izquierdo Garcia, Parfait Atchade-Adelomou, Gianluigi Greco, Luis Alberto Alonso Pastor, Kent Larson
- **Journal:** IEEE Transactions on Artificial Intelligence, Vol. 6, No. 12, pp. 3165-3184, December 2025
- **Publisher:** IEEE
- **DOI:** 10.1109/TAI.2025.3566362
- **File Location:** `Seminar Abstract/Generative_Agents_in_Agent-Based_Modeling_Overview_Validation_and_Emerging_Challenges.pdf`

---

## 3. Strict Rules, Formatting, and Style Constraints

1. **Punctuation Constraint:** Never use em dashes ('---' or unicode '-') or en dashes ('--' or unicode '-'). Always use only standard single '-' hyphens across both LaTeX source files and documentation.
2. **Academic Tone:** Strictly non-opinionated, factual, and academically rigorous. All statements, analyses, comparisons, and conclusions are completely grounded in what is established in the base research paper.
3. **Seminar Report Headings:** Headings in the seminar report MUST match the exact section headings of the base research paper:
   - Preliminary front matter and References are unnumbered.
   - Main chapters are numbered using Roman numerals matching the base paper (`Chapter I: INTRODUCTION` through `Chapter X: CONCLUSION`).
4. **Report Page Budget:** Strictly **30-35 pages**. The report code in `Aravind_Seminar_Report/main.tex` is calibrated at ~59 KB (1,061 lines), estimating ~32-34 compiled PDF pages.
5. **Image Handling:** All images must reside inside the `figures/` subfolder. In LaTeX, `\graphicspath{{./}{./figures/}}` is used so that files resolve cleanly. Image dimensions are properly bounded using `keepaspectratio` and `\textwidth` scaling to prevent page overflow.

---

## 4. Repository Structure and Active Directories

```
Seminar Related GitHub Repo/
├── seminar_context.md                                         (This continuity document)
├── context.md                                                 (Initial presentation context)
├── README.md                                                  (Repository overview)
├── CSQ413_Seminar_Syllabus.pdf                                (University syllabus and evaluation scheme)
├── Seminar_Assessment_Form.pdf                                (Official evaluation mark sheet)
├── Aravind_A_Kamath_CEC23CS041_CSQ413_Seminar_Summary.pdf     (Preliminary seminar notes)
├── Seminar Abstract/                                          (Abstracts and base paper repository)
│   ├── Generative_Agents_in_Agent-Based_Modeling_...pdf       (Base research paper)
│   ├── 20_AravindAKamath_Seminar_Abstract.pdf                 (Submitted abstract PDF)
│   ├── 20_AravindAKamath_Seminar_Abstract.docx                (Submitted abstract Word doc)
│   └── seminar-base-paper-selection.json                      (Paper selection metadata)
├── Aravind_Seminar_Presentation/                              (Active Presentation Directory)
│   ├── main.tex                                               (Complete 32-slide Beamer source, latest on disk)
│   ├── fig1_ai_in_abm.png                                     (Figure 1 from base paper)
│   ├── fig2_ga_feedback_loop_status.png                       (Figure 2 from base paper)
│   ├── fig3_gabm_validation_workflows.png                     (Figure 3 from base paper)
│   └── README.md                                              (Presentation build guide)
├── Aravind_Seminar_Report/                                    (Active Report Directory)
│   ├── main.tex                                               (Complete 30-35 page KTU report source)
│   └── figures/                                               (Image assets for report)
│       ├── fig1_ai_in_abm.png                                 (Figure 1: AI in ABM development)
│       ├── fig2_ga_feedback_loop_status.png                   (Figure 2: GA feedback loop and status)
│       ├── fig3_gabm_validation_workflows.png                 (Figure 3: GABM validation workflows)
│       └── logo.jpg                                           (College of Engineering Cherthala crest)
└── Sample_Seminar_Report/                                     (Reference Sample Directory - Arjun Manoj)
    ├── main.tex                                               (Arjun's 39-page sample report source)
    ├── ArjunManoj_CEC23CS043_Seminar_Report.pdf               (Compiled sample report PDF)
    └── figures/                                               (Egg detection sample images)
```

---

## 5. Seminar Technical Report Architecture (`Aravind_Seminar_Report/main.tex`)

The report is written with `\documentclass[12pt,a4paper]{report}`, Times font (`newtxtext`, `newtxmath`), 1.5 line spacing, and 1.3-inch left / 1-inch right/top/bottom margins as per KTU thesis format.

### Detailed Page Breakdown (Target: 30-35 Pages)

| Section / Chapter | Title / Topic | Elements Included | Estimated Pages |
| :--- | :--- | :--- | :---: |
| **Front Matter** | Cover Page | Title, Student, Guide, Dept, Logo, College details | 1 |
| **Front Matter** | Second Title Page | KTU B.Tech degree submission metadata | 1 |
| **Front Matter** | Certificate | Guide, Co-ordinator, HoD signatories | 1 |
| **Front Matter** | Acknowledgement | Thanks to Principal, HoD, Coordinators, Guide, Friends | 1 |
| **Front Matter** | Abstract | Strictly 1 single page (condensed to ~1,900 chars) | 1 |
| **Front Matter** | Table of Contents | `\tableofcontents` (two pages vi-vii) | 2 |
| **Front Matter** | List of Figures & Tables | `\listoffigures` (viii) and `\listoftables` (ix) | 2 |
| **Chapter I** | INTRODUCTION | ABM definition, bounded rationality, homo economicus, GenAI | 2.5 |
| **Chapter II** | ABMS AND GENERATIVE ABMS | Epstein generative social science vs GenAI, **Table I (Traffic)** | 2.5 |
| **Chapter III** | EVOLVING AGENTS | EAs, RL, Structural Specification & Output Analysis, **Figure 1** | 2.5 |
| **Chapter IV** | GENERATIVE AGENTS | Parameters vs Status, **Figure 2**, Memory scoring formula, Reflection tree, Planning, **Table II (GABMs)** | 3.5 |
| **Chapter V** | INFORMAL THEORY OF ABMS VALIDATION | Verification vs Validation, Data analytics, Docking, Bootstrapping, Causal DAGs, IGSS, Face validation | 2.0 |
| **Chapter VI** | GABMS VALIDATION | Black-box dilemma, **Figure 3**, Smallville ablation, SOTOPIA-EVAL, LLM-as-a-Judge, Algorithmic fidelity | 2.5 |
| **Chapter VII** | ABM VS GABM: A COMPARISON | Systematic comparative analysis across Resources, Design, Behavior, Validation, **Table III** | 2.5 |
| **Chapter VIII** | GABMS: EMERGING CHALLENGES | Factuality/faithfulness hallucinations, attention complexity $\mathcal{O}(n^2 \cdot d)$, communication scaling $\mathcal{O}(N^2)$ | 2.0 |
| **Chapter IX** | DISCUSSION | Epistemological validity, Cities as testbeds, Qualitative Experience Mapping, Hybrid ABM-GABM, Fire evacuation case study | 2.0 |
| **Chapter X** | CONCLUSION | Four core pillars of GABM, future research trajectories | 1.5 |
| **References** | References | 20 peer-reviewed IEEE citations matching base paper | 1.5 - 2.0 |
| **Total** | **Complete Document** | **Front matter (9) + Chapters (21) + References (2)** | **~32-34 Pages** |

---

## 6. Mathematical Formulations Encapsulated in the Report

1. **Agent-Based System Tuple:**
   $$\mathcal{S}_t = \langle \mathcal{A}_t, \mathcal{E}_t, \mathcal{I}_t \rangle$$
2. **Micro-Level Action Decision:**
   $$u_{i,t} = \pi_i(s_{i,t}, \mathcal{O}_{i,t})$$
3. **Reinforcement Learning Objective (MDP):**
   $$J(\pi) = \mathbb{E}_{\pi} \left[ \sum_{k=0}^{\infty} \gamma^k \mathcal{R}(s_{t+k}, u_{t+k}) \right]$$
4. **Memory Stream Multi-Factor Retrieval Scoring:**
   $$\text{Score}(m, q) = \alpha \cdot \text{Recency}(m) + \beta \cdot \text{Importance}(m) + \gamma \cdot \text{Relevance}(m, q)$$
   - Exponential Recency Decay: $\text{Recency}(m) = e^{-\lambda (t_{\text{current}} - t_{\text{last\_access}})}$
   - Embedding Cosine Relevance: $\text{Relevance}(m, q) = \frac{\mathbf{e}_m \cdot \mathbf{e}_q}{\|\mathbf{e}_m\| \|\mathbf{e}_q\|}$
5. **Self-Attention Context Computational Complexity:**
   $$\text{Complexity}_{\text{Attention}} = \mathcal{O}(n^2 \cdot d)$$
6. **Pairwise Agent Inter-Communication Scaling:**
   $$\text{Complexity}_{\text{Communication}} = \mathcal{O}(N^2)$$
7. **Memory Stream Vector Indexing Complexity:**
   $$\text{Complexity}_{\text{Retrieval}} \in [\mathcal{O}(\log M), \mathcal{O}(M)]$$

---

## 7. Comparative Tables Encapsulated in the Report

- **Table I: Comparison between Traditional ABM and Generative ABM (Urban Traffic Flow Scenario):**
  - Contrasts Objective, Outcomes & Generalization, and Decision Basis.
- **Table II: Comparison of Existing GABMs:**
  - Evaluates SOTOPIA (2024), CRSEC Norm Emergence (2024), Concordia (2023), Smallville (2023), and S3 Platform (2023).
- **Table III: Systematic Comparison Between ABM and GABM:**
  - Compares Rule-based, EA-based, RL-based, and GABM across 17 distinct attributes spanning Resources, Agent Design, Agent Behavior, and Validation.

---

## 8. Presentation Slide Deck Overview (`Aravind_Seminar_Presentation/main.tex`)

The presentation deck uses `\documentclass{beamer}` with `\usetheme{Madrid}`, custom color definitions (`themeblue`, `lightgray`, `advgreen`, `limred`), and date restricted to the footer. Total: 32 slides.

- Slide 1: Title Slide (Student, Roll No, Guide, Dept affiliation)
- Slide 2: Presentation Outline (9 agenda sections)
- Slide 3: Background: Agent-Based Modeling (ABM)
- Slide 4: The Concept of 'Generative' in Social Science (Epstein, Schelling, Reynolds)
- Slide 5: Traditional ABM vs. Generative ABM: Urban Traffic Flow (Table I)
- Slide 6: Evolution of Agents: Evolutionary Algorithms (EAs)
- Slide 7: Evolution of Agents: Reinforcement Learning (RL)
- Slide 8: AI Integration in ABM Development (Figure 1: Structural Specification vs Output Analysis)
- Slide 9: Defining Generative Agents (GAs)
- Slide 10: GA Decision Architectures: Inferential vs. Conversational (Figure 2)
- Slide 11: Internal State Representation: Parameters vs. Dynamic Status (Textual bullets)
- Slide 12: Core Cognitive Components: Memory Stream & Retrieval (Formula)
- Slide 13: Core Cognitive Components: Reflection & Dynamic Planning
- Slide 14: Notable Implementations: The Smallville Sandbox (Park et al., 25 agents)
- Slide 15: General-Purpose Simulation Frameworks (Concordia, SOTOPIA)
- Slide 16: Social Norm Emergence and Online Networks (CRSEC pipeline, S3)
- Slide 17: The Fundamental Validation Dilemma (White-box vs Black-box)
- Slide 18: Traditional ABM Validation Methods (Docking, empirical, IGSS, spatial)
- Slide 19: Face Validation: Qualitative and Human-Centric (Microface, Macroface, Immersive)
- Slide 20: GABM Validation Workflows: The Integrated Architecture (Figure 3)
- Slide 21: Validating Existing GAs: Empirical Implementations (Smallville, SOTOPIA-EVAL)
- Slide 22: Automated Validation: LLM-as-a-Judge & Algorithmic Fidelity
- Slide 23: Comparison: Resources and Agent Design (Table III Part 1)
- Slide 24: Comparison: Agent Behavior and Validation (Table III Part 2)
- Slide 25: Challenge 1: Large Language Model Hallucinations
- Slide 26: Challenge 2: Computational Bottlenecks and Scaling (Attention $\mathcal{O}(n^2 \cdot d)$)
- Slide 27: Discussion: Cities as a Natural Testbed for GABMs
- Slide 28: The Proposed Solution: Combined Hybrid ABM-GABM
- Slide 29: Case Study: Building Evacuation & Hybrid Validation
- Slide 30: Conclusion and Key Insights (4 core takeaways)
- Slide 31: References (6 core references from base paper, compact layout)
- Slide 32: Closing & Thank You Slide

---

## 9. How to Compile the Documents

### Compiling the Technical Seminar Report (`Aravind_Seminar_Report`)
- **Option A (Overleaf):**
  1. Compress the entire folder `Aravind_Seminar_Report/` (containing `main.tex` and the `figures/` subfolder) into a `.zip` archive.
  2. Upload to Overleaf as a New Project.
  3. Ensure the compiler is set to **pdfLaTeX**.
  4. Click **Recompile**.
- **Option B (Local Terminal with TeX Live or MiKTeX):**
  ```powershell
  cd "Aravind_Seminar_Report"
  pdflatex main.tex
  pdflatex main.tex
  ```
  *(Running twice ensures Table of Contents, List of Figures, List of Tables, and cross-references resolve properly).*

### Compiling the Presentation Slide Deck (`Aravind_Seminar_Presentation`)
- **Option A (Overleaf):**
  1. Compress `Aravind_Seminar_Presentation/` into a `.zip` archive.
  2. Upload to Overleaf, set compiler to **pdfLaTeX**, and click **Recompile**.
- **Option B (Local Terminal):**
  ```powershell
  cd "Aravind_Seminar_Presentation"
  pdflatex main.tex
  pdflatex main.tex
  ```

---

## 10. Key Items for Next Conversation / Future Tasks

When continuing in a new conversation, the following tasks can be directly initiated:
1. **Report Re-Verification:** If university feedback requires specific tweaks to margins, font sizes, or chapter subsections, edit `Aravind_Seminar_Report/main.tex`.
2. **Presentation Speaker Notes:** Generate slide-by-slide verbal speaker notes aligned with the 32 slides for a 20-minute seminar delivery.
3. **Seminar Defense / Viva Preparation:** Generate expected faculty questions, cross-examination points on black-box validation, and defensive answers grounded in the base paper.
4. **Seminar Diary Entries:** Draft weekly progress log entries required for the 10 marks awarded by the Seminar Coordinator under KTU CSQ413 regulations.
