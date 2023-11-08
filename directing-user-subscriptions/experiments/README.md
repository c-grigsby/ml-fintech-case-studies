# ML experiments from _Directing User Subscriptions_ 🧪 🤖

## Algorithms

- ### [XGBoost Classifier](./mlflow_xgb/README.md)

---

## Experiment Tracking

- To utilize the [MLflow](https://mlflow.org/) UI with your experiments when using a file directory for backend storage

  ```
  $ mlflow server --backend-store-uri <absolute_path_to_directory_hosting_your_experiment>
  ```

  Open your browser at http://localhost:5000/

  <img src="../../images/mlflow-ui.png" width="800">

  _The following files are excluded from this git repository: meta.yaml, tags_
