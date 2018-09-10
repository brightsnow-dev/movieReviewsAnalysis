## Movie Review Analysis

An analysis of the `movie_review` data set included in the `nltk` corpus. I would probably add some buzz words here later on.

***

## Index:

- [What is in this repo](https://github.com/prodicus/movieReviewsAnalysis#what-is-in-this-repo)
    - [Accuracy achieved](https://github.com/prodicus/movieReviewsAnalysis#accuracy-achieved)
- [Requirements](https://github.com/prodicus/movieReviewsAnalysis#requirements)
    - [Downloading the dataset](https://github.com/prodicus/movieReviewsAnalysis#downloading-the-dataset)
- [Running it](https://github.com/prodicus/movieReviewsAnalysis#running-it)
- [So](https://github.com/prodicus/movieReviewsAnalysis#so)
- [Legal stuff](https://github.com/prodicus/movieReviewsAnalysis#legal-stuff)

***

## What is in this repo
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

- [x] An implementation of `nltk.NaiveBayesClassifier` trained against **5000 movie reviews**. Implemented in `nltkNB.ipynb`
- [x] Using `sklearn`
  - [x] **Naive Bayes**: 
    - [x] `MultinomialNB`: 
    - [x] `BernoulliNB`:
  - [x] **Linear Model**
    - [x] `LogisticRegression`:
    - [x] `SGDClassifier`:
  - [x] **SVM**
    - [x] `SVC`: 
    - [x] `LinearSVC`:
    - [x] `NuSVC`:

Implemented in `scikitlearnNB.ipynb`

- [x] Implemented a voting system to choose the best out of all the learning methods. Implemented in `voting_process.ipynb`

***

### Accuracy achieved
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

| **Classifiers**                 | **Accuracy achieved** |
|---------------------------------|-----------------------|
| `nltk.NaiveBayesClassifier`     | _73.0%_               |
| **ScikitLearn Implementations** |                       |
| `BernoulliNB`                   | _72.0%_               |
| `MultinomialNB`                 | _76.0%_               |
| `LogisticRegression`            | _74.0%_               |
| `SGDClassifier`                 | _69.0%_               |
| `SVC`                           | _48.0%_               |
| `LinearSVC`                     | _74.0%_               |
| `NuSVC`                         | _74.0%_               |

***

## Requirements
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

The simplest way(and the suggested way) would be to install the required packages and the dependencies by using either [anaconda](https://www.continuum.io/downloads) or [miniconda](http://conda.pydata.org/miniconda.html)

After that you can do

```sh
$ conda update conda
$ conda install scikit-learn nltk
```

***

#### Downloading the dataset
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

The dataset used in this package is bundled along with the `nltk` package.

Run your python interpreter

```python
>>> import nltk
>>> nltk.download('stopwords')
>>> nltk.download('movie_reviews') 
```

**NOTE**: You can check system specific installation instructions from the official [`nltk` website](http://www.nltk.org/data.html)

Check if everything is good till now by running your interpreter again and importing these

```python
>>> import nltk
>>> from nltk.corpus import stopwords, movie_reviews
>>> import sklearn
>>> 
```

If these imports work for you. Then you are good to go!

***

## Running it
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

1. Clone the repo 

```sh
$ git clone https://github.com/prodicus/movieReviewsAnalysis
$ cd movieReviewsAnalysis
## run the ipython server
$ ipython notebook
```

2. Order of running
  1. `nltkNB.ipynb`
  2. `scikitlearnNB.ipynb`
  3. `voting_process.ipynb`

3. Hack away!

***

## So
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

**"So what, Well this is pretty basic!"**

Yes, it is but hey we all do start somewhere right?

**Psst**. I am working on a spam filtering system. You know the one in which you paste an email and then it tells you whether
it is a spam or not.

You can follow me on twitter [@tasdikrahman](https://twitter.com/tasdikrahman) to keep tabs on it. 

***

## Legal stuff
[[Back to top]](https://github.com/prodicus/movieReviewsAnalysis#movie-review-analysis)

Hacked together by [Tasdik Rahman](http://tasdikrahman.me) under the [MIT License](http://prodicus.mit-license.org)

You can find a copy of the License at http://prodicus.mit-license.org/

