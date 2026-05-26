# Causal Inference with DoWhy

This project demonstrates how to use Microsoft's **DoWhy** library to isolate a true causal effect in the presence of confounding bias. 

## The Causal Problem
We simulate a classic data science challenge: evaluating the impact of a **Job Training Program (Treatment)** on **Income (Outcome)**, where an individual's **Socioeconomic Background (Confounder)** influences both participation and earnings. 

Standard statistical models or naive regressions suffer from confounding bias. This project utilizes **Propensity Score Stratification** to remove the bias and accurately estimate the true causal effect.

## Project Structure
* `causal_analysis.ipynb`: The core Jupyter Notebook containing data generation, effect identification, estimation, and robustness refutation.
* `requirements.txt`: Environment dependencies.

## DoWhy's 4-Step Framework
1. **Model**: Formulate the causal graph (DAG).
2. **Identify**: Determine the backdoor or frontdoor statistical recipe.
3. **Estimate**: Calculate the causal effect value using propensity scores.
4. **Refute**: Stress-test the estimate using a *Random Common Cause* refutation method.

## Getting Started

1. Clone the repository:
   ```bash
   git clone [https://github.com/celikumit/causal-inference-dowhy.git](https://github.com/celikumit/causal-inference-dowhy.git)
   cd causal-inference-dowhy