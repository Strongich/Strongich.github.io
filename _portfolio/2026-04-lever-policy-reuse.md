---
title: "LEVER: Inference-Time Policy Reuse under Support Constraints"
header:
  link: "https://arxiv.org/abs/2604.20174"
excerpt: "RAI for Ukraine research project on offline reinforcement learning policy reuse. Preprint available on arXiv; code released on GitHub.<br/><img src='/images/portfolio/lever.png' alt='LEVER framework overview.'>"
collection: portfolio
---

This work was conducted during my Research Fellow appointment in the RAI for Ukraine program at the Center for Responsible AI at New York University.

**Preprint:** Vitenko I., et al. "[LEVER: Inference-Time Policy Reuse under Support Constraints](https://arxiv.org/abs/2604.20174)." arXiv, 2026.  
**Code:** The implementation is available in the [LEVER GitHub repository](https://github.com/Strongich/LEVER).

LEVER studies inference-time reuse of reinforcement learning policies: given a library of pretrained policies and a new composite objective, the framework constructs a policy offline, without additional environment interaction. The method retrieves relevant policies from metadata, evaluates candidates with behavioral embeddings, and composes policies through offline Q-value composition.

The paper focuses on the support-limited regime, where value propagation is unavailable and reuse quality depends on transition coverage in the policy library. In deterministic GridWorld experiments, LEVER can match or exceed training-from-scratch performance while reducing computation time, but performance degrades when long-horizon dependencies require propagation beyond the available support.
