# NLP_60k

Notebooks run based on local path (it should be the github repo one for local runs)
### A Baseline? 
* [word2vec-umap.ipynb](https://github.com/MachineLearningJournalClub/NLP_60k/blob/main/word2vec-umap.ipynb) : Using pretrained w2v for features extraction + UMAP for visualization purposes; Basic regression (with Gradient Boosting Regression), validation MSE = 0.44 
  * ToDos: K-Fold Cross Validation, W2V vectors augmentation (I'd give a try by applying small perturbations on the training set :) ), smart way to use the *std*, Ensembling several word embedding algos (W2V + GloVe + FastText) 
