# mushroom
Mushroom is simply the data, Jupyter notebook, and files that supported the writing of a Medium blog post, [*What Decision Trees Tell Us About Deadly Mushrooms*](https://medium.com/@evanquinlan/what-decision-trees-tell-us-about-deadly-mushrooms-b0342778b9de).

The article attempts to answer three questions from a dataset containing 22 features of North American mushroom samples:
1. Can a machine learning model reliably identify poisonous mushrooms based on the data?
2. Does any one feature of the data reliably classify mushroom toxicity?
3. Can we formulate simple, memorizable rules from the data that reliably classify mushroom toxicity?

## Data
Data was obtained fromm the [UCI Machine Learning Repository Mushroom Data Set](https://archive.ics.uci.edu/ml/datasets/Mushroom), donated by Jeff Schlimmer and drawn from *The Audubon Society Field Guide to North American Mushrooms* (1981). G. H. Lincoff (Pres.), New York: Alfred A. Knopf.

Note there are two datasets, seemingly due to some data recovery efforts on the part of the donor:
- [`agaricus-lepiota.data`](../master/downloaded/agaricus-lepiota.data), which has fewer records and uses single-chararcter representations of categorical values
- [`expanded`](../master/data/expanded), which has more records and uses full-word representations of categorical values (unzipped from [`expanded.Z`](../master/downloaded/expanded.Z))
My exploration makes use of the `expanded` dataset.

## Code
View the [Jupyter notebook](../master/analysis.ipynb).

To run the code locally you will need Python 3.7+ and [JupyterLab or Jupyter Notebook](https://jupyter.org/install) as well as the following Python libraries:
- [pandas](https://pandas.pydata.org/docs/getting_started/index.html)
- [scikit-learn](https://scikit-learn.org/stable/install.html)
- [Graphviz](https://pypi.org/project/graphviz-python/)
