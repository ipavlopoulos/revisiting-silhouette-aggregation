# Revisiting Silhouette: From Micro to Macro Aggregation 

Silhouette coefficient is an established internal clustering evaluation measure that produces a score per data point, assessing the quality of its clustering assignment. To assess the quality of the clustering of the whole dataset, the scores of all the points in the dataset are typically (micro) averaged into a single value. An alternative path, however, that is rarely employed, is to average first at the cluster level and then (macro) average across clusters. As we illustrate in this work with a synthetic example, the typical **micro-averaging strategy is sensitive to cluster imbalance** while the overlooked macro-averaging strategy is far more robust. By investigating macro-Silhouette further, we find that uniform sub-sampling, the only available strategy in existing libraries, harms the measure’s robustness against imbalance. We address this issue by **proposing a per-cluster sampling method**. An experimental study on eight real-world datasets is then used to analyse both coefficients in two clustering tasks.

![micro-sil increasing](https://arxiv.org/html/2401.05831v3/extracted/5685400/expanded_clusters.jpg)

---
The paper, presented at the 27th International Conference on Discovery Science 2024, Pisa, Italy, received the Best Paper runner up.

A preprint exists ([https://arxiv.org/abs/2401.05831](https://arxiv.org/abs/2401.05831)), which you can cite as:

```
@article{pavlopoulos2024revisiting,
  title={Revisiting Silhouette Aggregation},
  author={Pavlopoulos, John and Vardakas, Georgios and Likas, Aristidis},
  journal={arXiv e-prints},
  pages={arXiv--2401},
  year={2024}
}
```
