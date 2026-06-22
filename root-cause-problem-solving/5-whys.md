# The 5 Whys Methodology 🎯

## 1. What is it?
The 5 Whys is an iterative interrogative technique used to explore the cause-and-effect relationships underlying a specific problem. By repeatedly asking the question "Why?", you peel away layers of immediate symptoms to uncover the ultimate root cause of a process or systemic failure.

## 2. Core Framework
1. **Define the Problem:** Clearly state the specific issue (the anomaly or failure event).
2. **Ask "Why?" Five Times:** For each answer you get, ask "Why did that happen?" to uncover the next layer.
3. **Stop at the Root:** "Five" is a general rule of thumb. Stop when asking "Why" no longer yields actionable insights, usually pointing to a broken process, policy, or system structure.
4. **Implement Countermeasures:** Design a permanent solution to fix the root cause, rather than just patching the immediate symptom.

---

## 3. Real-World Application Example
### Problem Statement: A critical automated database backup failed to execute during a weekend maintenance window.

* **Why 1?** Why did the backup fail?
    * *Because the target virtual machine running the backup script ran out of disk storage space.*
* **Why 2?** Why did the virtual machine run out of disk storage space?
    * *Because a massive volume of unpurged activity logs accumulated over the past quarter.*
* **Why 3?** Why were the old activity logs unpurged?
    * *Because the automated cleanup cron job script had silently stopped running.*
* **Why 4?** Why did the automated cleanup cron job stop running?
    * *Because a recent server migration modified the system directory pathing, breaking the script's execution path.*
* **Why 5?** Why was the script path broken without anyone noticing during the migration?
    * *Because the infrastructure migration runbook lacked a validation step to test and verify cron job success post-migration.* **(Root Cause)**

### Resolution / Countermeasure:
Instead of just clearing space on the server (fixing the symptom), update the central migration runbook framework to mandate automated automated validation tests for all background processes and scheduled tasks before cutover completion.

---

## 4. Best Practices for Execution
* **People vs. Process:** Avoid blaming people (e.g., *"Why? Because Anil forgot"*). Focus on the underlying process flaw that allowed the human error to occur (e.g., *"Why? Because there was no automated validation check in place"*).
* **Trace the Logic:** Ensure there is a clear, unbroken line of cause-and-effect when reading the chain from bottom to top using "Therefore" statements.
