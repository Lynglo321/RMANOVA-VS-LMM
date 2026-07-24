# RMANOVA-VS-LMM
# RMANOVA-VS-LMM

The why behind the use of **Linear Mixed Models (LMM)** compared to **Repeated Measures Analysis of Variance (RMANOVA)**.
> **Note:** This dataset is completely synthetic, contains no real human subject information, and does not violate HIPAA regulations.

## Project Overview
With a pilot sample of 10 individuals, this project uses LMM and RMANOVA to identify, assess, and determine the rationale behind the preference for LMM. It specifically explores how this choice affects our understanding of data progression for patients within a clinical trial.

## The "Two Bosses" Analogy
The practical distinctions between these two models can be likened to how two different bosses might audit their employees based on their attendance at work events:

*   **Boss 1 (RM-ANOVA):** Assesses employees by noting their presence at *every single event* he organizes. If an employee misses just one event, they are immediately fired (dropped from the assessment). 
    *   *The Result:* Boss 1 will likely lose a significant portion of his workforce, leading to a small sample size and severely weakening the statistical power of the overall team.
*   **Boss 2 (LMM):** Assesses employees by duly counting the events they *were* present for, while simply noting the ones they missed. 
    *   *The Result:* Boss 2 keeps his entire team intact for the final assessment because he doesn't eliminate anyone based on a single missing data point.

## Key Methodology Takeaways

*   **Handling Missing Data:** In RMANOVA, the process of exclusion is called **listwise deletion**, which completely deletes a participant's data if they miss a single event. LMM avoids this, conserving data collection and drastically reducing attrition losses.
*   **Point-Specific Estimates:** LMM can track specific, time-point estimates over time, whereas RMANOVA focuses primarily on the overall global effect.
*   **Covariance Flexibility:** LMM requires no rigid assumptions of covariance, providing the flexibility to choose the best-fitting model structure for your specific data (e.g., **AICC, CS, UN, AR(1)**).
