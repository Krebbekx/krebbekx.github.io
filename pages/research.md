---
layout: page
title: Research
---

# Motivation

My PhD project is about developing tools to _shape the performance of nonlinear control systems_. In the case of Linear and Time-Invariant (LTI) systems, characterizing stability is done in terms of poles/eigenvalues. Additionally, engineers have access to an intuitive description of the _performance_, or desired behavior, in terms of the frequency-domain. 

When systems are non-linear (NL), both the characterization of stability and the frequency-domain description of performance is lost. Most research on NL control systems focuses solely on _stability_, since this is often a very hard property to study. Therefore, the aspect of _performance_ is not even touched upon in most cases.

# My Work

The starting point of my work a set of tools that engineers use for LTI systems: the Bode and Nyquist diagram. Because of the unreasonable effectiveness of these tools in practice, my aim is to provide practical versions of these for NL systems. 

The main modern tool I use is the Scaled Relative Graph (SRG) [1], which can be seen as a generalization of the spectrum of an operator. Chaffey et al. [2] took notice of this development in monotone operator theory and applied it to the analysis of feedback systems. 

## Analysis of Unstable Systems

As pointed out in [2], the SRG has an intimate connection to the Nyquist diagram of a stable LTI system, and offers the same graphical interpretation of slope-restricted nonlinearities as the circle criterion. Our first work [3] shows how to apply SRG analysis to **unstable** LTI systems in the loop. A corollary of [3] is that SRG analysis fully reproduces the circle criterion, gives $L_2$-gain bounds, and generalizes the circle criterion by including dynamic nonlinearities.

The conference paper [3] is extended to a full journal paper in [4], where the analysis of unstable systems is extended to _arbitrary_ interconnections of systems, thus going beyond the Lur'e system which was the focus of [3]. Additionally, we show in [5] how the tools in [3] may be used to design reset/hybrid controllers for _unstable_ open-loop plants.

## Nonlinear Bode Diagrams and Frequency-Domain Analysis

Where [3],[4] extend the range of applicability of SRG stability analysis by leveraging the Nyquist stability criterion, our second work [6] aims to extend the Bode diagram to NL systems. We leverage the property that many nonlinear systems preserve the periodicity of the input to compute **frequency-dependent gain bounds**. By plotting these bounds as magnitudes as function of frequency, one obtains a _nonlinear Bode plot_. These NL Bode plots can be made for open-loop and closed-loop systems, which allows for the definition of the corresponding _bandwidths_ as well. 

## Multivariable Nonlinear Systems

From the control theory perspective, all works mentioned before [2-6] focus on systems with one input and one output. Extending the method to multivariable systems, also known as _Multiple-Input Multiple-Output_ (MIMO) systems, is not so hard in the square case, i.e. systems having the same amount of inputs as outputs. In the non-square case, however, it was not known how to do this at all. 

In our recent paper [7], we develop a complete and mathematically rigorous framework for non-approximative stability and $L_2$-gain analysis for multivariable nonlinear systems, which may be non-square. We develop both the incremental and non-incremental theory, where the former provides additional well-posedness guarantees. One can view [7] as a generalization of the internal stability, well-posedness and $H_\infty$-norm computations that form the cornerstone of modern robust control design.


## References

[1] Ryu, Ernest K., Robert Hannah, and Wotao Yin. "Scaled relative graphs: Nonexpansive operators via 2D Euclidean geometry." _Mathematical Programming_ 194.1 (2022): 569-619.

[2] Chaffey, Thomas, Fulvio Forni, and Rodolphe Sepulchre. "Scaled relative graphs for system analysis." _2021 60th IEEE Conference on Decision and Control (CDC)._ IEEE, 2021.

[3] Krebbekx, J. P. J., Tóth, R., & Das, A. (2024). Scaled Relative Graph Analysis of Lur'e Systems and the Generalized Circle Criterion. arXiv preprint arXiv:2411.18318 ([arXiv link](https://arxiv.org/abs/2411.18318)). _Accepted for European Control Conference 2025._

[4] Krebbekx, J. P. J., Tóth, R., & Das, A. (2025). "Scaled Relative Graph Analysis of General Interconnections of SISO Nonlinear Systems." arXiv preprint arXiv:2507.15564 ([arXiv link](https://arxiv.org/abs/2507.15564)).

[5] Krebbekx, J. P. J., Tóth, R., & Das, A. (2025). "Reset Controller Analysis and Design for Unstable Linear Plants using Scaled Relative Graphs." arXiv preprint arXiv:2506.13518 ([arXiv link](https://arxiv.org/abs/2506.13518v2)). _Submitted to Automatica as a technical communique._

[6] Krebbekx, J. P. J., Tóth, R., & Das, A. (2025). Nonlinear Bandwidth and Bode Diagrams based on Scaled Relative Graphs. arXiv preprint arXiv:2411.18318 ([arXiv link](https://arxiv.org/abs/2504.01585)). _Accepted for the 64th Conference on Decision and Control 2025._

[7] Krebbekx, J. P. J., Tóth, R., & Das, A. (2025). "Graphical Analysis of Nonlinear Multivariable Feedback Systems." arXiv preprint arXiv:2507.16513 ([arXiv link](https://arxiv.org/abs/2507.16513)). _Submitted to IEEE-TAC as a full paper._