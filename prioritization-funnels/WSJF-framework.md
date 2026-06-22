# Weighted Shortest Job First (WSJF) Framework ⏱️

## 1. What is it?
WSJF is a prioritization model used in Agile and Scaled Agile Frameworks (SAFe) to sequence a backlog of features or initiatives. Instead of prioritizing based on who shouts the loudest, WSJF calculates an economic score based on the **Cost of Delay (CoD)** and the **Job Size/Duration**. 

The fundamental rule of WSJF is: **If two features provide equal value, do the shorter one first. If they take the same time, do the higher-value one first.**

## 2. The Formula & Components

$$WSJF = \frac{Cost\ of\ Delay\ (CoD)}{Job\ Size}$$

Where **Cost of Delay (CoD)** is the sum of three distinct variables:
1. **User-Business Value:** Relative value to the customer or business (e.g., revenue impact, operational savings).
2. **Time Criticality:** Does the value decay over time? Is there a fixed milestone, legal deadline, or immediate competitor threat?
3. **Risk Reduction or Opportunity Enablement:** Does this feature mitigate a technical/business risk or open up new business opportunities?

*Note: All components (including Job Size) are typically scored relatively using a modified Fibonacci sequence (1, 2, 3, 5, 8, 13, 20).*

---

## 3. Real-World Application Example
### Scenario: Sequencing Enterprise Architecture and Technical Migration Features

| Feature Name | User-Biz Value | Time Criticality | Risk Reduc. / Opp. Enable. | Total Cost of Delay (CoD) | Job Size | WSJF Score | Priority Sequence |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **A: Fix Cloud Security Compliance Gap** | 5 | 13 | 13 | 5 + 13 + 13 = **31** | 2 | $\frac{31}{2} = \mathbf{15.5}$ | **#1 (Do First)** |
| **B: Automated VM Backup Infrastructure** | 8 | 3 | 5 | 8 + 3 + 5 = **16** | 3 | $\frac{16}{3} = \mathbf{5.33}$ | **#2 (Do Second)** |
| **C: Next-Gen Analytics UI Overhaul** | 13 | 2 | 2 | 13 + 2 + 2 = **17** | 8 | $\frac{17}{8} = \mathbf{2.12}$ | **#3 (Do Third)** |

### Insights from the Matrix:
Even though **Feature C** has the highest raw customer value (13), it takes a long time to build (Job Size = 8). **Feature A** is highly time-critical and drastically reduces compliance risk while being a small task to build (Job Size = 2), giving it a massive WSJF score. It jumps to the front of the queue to maximize economic return.

---

## 4. Best Practices for Execution
* **Score Column by Column:** When facilitating a prioritization meeting, score the entire backlog for "User-Business Value" first, then move to "Time Criticality." This prevents teams from anchoring their scores based on a single favorite feature.
* **Use "Job Size" as a Proxy for Effort:** You don't need exact hours or story points. Relative sizing against a known baseline feature is enough to generate an accurate WSJF sequence.
