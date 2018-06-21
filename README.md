# Example MLflow Diabetes project

MLflow model using ElasticNet (sklearn) and Plots Lasso vs. ElasticNet Descent Paths

Usage:
```
# Via Python
python train_diabetes.py {alpha} {l1_ratio}

# Execute a MLproject published on GitHub  (ensure you have installed conda)
mlflow run git@github.com:dennyglee/mlflow-diabetes-example.git -P alpha=0.02 -P l1_ratio=0.05

# Remote execution on Databricks 
mlflow run -m databricks --cluster-spec cluster.json <uri>
```


Usage Notes:
* Remote Execution on Databricks
  * Refer to [Databricks Jobs New Cluster](https://docs.databricks.com/api/latest/jobs.html#jobsclusterspecnewcluster) on how to configure `cluster.json`. 
  * Currently this feature requires a new cluster creation

Attributions:
* This project uses the [sklearn Diabetes dataset](http://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_diabetes.html) to predict diabetes progression using ElasticNet
 * The predicted "progression" column is a quantitative measure of disease progression one year after baseline
* This proeject combines the above with the [Lasso Descent Path Plot](http://scikit-learn.org/stable/auto_examples/linear_model/plot_lasso_coordinate_descent_path.html)
 * Original author: Alexandre Gramfort <alexandre.gramfort@inria.fr>; License: BSD 3 clause

