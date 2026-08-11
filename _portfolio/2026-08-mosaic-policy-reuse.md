---
title: "When Can Pre-Trained Policies Be Reused? Inference-Time Policy Composition from Fixed Policy Libraries"
header:
  link: "https://arxiv.org/abs/2604.20174"
excerpt: "My project as part of the RAI for Ukraine program got accepted to the CIKM 2026 Short Paper Track — inference-time policy reuse in offline reinforcement learning. Extended version available on arXiv; code released on GitHub.<br/><img src='/images/portfolio/CIMK26_solo_scritta.png' alt='CIKM 2026 logo.' style='width:48.7%;max-width:100%;'>"
collection: portfolio
---

This work was conducted during my Research Fellow appointment in the RAI for Ukraine program at the Center for Responsible AI at New York University.

**Paper:** Vitenko I., Ibrahim N., Amer-Yahia S. "When Can Pre-Trained Policies Be Reused? Inference-Time Policy Composition from Fixed Policy Libraries." *CIKM 2026, Short Paper Track.*  
**Extended version:** "[LEVER: Inference-Time Policy Reuse under Support Constraints](https://arxiv.org/abs/2604.20174)." arXiv, 2026.  
**Code:** The implementation is available in the [MOSAIC GitHub repository](https://github.com/Strongich/MOSAIC).

MOSAIC studies inference-time reuse of reinforcement learning policies: given a library of pretrained policies and a new composite objective, the framework constructs a policy offline, without additional environment interaction. The method retrieves relevant policies from metadata, evaluates candidates with behavioral embeddings, and composes policies through offline Q-value composition.

The paper focuses on the support-limited regime, where value propagation is unavailable and reuse quality depends on transition coverage in the policy library. In deterministic GridWorld experiments, MOSAIC can match or exceed training-from-scratch performance while reducing computation time, but performance degrades when long-horizon dependencies require propagation beyond the available support.
