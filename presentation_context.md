# CSQ413 Seminar Presentation Context and Continuation Guide

## 1. Project and Student Metadata
- **Student Name:** Aravind A Kamath (ARAVIND A KAMATH)
- **Candidate Code / Register Number:** CEC23CS041
- **Class / Roll Number:** S7 B.Tech CSE, Roll No: 20
- **Course Code & Name:** CSQ413 Seminar (2019 Scheme, APJ Abdul Kalam Technological University / KTU)
- **Seminar Topic:** Generative Agents in Agent-Based Modeling: Overview, Validation, and Emerging Challenges
- **Seminar Guide:** Mrs. Jayasree K, Assistant Professor, Department of Computer Science and Engineering
- **Seminar Coordinators:** Mrs. Deepa C G, Mrs. Seethamol S, Mrs. Vidya S Mony (Assistant Professors, Dept. of CSE)
- **Head of Department:** Dr. Preetha Theresa Joy, Professor, Dept. of CSE
- **Principal:** Dr. Jaya V L
- **Department:** Department of Computer Science and Engineering
- **Institution:** College of Engineering, Cherthala (CECTL)
- **Date / Session:** September 2026

---

## 2. Base Research Paper Details
- **Title:** Generative Agents in Agent-Based Modeling: Overview, Validation, and Emerging Challenges
- **Authors:** Carlo Adornetto, Adrian Mora, Kai Hu, Leticia Izquierdo Garcia, Parfait Atchade-Adelomou, Gianluigi Greco, Luis Alberto Alonso Pastor, Kent Larson
- **Publication:** IEEE Transactions on Artificial Intelligence, Vol. 6, No. 12, pp. 3165-3184, December 2025
- **Publisher:** IEEE
- **DOI:** 10.1109/TAI.2025.3566362
- **Source Location:** `Seminar Abstract/Generative_Agents_in_Agent-Based_Modeling_Overview_Validation_and_Emerging_Challenges.pdf`

---

## 3. Core Presentation Guidelines and Formatting Constraints
1. **Punctuation Rule:** Never use em dashes ('---' or unicode em-dash) or en dashes ('--' or unicode en-dash). Always use standard single '-' hyphens across LaTeX files and documentation.
2. **Academic Tone:** Strictly non-opinionated, factual and grounded entirely in the base paper.
3. **Bullet Point Style & Nesting:** All bullet points are flat (single-level, zero nested sub-bullets) for maximum readability. Each item uses `\textbf{Keyword:}` followed by 1-2 punchy lines, separated by `\medskip`.
4. **Font Size & Content Density:** Uses standard `\normalsize` across text slides (no tiny fonts). Content is trimmed to 3-5 high-impact bullet points per slide so that text breathes and remains easily legible from a distance.
5. **Formula Symbol Definitions:** Every equation (Slide 14 and Slide 26) includes a dedicated `\textbf{Symbol Definitions:}` block that defines every mathematical symbol explicitly.
6. **Table Formatting:** All tables feature vertical rules (`|`) separating columns, explicit `\hline` row borders and balanced column dimensions. Table 1 has enlarged font and generous row height (`\arraystretch{1.4}`). Literature Survey tables and Comparison tables feature crisp, compact cell content.
7. **Footer Layout:** Configured via `\author[Aravind A Kamath | CEC23CS041]{...}`, `\title[Generative Agents in ABM]{...}`, `\institute[]{...}` and `\date{}`. The footer displays:
   - Left box: `Aravind A Kamath | CEC23CS041`
   - Center box: `Generative Agents in ABM`
   - Right box: `Slide / Total` (e.g. `2 / 33`)
   No multi-line text clipping or date crowding.
8. **Outline and Headings:** The presentation outline strictly reflects the 10 chapter headings of the seminar report and base paper:
   1. Introduction
   2. ABMs and Generative ABMs
   3. Evolving Agents
   4. Generative Agents
   5. Informal Theory of ABMs Validation
   6. GABMs Validation
   7. ABM vs GABM: A Comparison
   8. GABMs: Emerging Challenges
   9. Discussion
   10. Conclusion
9. **Standalone Figure Slides:** Major figures (Figure 1: AI in ABM, Figure 2: GA feedback loop architectures, Figure 3: GABM validation workflows) are presented on full dedicated slides with `keepaspectratio` and `\caption{\scriptsize ...}`. The explanatory notes and pathways are provided on separate follow-up slides.
10. **Streamlined Deck Architecture:** Redundant or duplicate slides (e.g., separate EA/RL slides, duplicate Smallville slides, standalone empirical validation text slides) were merged or removed to ensure a lean 33-slide deck tailored for a 15-20 minute seminar presentation.

---

## 4. Complete Slide-by-Slide Breakdown (33 Slides)

### Front Matter
- **Slide 1: Title Slide:** Paper title, subtitle, student name, roll number, guide details, department and institution.
- **Slide 2: Outline:** Clean `\tableofcontents` displaying the 10 formal sections.

### Section 1: Introduction
- **Slide 3: Background: Agent-Based Modeling (ABM):** Bottom-up modeling, micro-to-macro emergence, applications in epidemiology, traffic and finance, core objective.
- **Slide 4: Limitations of Classical Behavioral Models:** Perfect economic rationality (*homo economicus*), lack of emotions, absence of natural language, rigid if-then rules, population homogeneity.

### Section 2: ABMs and Generative ABMs
- **Slide 5: The Concept of 'Generative' in Social Science:** Joshua Epstein's 1999 motto ("grow it to explain it"), classical models (Schelling segregation, Reynolds boids), and the technological shift to LLM-driven cognition.
- **Slide 6: Traditional ABM vs. Generative ABM: Urban Traffic Flow:** Formatted comparison table with vertical rules (Table I) across Scenario, Objective, Outcomes and Decision Basis. Tall row height (`\arraystretch{1.4}`) and enlarged font.

### Section 3: Evolving Agents
- **Slide 7: Precursor Agent Architectures: EAs and RL:** Merged precursor slide covering Evolutionary Algorithms (adaptation mechanics and local optima bottlenecks) and Reinforcement Learning (reward maximization, sample inefficiency and lack of language dialogue).
- **Slide 8: AI Integration in ABM Development:** Full-slide standalone graphic of Figure 1 (Structural Specification vs. Output Analysis).
- **Slide 9: Roles of Generative AI in ABM Development:** Textual breakdown of population synthesis, interactive decision-making, scenario generation, macro-level tracking and synthetic interviews.

### Section 4: Generative Agents
- **Slide 10: Defining Generative Agents (GAs):** Formal definition, two-layer architecture (Mechanical Layer vs. Cognitive Layer), emergent behaviors from pre-trained world knowledge.
- **Slide 11: Internal State: Static Parameters vs. Dynamic Status:** Static baseline parameters (demographics, Big Five OCEAN traits, social network) vs. Dynamic runtime status (location, current task, affective state, decoupled storage).
- **Slide 12: GA Decision Architectures: Feedback Loop and Status:** Full-slide standalone graphic of Figure 2 (Inferential and Conversational feedback loops).
- **Slide 13: Inferential vs. Conversational Feedback Loops:** Concise explanation of Figure 2(a) (discrete action engine) vs. Figure 2(b) (dialogue updating internal status).
- **Slide 14: Core Cognitive Modules: Memory Stream & Retrieval:** Chronological database, linear scoring formula ($\text{Score}(m, q) = \alpha \cdot \text{Recency}(m) + \beta \cdot \text{Importance}(m) + \gamma \cdot \text{Relevance}(m, q)$) with explicit definitions for every mathematical symbol ($m, q, \alpha, \beta, \gamma, \lambda, \Delta t, \mathbf{e}_m, \mathbf{e}_q$).
- **Slide 15: Core Cognitive Modules: Reflection & Dynamic Planning:** Hierarchical reflection tree (observations at leaves, beliefs at roots), recursive daily-to-minute planning, dynamic reactive re-planning.
- **Slide 16: Literature Survey: Existing GABMs (Part 1 - Platforms & Benchmarks):** Formatted comparison table with vertical rules (Table II Part 1) surveying Park et al. (Smallville), Vezhnevets et al. (Concordia), and Zhou et al. (SOTOPIA) across Simulation Scenario, Core Architecture, Key Highlights, and Validation Approach.
- **Slide 17: Literature Survey: Existing GABMs (Part 2 - Social Dynamics & Norms):** Formatted comparison table with vertical rules (Table II Part 2) surveying CRSEC (Social Norm Emergence), Gao et al. (S3 Platform), and Williams et al. (Epidemic Modeling).

### Section 5: Informal Theory of ABMs Validation
- **Slide 18: The Fundamental Validation Dilemma:** Purpose of validation, white-box deterministic models vs. black-box probabilistic LLMs, evidence hierarchy adaptation.
- **Slide 19: Foundational and Face Validation in Traditional ABM:** Merged foundational validation (data analytics, docking, empirical testing, bootstrapping) and qualitative face validation (microface, macroface, immersive probing).

### Section 6: GABMs Validation
- **Slide 20: GABM Validation Workflows Architecture:** Full-slide standalone graphic of Figure 3 (Validation workflows across validation purposes).
- **Slide 21: Integrated Validation Pathways:** Detailed breakdown of Empirical Pathway (data matching), Macroface Pathway (group emergence) and Microface Pathway (individual interviews).
- **Slide 22: Automated Validation: LLM-as-a-Judge & Algorithmic Fidelity:** Independent LLM evaluators, nuance detection limits, algorithmic fidelity, similarity principle.

### Section 7: ABM vs GABM: A Comparison
- **Slide 23: Comparison: Resources and Agent Design:** Formatted comparison table with vertical rules (Table III Part 1) across Efficiency, Scalability, Data, Control, Learning, Optimization, Hyperparameters and Prototyping, with takeaway bullets.
- **Slide 24: Comparison: Agent Behavior and Validation:** Formatted comparison table with vertical rules (Table III Part 2) across Determinism, Reliable Decisions, Cognition, Language, Mental Models, Transparency and Direct Interviewing, with takeaway bullets.

### Section 8: GABMs: Emerging Challenges
- **Slide 25: Challenge 1: Large Language Model Hallucinations:** Factuality vs. Faithfulness hallucinations, three-stage mitigation pipeline (Data: RAG, Training: RLHF, Inference: constrained decoding & peer checks).
- **Slide 26: Challenge 2: Computational Bottlenecks and Scaling:** Attention complexity ($\mathcal{O}(n^2 \cdot d)$) and communication scaling ($\mathcal{O}(N^2)$) formulas with complete symbol definitions ($n, d, N, M$) and the scalability gap.

### Section 9: Discussion
- **Slide 27: Discussion: Cities as a Natural Testbed for GABMs:** Civic text alignment, Qualitative Experience Mapping (QEM: tracking comfort, fear, stress for urban planning).
- **Slide 28: The Proposed Solution: Combined Hybrid ABM-GABM:** Complementary synergy, low-level mechanistic layer ($\mathcal{O}(1)$ or $\mathcal{O}(N)$ physics) paired with high-level cognitive LLM layer.
- **Slide 29: Case Study: Building Evacuation & Hybrid Validation:** Building fire emergency, physical corridor navigation vs. moral rescue dilemma, sensor validation paired with agent interviews.

### Section 10: Conclusion
- **Slide 30: Summary of Key Insights and Contributions:** Cognitive paradigm shift, conceptual clarity, multi-tiered validation pipeline, hybrid path forward.
- **Slide 31: Future Research Trajectories:** Grounded directly in Sections VIII, IX, and X of the base paper (compact SLMs, open multi-agent benchmarks, mathematical hallucination bounds, ethical bias safeguards).

### References and Closing
- **Slide 32: References:** Clean, single slide citing 6 foundational papers from the base paper bibliography.
- **Slide 33: Final Slide:** "Thank You!" and "Questions and Discussion" prompt.

---

## 5. Justification for References Included in the Reference Slide (Slide 32)

Each of the 6 references cited on Slide 32 was selected directly from the base research paper's core bibliography to ground specific sections of the presentation:

1. **Adornetto et al. (IEEE TAI 2025) [Ref 1]:**
   - *Why included:* This is the **base research paper** upon which the entire seminar is built. It introduces the taxonomies, comparison tables (Tables I, II & III), and validation workflows (Figures 1, 2 & 3).
2. **Epstein (Complexity 1999) [Ref 2]:**
   - *Why included:* Seminal paper defining **Generative Social Science**. It provides the fundamental motto (*"If you didn't grow it, you didn't explain it"*) used to contrast classical rule-based emergence with modern LLM-driven generative AI (Section II of base paper).
3. **Park et al. (ACM UIST 2023) [Ref 3]:**
   - *Why included:* Landmark paper introducing the **Smallville sandbox** (25 generative agents). It formulated the core cognitive modules used in modern GAs: the memory stream retrieval formula, hierarchical reflection trees, and recursive planning (Section IV & VI of base paper).
4. **Vezhnevets et al. (arXiv 2023) [Ref 4]:**
   - *Why included:* Introduces **Concordia** (Google DeepMind), defining the "Game Master" architecture that grounds open-ended language actions in physical coordinates and institutional rules (Section IV-D of base paper).
5. **Zhou et al. (ICLR 2024) [Ref 5]:**
   - *Why included:* Introduces **SOTOPIA**, the premier multi-agent benchmark for evaluating social intelligence across 7 quantitative dimensions, used as the primary validation testbed in Section IV and VI.
6. **Gao et al. (arXiv 2023) [Ref 6]:**
   - *Why included:* Introduces the **S3 Platform**, demonstrating how GAs simulate online social media behavior, information cascades, and echo chamber polarization (Section IV-D of base paper).

---

## 6. Origin of Future Improvements / Research Trajectories (Slide 31)

All future trajectories listed on Slide 31 are derived directly from the base research paper:
- **Small Language Models (SLMs) & Parameter Efficiency:** Directly addresses Section VIII-C (*"Computational Costs"*), where quadratic attention overhead $\mathcal{O}(n^2 \cdot d)$ and token API latency are identified as the primary barrier preventing scale beyond hundreds of agents.
- **Standardized Multi-Agent Benchmarks:** Directly stems from Section VIII-B (*"Validation"*), where the authors highlight the urgent need for open-source, standardized multi-agent benchmarks to objectively evaluate social intelligence and overcome LLM judge self-preference bias.
- **Mathematical Hallucination Bounds:** Directly addresses Section VIII-A (*"LLMs' Hallucinations"*), which demands formal verification mechanisms when GABMs are deployed for high-stakes urban and public policy simulations.
- **Ethical Safeguards & Bias Propagation Mitigation:** Directly from Section VIII-A and Section IX-A (*"Addressing Broader Questions"*), emphasizing that simulated agents must be safeguarded against inheriting cultural and behavioral biases embedded in training corpora.

---

## 7. How to Compile the Presentation Slide Deck
### Method A: Overleaf (Recommended)
1. Compress the entire folder `Aravind_Seminar_Presentation/` into a `.zip` file.
2. Go to [Overleaf](https://www.overleaf.com) -> New Project -> Upload Project.
3. Select `pdfLaTeX` as compiler and click **Recompile**.

### Method B: Local Command Line (TeX Live / MiKTeX)
```powershell
cd "Aravind_Seminar_Presentation"
pdflatex main.tex
pdflatex main.tex
```
*(Running twice guarantees that section numbers, outline hyperref anchors and slide counters resolve cleanly).*
