---
layout: post
title: "Our paper on 3d human motion prediction was accepted at BMVC 2025"
date: 2025-07-26 00:12:10 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: Figure1.jpg # Add image post (optional)
---

I’m excited to announce that our paper, **“LuKAN: A Kolmogorov-Arnold Network Framework for 3D Human Motion Prediction”**, has been accepted at the **British Machine Vision Conference (BMVC) 2025**!

### About the Work

3D human motion prediction aims to forecast future poses from past motion sequences — a core challenge in fields like animation, human-computer interaction, and autonomous systems. Many existing methods struggle to balance accuracy and efficiency, often requiring deep or computationally heavy architectures.

Our proposed framework, **LuKAN**, addresses this by combining:

* **Kolmogorov-Arnold Networks (KANs)** with **Lucas polynomial activations** to efficiently capture temporal dependencies while mitigating spectral bias.
* **Discrete Wavelet Transform (DWT)** to encode both fine-grained and coarse motion dynamics, offering advantages over traditional DCT-based methods.
* **Spatial projections** to preserve inter-joint relationships and ensure structural consistency of the human body.

This design enables LuKAN to model both localized variations (like rapid hand gestures) and global trends (like walking cycles) while keeping the architecture lightweight.

### Key Results

* On **Human3.6M**, LuKAN achieved **state-of-the-art accuracy**, reducing Mean Per Joint Position Error (MPJPE) across multiple time horizons compared to strong baselines like SiMLPe.
* On **AMASS** and **3DPW**, LuKAN demonstrated **robust generalization**, particularly excelling in short-term predictions while maintaining strong long-term stability.
* An ablation study confirmed that **Lucas polynomials significantly outperform B-splines and other polynomial bases**, yielding up to **5.7% error reduction** at key horizons.

### Why It Matters

LuKAN shows that **compact, principled architectures** can rival or surpass heavy Transformer and GCN-based models in motion prediction. Its efficiency makes it well-suited for real-world applications where both accuracy and runtime matter.

### Next Steps

We’re excited to present this work at **BMVC 2025 in Sheffield, England** this November, share further insights with the community, and explore extensions of LuKAN to multi-person and more complex motion scenarios.

📄 Preprint: [ArXiv link](https://arxiv.org/abs/2508.04847)
💻 Code: [GitHub Repository](https://github.com/zadidhasan/LuKAN)

