# CSQ413 Seminar Presentation: Generative Agents in Agent-Based Modeling

## Presentation Details
- **Student Name:** Aravind A Kamath
- **Roll Number:** 20
- **Candidate Code:** CEC23CS041
- **Subject:** CSQ413 Seminar
- **Assigned Guide:** Mrs. Jayasree K, Assistant Professor
- **Department:** Department of Computer Science and Engineering, College of Engineering, Cherthala
- **Base Paper:** Carlo Adornetto et al., *"Generative Agents in Agent-Based Modeling: Overview, Validation, and Emerging Challenges,"* IEEE Transactions on Artificial Intelligence, Vol. 6, No. 12, December 2025.

---

## Directory Contents
- `main.tex`: Complete LaTeX Beamer presentation (32 slides, Madrid theme).
- `fig1_ai_in_abm.png`: High-resolution extracted Figure 1 from the base paper.
- `fig2_ga_feedback_loop_status.png`: High-resolution extracted Figure 2 from the base paper.
- `fig3_gabm_validation_workflows.png`: High-resolution extracted Figure 3 from the base paper.

---

## Figure Placement Guide

| Slide # | Slide Title | Paper Figure | Image File | Description & Visual Contents |
| :--- | :--- | :--- | :--- | :--- |
| **Slide 8** | *AI Integration in ABM Development* | **Figure 1** (p. 4) | `fig1_ai_in_abm.png` | Illustrates the two domains of AI in ABM: Structural Specification and Output Analysis, with Generative AI driving population synthesis, interaction decision-making, and scenario generation. |
| **Slide 10** | *GA Decision Architectures: Inferential vs. Conversational* | **Figure 2(a) & 2(b)** (p. 5) | `fig2_ga_feedback_loop_status.png` | Contrasts the (a) Inferential GA feedback loop (LLM outputs discrete actions) with (b) Conversational GA feedback loop (natural language dialogues directly modifying internal agent status). |
| **Slide 11** | *Internal State Representation: Parameters vs. Dynamic Status* | **Figure 2(c)** (p. 5) | `fig2_ga_feedback_loop_status.png` | Schema of dynamic Agent Status containing demographic traits, real-time sentiment/emotional state, and chronological interaction memories. |
| **Slide 20** | *GABM Validation Workflows: The Integrated Architecture* | **Figure 3** (p. 11) | `fig3_gabm_validation_workflows.png` | Holistic validation flowchart mapping foundational and advanced ABM methods to Empirical, Macroface, and Microface validation pathways. |

### How to Toggle Between Placeholders and Direct Images
By default, the slides render clean, professional placeholder boxes indicating exact figure details. To render the actual extracted image files directly in the PDF:
1. Open `main.tex`.
2. Locate the corresponding `\begin{figure}` block.
3. Uncomment the line containing `\includegraphics[...]`.
4. Comment out or remove the `\fbox{\parbox{...}}` placeholder block.

---

## How to Compile

### Option 1: On Overleaf (Recommended for University Seminars)
1. Zip the entire `Aravind_Seminar_Presentation` folder (or upload all files inside it).
2. Create a "New Project" -> "Upload Project" on [Overleaf](https://www.overleaf.com).
3. Set the compiler to `pdfLaTeX` (Default) and click **Recompile**.

### Option 2: Local Compilation (TeX Live / MiKTeX)
Run the following terminal command inside this directory:
```bash
pdflatex main.tex
pdflatex main.tex
```
*(Running twice ensures slide numbers and navigation symbols are properly resolved).*
