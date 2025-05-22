---
layout: default
title: Datasets
---

# Datasets

Below are the available datasets on spin-dependent exotic interactions:

{% for dataset in site.data.datasets %}
## {{ dataset.title }}

**Description:** {{ dataset.description }}

**Data:** [{{ dataset.data_link_text }}]({{ dataset.data_link }})

**Interactive Plot:** [View Plot]({{ dataset.plot_link }})

---

{% endfor %}
