---
layout: post
title: "Replication: Long-run Risk Model"
date: 2024-06-16
last_updated: 2024-06-16
description: This notes replicates the long-run risk model numerically.
giscus_comments: false
related_posts: false
---

**I gratefully thank the help of my supervisor [David Schreindorfer](https://www.davidschreindorfer.com/). The Python code was built based on the replication code in [Beason and Schreindorfer (2022)](https://www.journals.uchicago.edu/doi/10.1086/720396) and the Macro-finance lecture notes by David Schreindorfer at ASU. All faults are mine.**

The below code uses PyTorch to numerically replicates the long-run risk model and related papers. With cuda, the parallel computation highly speed up the matrix calculation.


{::nomarkdown}
{% assign jupyter_path = 'assets/jupyter/replication_long_run_risk_torch.ipynb' | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/blog.ipynb %}{% endcapture %}
{% if notebook_exists == 'true' %}
  {% jupyter_notebook jupyter_path %}
{% else %}
  <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}