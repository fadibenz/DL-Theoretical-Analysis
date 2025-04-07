# DL-Theoretical-Analysis

This is a meta-repository that includes theoratical experiments on various techniques widely used in deep learning, the analysis is mathematically rigorous and followed by empirical testing. This provides a very deep understanding of these techniques and gave me a better understanding on how ML research is conducted.

## 📌 Table of Contents
- [Momentum acceleration in Linear Regression](#momentum-acceleration-in-linear-regression)
- [Dropout in Linear regression is a ridge regularization](#dropout-in-linear-regression-is-a-ridge-regularization)
- [How Does Pruning Work](#how-does-pruning-work)
---

## 📈 Techniques & Analysis:

### Momentum acceleration in Linear Regression:

- 📂 **Project Repo:** [Momentum Accelaration](https://github.com/fadibenz/Momentum-Experimentation)
- 📝 **Description:** This is an in-depth analysis of Momentum in Linear regression, it shows how Momentum allows for bigger learning rates in ill-conditioned problems, this is done by analyzing the **eigenvalues of the dynamic system** that governs gradient updates,  the findings here can be transcribed loosely to Neural Nets using the **Generalized Linear Model** View. It also shows that Momentum accelerates convergence optimally when it places eigenvalues in the complex/repeated regime.

---

### Dropout in Linear regression is a ridge regularization:

- 📂 **Project Repo:** [Dropout as a regularizer](https://github.com/fadibenz/Dropout-InDepth)
- 📝 **Description:**  Main take was how  Dropout in addition to normalizing the design matrix, leads to solving a regularized least-squares instead of $OLS$, so there's a form of double-regularization, one stemming from the normalization of the matrix (and its effects on the loss-landscape and the magnitude of singular values) and the other from the added ridge-regularization (the constant $\lambda$ regularizes the inverse of the singular values even further).

---

### How Does Pruning Work:

- 📂 **Project Repo:** [Pruning](https://github.com/fadibenz/Pruning)
- 📝 **Description:**  This notebbok goes through implementing both fine-grained and channel prunning from scratch to understand the mechanics and includes a small comaparision between the two, in addition to a philosophical understanding of how fine-grained pruning can lead to regularization by amplyfying the implicit bias of GD.
---
