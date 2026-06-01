# Spatial-Optimization-Models-for-Indoor-Autonomous-Logistics. Thesis Chapter 2 

This repository provides the Python implementation for the numerical study and visual results of **Chapter 2** of the PhD dissertation: *"Optimal Spatial and Temporal Decisions under Uncertainty"* (McMaster University, 2026).

## Abstract
Chapter 2 develops a unified spatial-temporal framework for locating an Autonomous Robot Hub in a multi-floor building. It integrates horizontal travel, vertical displacement, and elevator queuing delays. We prove that the optimal horizontal coordinates follow the **Scaled Gravity Center** result:
$$\hat{a}_k = p_k \mathbb{E}[X], \quad \hat{b}_k = p_k \mathbb{E}[Y]$$
Where $p_k$ is the demand probability on floor $k$.

## Key Features
- **Convexity Verification:** Automated check for discrete convexity to ensure the local sign test identifies the global optimum.
- **Sensitivity Analysis:** Visualizes how arrival rates ($\Lambda$) and vertical speeds influence the optimal hub floor ($c^*$).
- **Benchmark Comparison:** Compares the integrated model against the "Highest-Peak" heuristic (anchoring at max demand) and "Distance-Only" policies.

## Visualizations
The included script generates:
1. **Vertical Demand Profiles:** Symmetric vs. Top-Heavy archetypes.
2. **$\mathcal{H}(k)$ Cost Curves:** Highlighting the global minimum across various regimes.
3. **Convexity Failures:** Demonstrating how global convexity can fail in spatial-dominated regimes (e.g., extremely high $\kappa_t/v_1$).
4. **Efficiency Gains:** Shaded area plots showing avoidable costs eliminated by the integrated framework.

## Usage
Ensure you have `numpy` and `matplotlib` installed. 
