# Example MLflow Diabetes project

MLflow model using ElasticNet (sklearn) and Plots Lasso vs. ElasticNet Descent Paths

Usage:
```
python train_diabetes.py {alpha} {l1_ratio}
```


Uses the [sklearn Diabetes dataset](http://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_diabetes.html) to predict diabetes progression using ElasticNet
* The predicted "progression" column is a quantitative measure of disease progression one year after baseline
 
Combines the above with the [Lasso Descent Path Plot](http://scikit-learn.org/stable/auto_examples/linear_model/plot_lasso_coordinate_descent_path.html)
* Original author: Alexandre Gramfort <alexandre.gramfort@inria.fr>; License: BSD 3 clause

