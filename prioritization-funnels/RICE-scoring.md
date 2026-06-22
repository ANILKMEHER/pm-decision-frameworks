# RICE Scoring Model 🎯

## 1. What is it?
RICE is a quantitative prioritization framework designed to help product managers objectively evaluate and score competing features, ideas, or projects. By calculating a single, standardized score based on data and confidence levels, it removes internal bias and opinions from roadmap discussions.

## 2. The Formula & Components

$$RICE = \frac{Reach \times Impact \times Confidence}{Effort}$$

* **Reach (Quantitative):** How many users will this feature affect within a specific timeframe? (e.g., *1,500 users per quarter*).
* **Impact (Qualitative Estimate):** How much will this feature benefit an individual user? 
    * 3 = Massive impact
    * 2 = High impact
    * 1 = Medium impact
    * 0.5 = Low impact
* **Confidence (Percentage):** How sure are you about your Reach, Impact, and Effort estimates based on data?
    * 100% = High confidence (supported by user research/analytics data)
    * 80% = Medium confidence (supported by qualitative feedback or proxy data)
    * 50% = Low confidence (speculative or "gut feeling")
* **Effort (Person-Months):** The total time required from all team members (product, design, engineering) to deliver the feature. (e.g., *If 1 developer and 1 designer work on it for 2 months, Effort = 4 person-months*).

---

## 3. Real-World Application Example
### Scenario: Prioritizing Backlog Items for an Enterprise App Upgrade

| Backlog Feature | Reach (Qtr) | Impact | Confidence | Effort (Person-Mo) | RICE Score Calculation | Priority |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **A: Biometric Login Integration** | 5,000 | 2.0 (High) | 100% (1.0) | 2.0 | $\frac{5000 \times 2.0 \times 1.0}{2.0} = \mathbf{5,000}$ | **#1 High Priority** |
| **B: Real-time Analytics Dashboard** | 1,200 | 3.0 (Massive) | 80% (0.8) | 4.0 | $\frac{1200 \times 3.0 \times 0.8}{4.0} = \mathbf{720}$ | **#3 Low Priority** |
| **C: Automated PDF Report Export** | 4,000 | 1.0 (Med) | 90% (0.9) | 1.5 | $\frac{4000 \times 1.0 \times 0.9}{1.5} = \mathbf{2,400}$ | **#2 Medium Priority** |

---

## 4. Best Practices for Execution
* **Standardize the Timeframe:** Ensure your **Reach** metric uses the exact same duration (e.g., monthly, quarterly) across all features being compared.
* **Kill the "Pet Projects":** If a low-value feature has high internal pressure from a stakeholder, run it through the RICE formula to visually show why it shouldn't jump the queue.
