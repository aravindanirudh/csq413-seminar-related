# Seminar Project Context and Continuation Guide

## Project Metadata
- **Subject:** CSQ413 Seminar (APJ Abdul Kalam Technological University / KTU)
- **Seminar Topic:** Generative Agents in Agent-Based Modeling: Overview, Validation, and Emerging Challenges
- **Student Name:** Aravind A Kamath
- **Candidate Code / Register Number:** CEC23CS041
- **Roll Number:** 20 (Class: S7 CS - A)
- **Seminar Guide:** Mrs. Jayasree K, Assistant Professor
- **Department:** Department of Computer Science and Engineering
- **Institution:** College of Engineering, Cherthala (CECTL)

---

## Base Research Paper Details
- **Title:** Generative Agents in Agent-Based Modeling: Overview, Validation, and Emerging Challenges
- **Authors:** Carlo Adornetto, Adrian Mora, Kai Hu, Leticia Izquierdo Garcia, Parfait Atchade-Adelomou, Gianluigi Greco, Luis Alberto Alonso Pastor, Kent Larson
- **Publication:** IEEE Transactions on Artificial Intelligence, Vol. 6, No. 12, pp. 3165-3184, December 2025
- **Publisher:** IEEE
- **DOI:** 10.1109/TAI.2025.3566362

---

## Strict Formatting and Style Rules
1. **Punctuation Constraint:** Never use em dashes ('-'). Always use only standard '-' hyphens.
2. **Academic Tone:** Strictly non-opinionated. All text, comparisons, and conclusions must be completely based on what is established in the base research paper.
3. **Slide Bullet Style:** All bullet points must be punchy, crisp, and to-the-point. Do not use long, paragraph-like descriptions on slides.
4. **Beamer Template:** Uses `\documentclass{beamer}` with `\usetheme{Madrid}` and `\usecolortheme{default}`.
5. **Title Page Date:** Date is omitted from the title page and placed only in the footer via `\date[\today]{}`.
6. **Figures:** High-resolution figures extracted directly from the base research paper are embedded via `\includegraphics`. Do not use float environments (`figure`) or captions on compact slides to prevent bottom vertical overflow.

---

## Directory and File Structure

```
Seminar Related/
├── context.md                                              (Root-level continuity document)
├── Aravind_A_Kamath_CEC23CS041_CSQ413_Seminar_Summary.pdf  (Topic summary notes)
├── CSQ413 Seminar.pdf                                      (University syllabus & evaluation scheme)
├── Generative_Agents_in_Agent-Based_Modeling_Overview_...pdf (Base research paper)
├── Seminar_Assessment_Form.pdf                             (Evaluation mark sheet)
├── Sample_Seminar_Report.pdf                               (Sample KTU seminar report)
├── Sample_Seminar_Presentation/                            (Faculty reference deck)
│   ├── main.tex
│   └── Sample_Seminar_Presentation.pdf
└── Aravind_Seminar_Presentation/                           (Active Project Directory)
    ├── main.tex                                            (Complete Beamer presentation source)
    ├── fig1_ai_in_abm.png                                  (Figure 1 from base paper)
    ├── fig2_ga_feedback_loop_status.png                    (Figure 2 from base paper)
    ├── fig3_gabm_validation_workflows.png                  (Figure 3 from base paper)
    ├── README.md                                           (Compilation & figure reference guide)
    └── context.md                                          (Presentation continuity document)
```

---

## Slide-by-Slide Breakdown of `main.tex` (32 Slides Total)

### Slide 1: Title Slide
- Title, subtitle, student name, roll number, guide details, and department affiliation. Date configured for footer only.

### Slide 2: Presentation Outline
- Table of contents covering all 9 major presentation sections.

### Slide 3: Background: Agent-Based Modeling (ABM)
- Definition, microscopic-to-macroscopic emergence, classical mechanics, homo economicus assumptions, and fundamental limitations regarding human bounded rationality.

### Slide 4: The Concept of 'Generative' in Social Science
- Historical roots from Joshua Epstein (1999) ("grow it to explain it"), classical models (Schelling segregation, Reynolds Boids), and the contemporary distinction between rule-based generative simulations and modern LLM-driven generative AI.

### Slide 5: Traditional ABM vs. Generative ABM: Urban Traffic Flow (Table I)
- Side-by-side comparison across Scenario, Objective, Outcomes, and Decision Basis based on Table I of the base paper.

### Slide 6: Evolution of Agents: Evolutionary Algorithms (EAs)
- Darwinian mechanics in ABM (selection, mutation, recombination), cultural algorithms with shared belief spaces, and EA bottlenecks (premature convergence, heavy hyperparameter tuning).

### Slide 7: Evolution of Agents: Reinforcement Learning (RL)
- Trial-and-error policy optimization, applications (pedestrian routing, evacuation), and challenges (stochastic instability, brittle transfer, absence of natural language dialogue).

### Slide 8: AI Integration in ABM Development
- Structural Specification vs. Output Analysis. Embeds `fig1_ai_in_abm.png` illustrating Population Synthesis, Decision Making via Interactions, and Scenario Generation.

### Slide 9: Defining Generative Agents (GAs)
- Formal definition, the environmental feedback loop, mechanical model vs. cognitive layer, and emergent behavioral rules.

### Slide 10: GA Decision Architectures: Inferential vs. Conversational
- Embeds `fig2_ga_feedback_loop_status.png` comparing (a) Inferential GA feedback loop (discrete action outputs) vs. (b) Conversational GA feedback loop (natural language dialogue updating internal status).

### Slide 11: Internal State Representation: Parameters vs. Dynamic Status
- Full-slide textual breakdown comparing static baseline parameters (demographics, OCEAN personality, social network) with runtime Dynamic Agent Status (sentiment tracking, memory logs, decoupled from LLM logic). Diagram omitted as requested.

### Slide 12: Core Cognitive Components: Memory Stream & Retrieval
- Chronological natural language database overcoming context limits. Mathematical formulation:
  $$\text{Score} = \alpha \cdot \text{Recency} + \beta \cdot \text{Importance} + \gamma \cdot \text{Relevance}$$

### Slide 13: Core Cognitive Components: Reflection & Dynamic Planning
- Hierarchical reflection tree (observations at leaves, abstract beliefs at higher tiers) and recursive plan decomposition (daily to minute-level execution with dynamic interruption).

### Slide 14: Notable Implementations: The Smallville Sandbox
- Park et al. (2023) 25-agent 2D town simulation. Emergent social dynamics: Valentine's Day party coordination, information diffusion, political campaigns, and ablation study findings.

### Slide 15: General-Purpose Simulation Frameworks
- Concordia (Google DeepMind): Centralized Game Master agent grounding actions in physical/digital reality.
- SOTOPIA: Interactive benchmark for multi-agent social intelligence (cooperation, competition, negotiation).

### Slide 16: Social Norm Emergence and Online Networks
- CRSEC 4-stage pipeline (Creation & Representation, Spreading, Evaluation, Compliance).
- S3 Platform (Gao et al.): Social network simulation of information diffusion, echo chambers, and emotional contagion.

### Slide 17: The Fundamental Validation Dilemma
- Epistemological gap: White-box deterministic traditional models vs. black-box probabilistic non-deterministic LLM agents. Hierarchy of evidence adaptation.

### Slide 18: Traditional ABM Validation Methods
- Foundational methods (data analytics, docking, empirical validation, sampling) and advanced methods (bootstrapping, causal analysis, Inverse Generative Social Science, spatial analytics).

### Slide 19: Face Validation: Qualitative and Human-Centric
- Microface validation (individual agent consistency), Macroface validation (collective aggregate patterns), and Immersive assessment (VR/interactive interviewing).

### Slide 20: GABM Validation Workflows: The Integrated Architecture
- Embeds `fig3_gabm_validation_workflows.png` with constrained height and compact bullet points detailing Empirical, Macroface, and Microface pathways without bottom overflow.

### Slide 21: Validating Existing GAs: Empirical Implementations
- Smallville 5-category interview evaluation across ablation conditions.
- SOTOPIA-EVAL 7-dimensional scoring matrix (Goal completion, Believability, Knowledge, Secret keeping, Relationship dynamics, Norm adherence, Financial benefit).

### Slide 22: Automated Validation: LLM-as-a-Judge & Algorithmic Fidelity
- LLM evaluators grading dialogues, empirical dual-evaluation insights (strengths on objective metrics, limitations on social nuance/deception), algorithmic fidelity, and similarity principle.

### Slide 23: Comparison: Resources and Agent Design (Table III)
- Formatted tabular analysis across Computational Efficiency, Scalability, Data Independence, Control, Learning, Optimization, Hyperparameter Tuning, and Fast Prototyping.

### Slide 24: Comparison: Agent Behavior and Validation (Table III)
- Formatted tabular analysis across Determinism, Reliable Decision-Making, Cognitive Functions, Language Interactions, Mental Models, Transparency, and Direct Interview Validation.

### Slide 25: Challenge 1: Large Language Model Hallucinations
- Factuality hallucinations vs. Faithfulness hallucinations. Mitigation stages: Data (RAG), Training (sensitive neuron dropout, RLHF), Inference (constrained decoding, multi-agent peer checks).

### Slide 26: Challenge 2: Computational Bottlenecks and Scaling
- Quadratic attention overhead: $\text{Complexity} = \mathcal{O}(n^2 \cdot d)$. Pairwise communication scaling $\mathcal{O}(N^2)$, memory retrieval indexing costs $\mathcal{O}(\log N)$ to $\mathcal{O}(N)$, and the resulting scalability gap.

### Slide 27: Discussion: Cities as a Natural Testbed for GABMs
- Urban community alignment, social norms in text corpora, and Qualitative Experience Mapping (emotional highs/lows) for human-centered urban planning.

### Slide 28: The Proposed Solution: Combined Hybrid ABM-GABM
- Synergy rather than replacement: Low-level deterministic mechanics (kinematics, collision, routing at $\mathcal{O}(1)$/$\mathcal{O}(N)$) paired with high-level cognitive decision-making via LLMs.

### Slide 29: Case Study: Building Evacuation & Hybrid Validation
- Concrete scenario: Building fire evacuation (deterministic navigation vs. ethical dilemma of aiding trapped peer). Multi-tier validation bridging sensor analytics with qualitative agent interviews.

### Slide 30: Conclusion and Key Insights
- Summary of four core takeaways: Paradigm shift, terminology clarification, validation blueprint, and hybrid architecture path forward.

### Slide 31: References
- 6 key peer-reviewed citations directly from the base paper, formatted with `\fontsize{7.5pt}{8.5pt}\selectfont` and `\setlength{\itemsep}{1pt}` to fit without overflow.

### Slide 32: Thank You & Interactive Discussion
- Closing slide with student credentials and Q&A prompt.

---

## Critical Fixes Completed
1. **Slide 11:** Removed duplicate Figure 2 diagram; converted parameters and status into full-slide to-the-point bullets.
2. **Slide 20:** Removed figure float/caption margins, bounded image height, and made pathway text compact to eliminate bottom overflow.
3. **Slide 22:** Flattened deep nested lists into concise, bulleted evaluation takeaways.
4. **Slide 23 & 24:** Stripped floating `table` environments, applied direct `\centering \scriptsize` with compact takeaway notes.
5. **Slide 26:** Replaced broken multi-list equation block with clean inline math $\mathcal{O}(n^2 \cdot d)$, removing large blank gaps.
6. **Slide 31:** Tuned font and line spacing so all references fit cleanly without overflowing the frame.
7. **Slide Text Tone & Density:** Replaced paragraph-like text with concise, presentation-ready bullets across all technical slides.

---

## How to Compile on Another PC

### Method A: Overleaf (Zero Setup)
1. Copy the entire folder `Aravind_Seminar_Presentation/` to a ZIP archive.
2. Go to [Overleaf](https://www.overleaf.com) -> "New Project" -> "Upload Project".
3. Upload the ZIP. Set compiler to `pdfLaTeX` and click **Recompile**.

### Method B: Local TeX Live / MiKTeX / VS Code
Open terminal in `Aravind_Seminar_Presentation/` and run:
```bash
pdflatex main.tex
pdflatex main.tex
```
*(Running twice ensures slide numbers and navigation links resolve properly).*

---

## Potential Next Steps for the Seminar Course (CSQ413)
- **Seminar Technical Report:** KTU CSQ413 requires submitting a formal seminar report following university guidelines (refer to `Sample_Seminar_Report.pdf` in parent directory for chapter structure, font sizes, margins, and declaration format).
- **Presentation Rehearsal / Speaker Notes:** Prepare speaking points corresponding to each slide, keeping within the standard 20-25 minute presentation window.
