# Introduction to Deep Equilibrium Nets (DEQNs)

**A Mini-Course — March 2026**

## Description

This self-contained mini-course introduces **Deep Equilibrium Nets (DEQNs)**, a method that uses deep neural networks to solve high-dimensional dynamic stochastic economic models. DEQNs replace traditional grid-based collocation with neural network training, where the loss function is derived directly from the economic equilibrium conditions — no labeled data is needed.

The course covers the necessary ML/DL foundations, develops the DEQN methodology from scratch, applies it to the Brock–Mirman benchmark (which has an analytical solution), scales it up to the multi-country International Real Business Cycle (IRBC) model, and introduces practical tools such as Neural Architecture Search and loss normalization (ReLoBRaLo).

## Prerequisites

- Basic knowledge of macroeconomics (Euler equations, dynamic programming)
- Familiarity with Python and Jupyter notebooks
- Linear algebra and calculus fundamentals

## Software Requirements

| Package | Version |
|---|---|
| Python | >= 3.9 |
| NumPy | >= 1.24 |
| SciPy | >= 1.10 |
| Matplotlib | >= 3.7 |
| TensorFlow | >= 2.15 |
| TensorFlow Probability | >= 0.23 |
| PyTorch | >= 2.0 |

Install all dependencies via:
```bash
pip install -r requirements.txt
```

## Course Content

The slide deck (`slides/DEQN_MiniCourse.tex`) is organized as follows:

| Part | Topic | Content |
|---|---|---|
| I | ML/DL Foundations | DNNs as function approximators, activation functions, SGD, loss functions |
| II | Deep Equilibrium Nets | Motivation, curse of dimensionality, DEQN loss function, training algorithm |
| III | Brock–Mirman Benchmark | Analytical test case, DEQN implementation, parallelization & scalability |
| IV | Practical Tools | Neural Architecture Search (NAS) and ReLoBRaLo loss normalization |
| V | Scaling Up — The IRBC Model | Multi-country model, equilibrium system, high-dimensional DEQNs |
| VI | Hands-on Exercises | Notebook overview and suggested readings |

## Code Notebooks

| Notebook | Description |
|---|---|
| `code/01_Brock_Mirman_1972_DEQN.ipynb` | Deterministic Brock–Mirman model with analytical benchmark |
| `code/02_Brock_Mirman_Uncertainty_DEQN.ipynb` | Stochastic Brock–Mirman with TFP shocks |
| `code/03_DEQN_Exercises_Blancs.ipynb` | Exercise problems (blanks to fill in) |
| `code/03_DEQN_Exercises_Solutions.ipynb` | Exercise solutions |
| `code/04_IRBC_DEQN.ipynb` | Full IRBC model: multi-country DEQN with adjustment costs and irreversibility |

## Readings

| Paper | File |
|---|---|
| Azinovic, Gaegauf & Scheidegger (2022). *Deep Equilibrium Nets.* International Economic Review 63(4), 1471–1525. | `readings/Azinovic_Gaegauf_Scheidegger_2022_DEQN.pdf` |
| Fernández-Villaverde, Nuño & Perla (2024). *Taming the Curse of Dimensionality: Quantitative Economics with Deep Learning.* NBER Working Paper 33117. | `readings/taming.pdf` |
| Chen, Didisheim & Scheidegger (2026). *Deep Surrogates for Finance: With an Application to Option Pricing.* Journal of Financial Economics 177, 104222. | `readings/DeepSurrogates_JFE.pdf` |
| Friedl, Kübler, Scheidegger & Usui (2023). *Deep Uncertainty Quantification: With an Application to Integrated Assessment Models.* Working paper. | `readings/DeepUQ_with_an_application_to_IAM.pdf` |

## References

If you use materials from this course, please cite:

```bibtex
@article{azinovic2022deep,
  title={Deep Equilibrium Nets},
  author={Azinovic, Marina and Gaegauf, Luca and Scheidegger, Simon},
  journal={International Economic Review},
  volume={63},
  number={4},
  pages={1471--1525},
  year={2022},
  doi={10.1111/iere.12575}
}
```

## Lecturers

**Simon Scheidegger**
HEC, University of Lausanne
[https://sites.google.com/site/simonscheidegger/](https://sites.google.com/site/simonscheidegger/)

**Galo Nuño**
Banco de España
[https://www.galonuno.com/](https://www.galonuno.com/)

## License

This work is licensed under [CC0 1.0 Universal](LICENCE).
