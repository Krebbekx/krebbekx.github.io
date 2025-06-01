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

As pointed out in [2], the SRG has an intimate connection to the Nyquist diagram of a stable LTI system, and offers the same graphical interpretation of slope-restricted nonlinearities as the circle criterion. Our first work [3] shows how to apply SRG analysis to **unstable** LTI systems in the loop. A corollary of [3] is that SRG analysis fully reproduces the circle criterion, gives $L_2$-gain bounds, and generalizes the circle criterion by including dynamic nonlinearities.

Where [3] extends the range of applicability of SRG stability analysis by leveraging the Nyquist stability criterion, our second work [4] aims to extend the Bode diagram to NL systems. We leverage the property of incrementally stable systems that they preserve the periodicity of the input to compute **frequency-dependent gain bounds**. By plotting these bounds as magnitudes as function of frequency, one obtains a _nonlinear Bode plot_. These NL Bode plots can be made for open-loop and closed-loop systems, which allows for the definition of the corresponding _bandwidths_ as well. 

## References

[1] Ryu, Ernest K., Robert Hannah, and Wotao Yin. "Scaled relative graphs: Nonexpansive operators via 2D Euclidean geometry." _Mathematical Programming_ 194.1 (2022): 569-619.

[2] Chaffey, Thomas, Fulvio Forni, and Rodolphe Sepulchre. "Scaled relative graphs for system analysis." _2021 60th IEEE Conference on Decision and Control (CDC)._ IEEE, 2021.

[3] Krebbekx, J. P. J., Tóth, R., & Das, A. (2024). Scaled Relative Graph Analysis of Lur'e Systems and the Generalized Circle Criterion. arXiv preprint arXiv:2411.18318 ([arXiv link](https://arxiv.org/abs/2411.18318)). _Accepted for European Control Conference 2025._

[4] Krebbekx, J. P. J., Tóth, R., & Das, A. (2025). Nonlinear Bandwidth and Bode Diagrams based on Scaled Relative Graphs. arXiv preprint arXiv:2411.18318 ([arXiv link](https://arxiv.org/abs/2504.01585)). _Submitted for the 64th Conference on Decision and Control 2025._