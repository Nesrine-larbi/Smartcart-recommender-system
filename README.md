# SmartCart — AI Recommendation Engine

**Instructor:** Dr. Reza Mirsalari  
**Team:**
- Mehrad Mostaan (40248205)
- Nesrine Larbi (40079009)
- Mymanat Mohammed (40298076)
- Alessandro TingYi Lorigiano (40017756)

---

## Overview

SmartCart is a Python-based e-commerce recommendation system with three parts:

- **Part 1 — Preprocessing:** Clean data and build a user–item rating matrix
- **Part 2 — Collaborative Filtering:** Recommend products using user-based cosine similarity
- **Part 3 — Association Rule Mining:** Find frequent product combinations using Apriori

---

## Setup

```bash
pip install pandas numpy scikit-learn matplotlib seaborn mlxtend
```

---

## How to Run

**Recommended — run all parts at once:**

```bash
jupyter notebook smartcart_complete.ipynb
```

Run all cells top to bottom. `ecommerce_user_data.csv` and `product_details.csv` must be in the same folder.

**Alternatively — run parts separately (Part 1 must go first):**

```bash
jupyter notebook "part1_preprocessing (1).ipynb"
jupyter notebook part2_collaborative_filtering.ipynb
jupyter notebook "part3_association_rule_mining_apriori_final(1).ipynb"
```

---

## File Structure

```
├── ecommerce_user_data.csv                          # Input: user–product ratings
├── product_details.csv                              # Input: product metadata
├── smartcart_complete.ipynb                         # Main notebook (all 3 parts)
├── part1_preprocessing (1).ipynb                   # Part 1 standalone
├── part2_collaborative_filtering.ipynb             # Part 2 standalone
├── part3_association_rule_mining_apriori_final(1).ipynb  # Part 3 standalone
└── README.md
```

---

## Outputs

All files below are generated automatically when the notebook runs:

| File | Part | Description |
|------|------|-------------|
| `user_data_clean.csv` | 1 | Cleaned interaction log |
| `user_item_matrix.csv` | 1 | 50×100 user–item rating matrix |
| `user_category_agg.csv` | 1 | Ratings aggregated by user and category |
| `recommendations_top5.csv` | 2 | Top-5 recommendations per user |
| `part3_frequent_itemsets.csv` | 3 | Frequent itemsets with support values |
| `part3_association_rules.csv` | 3 | Rules with support, confidence, and lift |
| `part1_eda_plots.png` | 1 | Rating and category distribution charts |
| `part2_similarity_heatmap.png` | 2 | User–user cosine similarity heatmap |
| `part2_evaluation_metrics.png` | 2 | Precision / Recall / MAP bar chart |
| `part2_summary_table.png` | 2 | Full evaluation summary |
