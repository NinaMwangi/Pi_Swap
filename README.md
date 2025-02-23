# Pi_Swap

##Problem Statement
The rising cost of living, poor economic conditions, and limited resources have necessitated the need for a more sustainable and affordable way of acquiring school-going children’s books. The current second-hand market has tried to bridge the gap however, the existing platforms and traditional markets have fallen short due to factors such as accessibility and trust.

## Dataset
The dataset used is from the current KLB approved book list from pre primary level to tertiary level.
https://drive.google.com/file/d/1hTpUvFbw0KyMOB89QHiLhoYj0uD3XlGY/view?usp=share_link

## Models
The Notebook contains recommender based system models.
1. Collaborative filtering
2. Hybrid (Collaborative filtering & Content based)

# Evaluation
The performance is measured using:
1. RMSE
2. Precison@k
3. Recall@k

# Table
## 📊 Model Performance Comparison

| Training Instance | Model                   | Similarity Metric        | Weight Balancing                                | Truncated SVD | Top K | RMSE  | Precision@K | Recall@K |
|------------------|------------------------|-------------------------|------------------------------------------------|--------------|------|------|-------------|----------|
| Instance 1      | Collaborative Filtering | Cosine Similarity       | -                                              | -            | 5    | 0    | 0.0023      | 0.0116   |
| Instance 2      | Collaborative Filtering | Pearson                 | -                                              | -            | 10   | 0    | 0.0023      | 0.0116   |
| Instance 3      | Hybrid                  | Cosine & Pearson        | content_weight - 0.4, cf_weight - 0.4, svd_weight - 0.2 | 100          | -    | 0.2451 | 0.0047      | 0.0349   |


# Video Recording
https://drive.google.com/file/d/1YudrbLSqrS19COvHd1tWzLVGfkeMwfZE/view?usp=sharing
