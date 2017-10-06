# Dimension Reduction Comparison
After noticing that the ICA transformation of data seems to shift the null to the left in a permutation test using in-house data,
The effect was replicated using the Haxby dataset.

Here we compare the results of a support vector classifier (faces vs. houses) on data that has been transformed using PCA, ICA,
Factor Analysis, and Dictionary learning. The results of the true classification are generally comprable across all 6 subjects.
Shuffled k-folds seems to lead to better classification rates generally.

On non-shuffled k-fold PCA has the lowest classification rate on 4/6 subjects and dictionary learning produces the lowest on 2/6 
subjects. During the Shuffled K-fold ICA performs the lowest on 3/6, PCA on 2/6, and Dictionary learning on 1/6.

On non-shuffled k-fold validation ICa performs the best on 4/6 subjects, Factor Analysis data performs the best on 1/6 subjects,
and ICA and PCA have the same scores for one subject. On shuffled validations each transformation performs the best in at least
one case except for PCA.

More notably during the permutation test the empirical null of the ICA transformed data seems to have shifted to the left of what
should be chance. I do not know why this is. I do not know whether this effects the non-permuted classification.
