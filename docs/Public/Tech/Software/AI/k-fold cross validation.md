*K-fold cross validation* is a technique to assess the performance of a [[machine learning]] model; specifically, comparing models and to prevent overfitting. It involves partitioning a [[dataset]] into $k$ equal-sized *folds* or subsets ([[subset]]). 

The model is trained and evaluated $k$ times, using a different fold for evaluation each time while the remaining $k-1$ folds are used for training. Each *fold* contains approximately the same proportion of [[data]] points, preserving how these points are spread. 

The performance metric is averaged across all iterations into a single estimate - how well the model generalizes to unseen data. 