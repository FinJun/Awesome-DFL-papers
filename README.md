<div align="center">

# 🎯 Awesome Decision-Focused Learning

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/FinJun/Awesome-DFL-papers/graphs/commit-activity)

<img width="600" alt="DFL Pipeline" src="https://github.com/FinJun/Awesome-DFL-papers/assets/76249916/8e0ba391-af89-45cf-a2ea-155225bf9183">

**A curated list of Decision-Focused Learning (DFL) papers, code, and resources.**

*Bridging the gap between prediction and optimization.*

[Overview](#-overview) •
[Papers](#-papers) •
[Libraries](#-libraries--benchmarks) •
[Contributing](#-contributing)

</div>

---

## 📖 Overview

**Decision-Focused Learning (DFL)** is an emerging paradigm that integrates machine learning with downstream optimization tasks. Unlike traditional two-stage approaches that minimize prediction error, DFL directly minimizes **decision regret** — the suboptimality of decisions made using predicted parameters.

---

## 📚 Papers

### 📐 Differentiable Optimization Layers
*Embedding optimization problems as neural network layers with exact or approximate gradients.*

| Year | Venue | Paper | Keywords | Code |
|:----:|:-----:|:------|:--------:|:----:|
| 2017 | ICML | [OptNet: Differentiable Optimization as a Layer in Neural Networks](https://arxiv.org/pdf/1703.00443) | `QP` `KKT` | [![GitHub](https://img.shields.io/github/stars/locuslab/optnet?style=social)](https://github.com/locuslab/optnet) |
| 2020 | NeurIPS | [Interior Point Solving for LP-based prediction+optimisation](https://arxiv.org/pdf/2010.13943) | `LP` `Interior Point` | [![GitHub](https://img.shields.io/github/stars/JayMan91/NeurIPSIntopt?style=social)](https://github.com/JayMan91/NeurIPSIntopt) |
| 2024 | NeurIPS | [BPQP: A Differentiable Convex Optimization Framework for Efficient End-to-End Learning](https://arxiv.org/pdf/2411.19285) | `QP` `ADMM` `Efficient` | [![GitHub](https://img.shields.io/github/stars/jmp41/BPQP?style=social)](https://github.com/jmp41/BPQP) |
| 2025 | NeurIPS | [Differentiation Through Black-Box Quadratic Programming Solvers](https://arxiv.org/pdf/2410.06324) | `QP` `Black-box` `Modular` | [![GitHub](https://img.shields.io/github/stars/cwmagoon/dQP?style=social)](https://github.com/cwmagoon/dQP) |

### 📉 Surrogate Loss Methods
*Designing tractable loss functions that provide informative gradients for training.*

| Year | Venue | Paper | Keywords | Code |
|:----:|:-----:|:------|:--------:|:----:|
| 2017 | NeurIPS | [Task-based End-to-end Model Learning in Stochastic Optimization](https://arxiv.org/pdf/1706.02032) | `Stochastic` `End-to-End` | [![GitHub](https://img.shields.io/github/stars/locuslab/e2e-model-learning?style=social)](https://github.com/locuslab/e2e-model-learning) |
| 2019 | AAAI | [Melding the Data-Decisions Pipeline: Decision-Focused Learning for Combinatorial Optimization](https://arxiv.org/pdf/1809.05504) | `CO` `QP Smoothing` | [![GitHub](https://img.shields.io/github/stars/bwilder0/aaai_melding_code?style=social)](https://github.com/bwilder0/aaai_melding_code) |
| 2021 | Management Science | [Smart "Predict, then Optimize"](https://arxiv.org/abs/1710.08005) | `SPO+` `Convex Surrogate` | [![GitHub](https://img.shields.io/github/stars/paulgrigas/SmartPredictThenOptimize?style=social)](https://github.com/paulgrigas/SmartPredictThenOptimize) |
| 2021 | IJCAI | [Contrastive Losses and Solution Caching for Predict-and-Optimize](https://arxiv.org/pdf/2011.05354) | `NCE` `Caching` `Efficient` | - |
| 2022 | NeurIPS | [Decision-Focused Learning without Differentiable Optimization: Learning Locally Optimized Decision Losses](https://arxiv.org/pdf/2203.16067) | `LODL` `Learned Loss` | [![GitHub](https://img.shields.io/github/stars/sanketkshah/LODLs?style=social)](https://github.com/sanketkshah/LODLs) |
| 2024 | NeurIPS | [Decision-Focused Learning with Directional Gradients](https://arxiv.org/pdf/2402.03256) | `PG Loss` `Zeroth-order` | - |
| 2025 | NeurIPS | [Solver-Free Decision-Focused Learning for Linear Optimization Problems](https://arxiv.org/pdf/2505.22224) | `LAVA` `Solver-Free` | [![GitHub](https://img.shields.io/github/stars/ML-KULeuven/Solver-Free-DFL?style=social)](https://github.com/ML-KULeuven/Solver-Free-DFL) |
| 2025 | arXiv | [Minimizing Surrogate Losses for Decision-Focused Learning using Differentiable Optimization](https://arxiv.org/pdf/2508.11365) | `DYS-Net` `Surrogate` | - |

### 🎲 Perturbation & Gradient Approximation
*Using randomization or geometric insights to approximate gradients through discrete solvers.*

| Year | Venue | Paper | Keywords | Code |
|:----:|:-----:|:------|:--------:|:----:|
| 2020 | NeurIPS | [Learning with Differentiable Perturbed Optimizers](https://arxiv.org/pdf/2002.08676) | `PFYL` `Perturbation` `Fenchel-Young` | - |
| 2022 | ICML | [Decision-Focused Learning: Through the Lens of Learning to Rank](https://arxiv.org/pdf/2112.03609) | `LTR` `Ranking` | [![GitHub](https://img.shields.io/github/stars/jayman91/ltr-predopt?style=social)](https://github.com/jayman91/ltr-predopt) |
| 2023 | ICLR | [Backpropagation through Combinatorial Algorithms: Identity with Projection Works](https://arxiv.org/pdf/2205.15213) | `IWP` `Projection` `Simple` | [![GitHub](https://img.shields.io/github/stars/martius-lab/solver-differentiation-identity?style=social)](https://github.com/martius-lab/solver-differentiation-identity) |

### 📊 Surveys & Benchmarks

| Year | Venue | Paper | Description |
|:----:|:-----:|:------|:------------|
| 2024 | EJOR | [A Survey of Contextual Optimization Methods for Decision-Making under Uncertainty](https://arxiv.org/pdf/2306.10374) | Comprehensive survey covering DFL, contextual optimization, and stochastic programming |

---

## 🛠️ Libraries & Benchmarks

| Library | Description | Links |
|:--------|:------------|:-----:|
| **PyEPO** | PyTorch-based End-to-End Predict-then-Optimize Library | [![GitHub](https://img.shields.io/github/stars/khalil-research/PyEPO?style=social)](https://github.com/khalil-research/PyEPO) [![Paper](https://img.shields.io/badge/Math.%20Prog.%20Comp.-2024-blue)](https://arxiv.org/abs/2206.14234) |

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

**Ways to contribute:**
- 📝 Add new papers
- 🔗 Update links and code repositories  
- 📖 Improve descriptions
- 🐛 Report issues

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Made with ❤️ for the DFL community

</div>
