# Revisiting Silhouette: From Micro to Macro Aggregation 

Silhouette coefficient is an established internal clustering evaluation measure that produces a score per data point, assessing the quality of its clustering assignment. To assess the quality of the clustering of the whole dataset, the scores of all the points in the dataset are typically (micro) averaged into a single value. An alternative path, however, that is rarely employed, is to average first at the cluster level and then (macro) average across clusters. As we illustrate in this work with a synthetic example, the typical **micro-averaging strategy is sensitive to cluster imbalance** while the overlooked macro-averaging strategy is far more robust. By investigating macro-Silhouette further, we find that uniform sub-sampling, the only available strategy in existing libraries, harms the measure's robustness against imbalance. We address this issue by **proposing a per-cluster sampling method**. An empirical analysis on eight real-world datasets in two clustering tasks reveals the disagreement between the two coefficients for imbalanced datasets.

![micro-sil increasing](https://arxiv.org/html/2401.05831v3/extracted/5685400/expanded_clusters.jpg)

---
The paper, presented at the 27th International Conference on Discovery Science 2024, Pisa, Italy, received the **Best Paper runner up** .

For a preprint, see: ([https://arxiv.org/abs/2401.05831](https://arxiv.org/abs/2401.05831)) and to cite us, please use the following:

```
@InProceedings{Pavlopoulos2024-revisiting,
  author="Pavlopoulos, John and Vardakas, Georgios and Likas, Aristidis",
  editor="Pedreschi, Dino and Monreale, Anna and Guidotti, Riccardo and Pellungrini, Roberto and Naretto, Francesca",
  title="Revisiting Silhouette Aggregation",
  booktitle="Discovery Science",
  year="2025",
  publisher="Springer Nature Switzerland",
  address="Cham",
  pages="354--368",
  isbn="978-3-031-78977-9"
}
```
---
Acknowledging Aggelos Semoglou for extending the work with [a composite Sihouette metric](https://github.com/semoglou/composite_silhouette), which is also available in PyPi. Install it using `pip install composite-silhouette` and import it in Python as:
```python
>>> from composite_silhouette import CompSil as composil
```
