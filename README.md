# NLP_60k

Notebooks run based on local path (it should be the github repo one for local runs)
### A Baseline? 
* [word2vec-umap.ipynb](https://github.com/MachineLearningJournalClub/NLP_60k/blob/main/word2vec-umap.ipynb) : Using pretrained w2v for features extraction + UMAP for visualization purposes; Basic regression (with Gradient Boosting Regression), validation MSE = 0.44 
  * ToDos: K-Fold Cross Validation, W2V vectors augmentation (I'd give a try by applying small perturbations on the training set :) ), smart way to use the *std*, Ensembling several word embedding algos (W2V + GloVe + FastText) 

### Limits of statistical features
By using only informations about the number of the words, their length, and similar things about the sentences or the text as a whole does not make a decent result: RMSE is about 0.81 in most cases, even using a minimal amount of augmentation. However it could be useful to further boost more advanced models. Time will tell :)

### Proposed approaches

* From a rapid look at the data, it seems that the most readable texts talk about well known (by a kid) things in a simple way (for example: dinosaurs), while the least readable one are about highly techinical subjects (such as metalworking), with a lot of technical words in the text (which of course will be hard to read for a kid). This suggests two approaches: the first one is to select the argument(s) of the text as an extra training variable (maybe spacy + W2V), the second one is to estimate the frequency of words in a large corpora of WELL BALANCED text and look for those words that are higly specilized and unusual (maybe accounting also for the intrinsic "intensione (vedi 'Il software del linguaggio' di R. Simone)
