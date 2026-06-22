# Executive Decision-Making Frameworks Playbook 🚀

Welcome to the **Executive Decision-Making Frameworks Playbook**. This repository serves as a centralized, practical guide to the world's most effective analytical models, prioritization funnels, and governance frameworks used in Technical Product Management, business strategy, and engineering leadership.

The goal of this toolkit is to replace gut-feeling opinions with structured, data-driven, and highly defensible decision-making mechanics.

---

## 📋 Table of Contents & The 10 Core Frameworks

### 🏛️ Section 1: Strategic & Environmental Analysis
1. **[SWOT Analysis](./strategic-analysis/SWOT-analysis.md)** (Strengths, Weaknesses, Opportunities, Threats)
   * *When to use:* Evaluating internal capabilities vs. external market realities.
2. **[PESTLE Analysis](./strategic-analysis/PESTLE-analysis.md)** (Political, Economic, Social, Technological, Legal, Environmental)
   * *When to use:* High-level macro-environmental analysis for long-term product roadmaps and global risk assessments.

### 🔍 Section 2: Root Cause Analysis & Problem Solving
3. **[Fishbone (Ishikawa) Diagram](./root-cause-problem-solving/fishbone-ishikawa.md)**
   * *When to use:* Visualizing and categorizing potential causes of a complex systemic problem or architectural failure.
4. **[The 5 Whys Methodology](./root-cause-problem-solving/5-whys.md)**
   * *When to use:* Drilling down rapidly to the behavioral, process, or technical root cause of an incident or operational bottleneck.

### 🎯 Section 3: Prioritization Funnels & Frameworks
5. **[RICE Scoring Model](./prioritization-funnels/RICE-scoring.md)** (Reach, Impact, Confidence, Effort)
   * *When to use:* Objective backlog grooming and feature prioritization using quantifiable metrics.
6. **[MoSCoW Method](./prioritization-funnels/MoSCoW-method.md)** (Must have, Should have, Could have, Won't have)
   * *When to use:* Setting immediate MVP boundaries and release scoping with cross-functional stakeholders.
7. **[WSJF Framework](./prioritization-funnels/WSJF-framework.md)** (Weighted Shortest Job First)
   * *When to use:* Sequencing complex epics in Agile/SAFe environments by calculating the immediate cost of delay.

### ⚡ Section 4: Advanced Hierarchy & Decision-Making
8. **[AHP (Analytic Hierarchy Process)](./decision-making-execution/AHP-hierarchy-process.md)**
   * *When to use:* Multi-criteria decision-making when evaluating high-stakes alternatives such as vendor selections or architectural paths.
9. **[The Cynefin Framework](./decision-making-execution/cynefin-framework.md)**
   * *When to use:* Categorizing operational contexts (Clear, Complicated, Complex, Chaotic) to choose the right leadership or engineering response.
10. **[RACI Matrix](./decision-making-execution/RACI-matrix.md)** (Responsible, Accountable, Consulted, Informed)
    * *When to use:* Establishing cross-functional governance, resource mapping, and clear ownership streams for critical deployments.

---

## 🛠️ High-Level Highlights & Mathematical Foundations

Here is a quick overview of how some of these frameworks introduce objective metrics into product decisions:

### 🔢 The RICE Scoring Equation
To bring mathematical objectivity to feature backlogs, initiatives are scored using:

$$RICE = \frac{Reach \times Impact \times Confidence}{Effort}$$

* **Reach:** Number of users impacted over a specific timeframe (e.g., users per quarter).
* **Impact:** Relative contribution to a quantitative goal (3 = Massive, 2 = High, 1 = Medium, 0.5 = Low).
* **Confidence:** Data certainty percentage (100% = High, 80% = Medium, 50% = Low/Speculative).
* **Effort:** Total person-months required from all teams to ship.

### ⏱️ Weighted Shortest Job First (WSJF)
To optimize delivery pipelines based on economic return and speed, SAFe environments leverage:

$$WSJF = \frac{Cost\ of\ Delay\ (CoD)}{Job\ Size}$$

Where **Cost of Delay** is determined by summing: `User-Business Value` + `Time Criticality` + `Risk Reduction/Opportunity Enablement`.

---

## 🚀 How to Use This Playbook

1.  **Browse by Problem Type:** Click on any framework in the [Table of Contents](#-table-of-contents--the-10 core-frameworks) to navigate directly to its dedicated deep-dive page.
2.  **Deploy the Templates:** Each deep-dive file contains markdown templates and real-world execution matrices that you can copy-paste straight into your project wikis, Confluence spaces, or roadmap documentation.
3.  **Contribute:** Found an interesting edge case or have a real-world matrix to share? Feel free to open an issue or submit a Pull Request to grow the playbook!
