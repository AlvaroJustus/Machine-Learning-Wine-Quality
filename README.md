<div align="center">
  <img src="http://cdn.wittysparks.com/wp-content/uploads/2017/08/09210754/Machine-Learning.jpg"><br><br>
</div>

-----------------


| **`Scikit-Learn`** |
|--------------------|
[![Scikit-Learn](https://elitedatascience.com/wp-content/uploads/2016/11/sklearn-logo.png)](http://scikit-learn.org)

# **Wine Quality Analysis**

## **Abstract**
This work aims to perform an exploratory analysis in a database on the quality of red wines. The database consists 
of wine samples from the north of Portugal, provided by the Viticulture Commission of the Vinho Verde Region (CVRVV). 
The goal is to model wine quality based on physicochemical tests (see [Cortez et al., 2009](http://www3.dsi.uminho.pt/pcortez/wine/)) using machine learning techniques and models to classify and predict dataset data. Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.).

## Source
* [Paulo Cortez, University of Minho, Guimarães, Portugal](http://www3.dsi.uminho.pt/pcortez).
* [A. Cerdeira, F. Almeida, T. Matos and J. Reis, Viticulture Commission of the Vinho Verde Region(CVRVV), Porto, Portugal @2009](http://www.vinhoverde.pt/en/).
* [UCI Machine Learning Repository Wine Quality Data Set](https://archive.ics.uci.edu/ml/datasets/Wine+Quality).


## Data Information ##

|**Number of Instances:**| 4898      | **Attribute Characteristics:** |  Real    |
|------------------------|-----------|--------------------------------|----------|
|    **Date Donated:**   | 2009-10-07|          **Area:**             | Business |

* There are 12 classes that make up the dataset. There is no previous information about any class, so it is necessary to analyze the influence and relevance of each one.

**Attribute Information:**

For more information, read [Cortez et al., 2009](http://www3.dsi.uminho.pt/pcortez/wine/). 

Input variables (based on physicochemical tests):

* 1 - Fixed acidity (g(tartaric acid)/dm3)
* 2 - Volatile acidity (g(acetic acid)/dm3)
* 3 - Citric acid (g/dm3)
* 4 - Residual sugar (g/dm3)
* 5 - Chlorides (g(sodium chloride)/dm3)
* 6 - Free sulfur dioxide (mg/dm3)
* 7 - Total sulfur dioxide (mg/dm3)
* 8 - Density (g/cm3)
* 9 - pH
* 10 - Sulphates (g(potassium sulphate)/dm3)
* 11 - Alcohol (% vol.)

Output variable (based on sensory data):
* 12 - quality (score between 0 and 10)


[References](http://www3.dsi.uminho.pt/pcortez/wine5.pdf)


## Data Exploration 
```shell
$ python
```
```python
>>> import pandas as pd
>>> import matplotlib.pyplot as plt
>>> %matplotlib inline
>>> import seaborn as sns
>>> wine = pd.read_csv('winequality-red.csv',sep=';')
>>> wine.info()
	fixed acidity	volatile acidity	citric acid	residual sugar	chlorides	free sulfur dioxide	total sulfur dioxide	density	pH	sulphates	alcohol	quality
count	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000	1599.000000
mean	8.319637	0.527821	0.270976	2.538806	0.087467	15.874922	46.467792	0.996747	3.311113	0.658149	10.422983	5.636023
std	1.741096	0.179060	0.194801	1.409928	0.047065	10.460157	32.895324	0.001887	0.154386	0.169507	1.065668	0.807569
min	4.600000	0.120000	0.000000	0.900000	0.012000	1.000000	6.000000	0.990070	2.740000	0.330000	8.400000	3.000000
25%	7.100000	0.390000	0.090000	1.900000	0.070000	7.000000	22.000000	0.995600	3.210000	0.550000	9.500000	5.000000
50%	7.900000	0.520000	0.260000	2.200000	0.079000	14.000000	38.000000	0.996750	3.310000	0.620000	10.200000	6.000000
75%	9.200000	0.640000	0.420000	2.600000	0.090000	21.000000	62.000000	0.997835	3.400000	0.730000	11.100000	6.000000
max	15.900000	1.580000	1.000000	15.500000	0.611000	72.000000	289.000000	1.003690	4.010000	2.000000	14.900000	8.000000
42
>>> sess.close()
```


#### *Try your first TensorFlow program*
```shell
$ python
```
```python
>>> import tensorflow as tf
>>> hello = tf.constant('Hello, TensorFlow!')
>>> sess = tf.Session()
>>> sess.run(hello)
'Hello, TensorFlow!'
>>> a = tf.constant(10)
>>> b = tf.constant(32)
>>> sess.run(a + b)
42
>>> sess.close()
```

## Contribution guidelines

**If you want to contribute to TensorFlow, be sure to review the [contribution
guidelines](CONTRIBUTING.md). This project adheres to TensorFlow's
[code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
uphold this code.**

**We use [GitHub issues](https://github.com/tensorflow/tensorflow/issues) for
tracking requests and bugs. So please see
[TensorFlow Discuss](https://groups.google.com/a/tensorflow.org/forum/#!forum/discuss) for general questions
and discussion, and please direct specific questions to [Stack Overflow](https://stackoverflow.com/questions/tagged/tensorflow).**

The TensorFlow project strives to abide by generally accepted best practices in open-source software development:

[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1486/badge)](https://bestpractices.coreinfrastructure.org/projects/1486)

## For more information

* [TensorFlow Website](https://www.tensorflow.org)
* [TensorFlow White Papers](https://www.tensorflow.org/about/bib)
* [TensorFlow Model Zoo](https://github.com/tensorflow/models)
* [TensorFlow MOOC on Udacity](https://www.udacity.com/course/deep-learning--ud730)
* [TensorFlow Course at Stanford](https://web.stanford.edu/class/cs20si)

Learn more about the TensorFlow community at the [community page of tensorflow.org](https://www.tensorflow.org/community) for a few ways to participate.

## License

[MIT](LICENSE)
