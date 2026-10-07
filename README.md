# Learning an Interpretable Traffic Signal Control Policy

**Deep Reinforcement Learning – Assignment 1**
**Group:** 100

## Group Members

| Name | BITS ID |
|---|---|
| Guduru Sai Deepthi | 2025ag05517 |
| Souhardya Sengupta | 2025ag05033 |
| Sourav Bhattacharya | 2025ag05188 |
| S. Ameer Deen | 2025ag05037 |

## Paper

Ault, J., Hanna, J. P., and Sharon, G. (2020).
**Learning an Interpretable Traffic Signal Control Policy.**

Paper: https://arxiv.org/pdf/1912.11023

## Summary
- **Problem:** Deep RL cuts signal delay by up to 73%, but DNN controllers are unexplainable. Transportation agencies need controllers that are interpretable and legally auditable.
- **Approach:** A monotonic, regulatable precedence function. It uses 6 lane-level traffic variables and 4 clearance flags, with tunable weights and exponents. It is trained offline from a DQN "teacher" using DRQ, DRSQ and DRHQ.
- **Results:** Tested in SUMO on Utah DOT data (State St & E 4500 S, Murray). DRHQ and DRSQ beat PPO and CMA-ES, and DRHQ cuts delay by up to 19.4% versus actuated control.
- **Limitations / future work:** Results are simulation-only. Safe "Day One" exploration needs warm-starting, and the method still has to scale to coordinated city-wide networks.
  
