# Multilabel-Classification

In multi-label classification1 problems instances can belong to more than one class at a time. The task here is to implement a selection of multi-label classification approaches with the help of scikit-learn base estimator implementation.

For all of the tasks we will use the Yeast dataset2. The Yeast dataset is formed by micro-array expression data and phylogenetic pro-files with 2,417 included. There are 103 descriptive features per gene. Each gene is associated with a set of functional classes. In this version of the dataset there are 14 functional classes and a gene can be associated with any number of these.

The simplest approach to multi-label classification is the binary relevance algorithm in which individual binary base classifiers are implemented for each label. This uses a one-vs-all approach to generate the training sets for each base classifier. Implement the binary relevance algorithm. Allow the base classifier type to be set as a parameter to this algorithm.

One of the criticisms of the simple binary relevance classifier approach is that it does not take advantage of associations between labels in a multi- label classification scenario. The classifier chain algorithm is an effective multi-label classification algorithm that takes advantage of label associations. A classifier chain model generates a chain of binary classifiers each of predicts the presence or absence of a specific label. The in input to each classifier in the chain, however, includes the original descriptive features plus the outputs of the classifiers so far in the chain. This allows label associations to be taken into account. 
