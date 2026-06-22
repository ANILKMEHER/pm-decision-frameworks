# Fishbone (Ishikawa) Diagram Framework 🐟

## 1. What is it?
The Fishbone Diagram (or Cause-and-Effect Diagram) is a visual root-cause analysis tool used to brainstorm, categorize, and identify the potential causes of a specific, complex problem. It prevents teams from focusing on symptoms and forces them to look at systemic issues.

## 2. The 6 Ms Structure
The problem (or "Effect") is placed at the head of the fish, and potential causes are branched out across six categories:
1.  **Manpower (People):** Gaps in training, fatigue, communication silos, or human error.
2.  **Machine (Technology):** Server downtime, software bugs, outdated hardware, or tool constraints.
3.  **Method (Process):** Inadequate workflows, rigid release cycles, or lack of standard operating procedures (SOPs).
4.  **Material (Data/Resources):** Poor data quality, third-party API dependencies, or missing documentation.
5.  **Measurement (Metrics):** Flawed KPIs, lack of real-time monitoring, or incorrect telemetry data.
6.  **Milieu / Mother Nature (Environment):** Organizational culture shifts, sudden market volatility, or physical workspace challenges.

---

## 3. Real-World Application Example
### Problem Statement (The Fish Head): High-Stakes System Deployment Delayed by 48 Hours

```text
  MANPOWER               MACHINE                 METHOD
  (Skill Gaps)      (API Rate Limits)       (Fragile SOPs)
       \                    \                    /
        \                    \                  /
---------\--------------------\----------------/---------> [ 48-Hour Deployment Delay ]
         /                    /                \
        /                    /                  \
       /                    /                    \
  MATERIAL              MEASUREMENT             MILIEU
(Bad Config Data)    (No Pre-alert System)   (Time-zone Silos)
