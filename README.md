# topic-model-tutorial
This repository contains notebooks, slides, and data for the short tutorial *"Topic modelling with Scikit-learn"*, presented at [PyData Dublin](https://www.meetup.com/PyDataDublin/) in September 2017. 

### Contents

The summary tutorial is covered [in these slides](topic-modelling-with-scikitlearn.pdf). There are three associated IPython notebooks:

1. [Text Preprocessing](1%20-%20Text%20Preprocessing.ipynb): Provides a basic introduction to preprocessing documents with *scitkit-learn*.
2. [NMF Topic Models](2%20-%20NMF%20Topic%20Models.ipynb): Covers the application and interpretation of topic models via the NMF implementation provided by *scitkit-learn*.
3. [Parameter Selection for NMF](3%20-%20Parameter%20Selection%20for%20NMF.ipynb): More advanced material on selecting the number of topics for NMF, using topic coherence.

To demonstrate the topic modelling techniques, a sample dataset [is provided here](data/articles.txt). This consists of 4,551 news articles collected from the [Guardian News API](https://open-platform.theguardian.com) in 2016, stored in a single text file (25MB), with one article per line.

### Dependencies

This code has been tested with Python 3.6-3.8. The core package requirements are:

- *scikit-learn*
- *numpy*
- *matplotlib*

The model selection code also relies on the *gensim* package to build a Word2Vec model (tested with v4.1.2). A sample pre-built Word2Vec model for the sample dataset [is also provided here for download](http://erdos.ucd.ie/files/pydata/w2v-model.bin) (71MB).

### Links and References

- [*Scikit-learn* home](http://scikit-learn.org/stable/)
- [NMF documentation for *scikit-learn*](http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.NMF.html)
- Lee, D. D., & Seung, H. S. (1999). Learning the parts of objects by non-negative matrix factorization. Nature. [[Article]](https://www.nature.com/articles/44565)
- Blei, D. M. (2012). Probabilistic topic models. Communications of the ACM, 55(4). [[Article]](https://cacm.acm.org/magazines/2012/4/147361-probabilistic-topic-models/fulltext)
- O’Callaghan, D., Greene, D., Carthy, J., & Cunningham, P. (2015). An analysis of the coherence of descriptors in topic modeling. Expert Systems with Applications. [[PDF]](http://derekgreene.com/papers/ocallaghan15eswa.pdf)
