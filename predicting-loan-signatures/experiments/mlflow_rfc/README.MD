# mlflow_rfc

Hyperopt trials for Random Forest Classifier

- ID: 995960703112558784, Name: hyperopt_tuning

  Description: MLflow runs from scikit-learn Random Forest Classifier models with the highest accuracy scores during initial Hyperopt trials. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 85
  search_space = {'criterion': 'entropy',
        'max_depth': hp.quniform('max_depth', 1, 10, 1),
        'max_features': hp.choice('max_features', ['sqrt','log2', None]),
        'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 10, 1),
        'min_samples_split' : hp.quniform ('min_samples_split', 2, 10, 1),
        'n_estimators' : hp.quniform('n_estimators', 50, 500, 5)
        }
  ```

  best_loss: 0.6319977724574005

  best_params: {'criterion': 0, 'max_depth': 10.0, 'max_features': 1, 'min_samples_leaf': 4.0, 'min_samples_split': 8.0, 'n_estimators': 375.0}

  best run_id: = 79b16a349526460b98af72d593fde3ff

---

- ID: 220807592115232226, Name: hyperopt_tuning_34874

  Description: MLflow runs from scikit-learn Random Forest Classifier models with the highest accuracy scores during Hyperopt trials. Models need to be fit before inference.

  ```python
  num_evals = 85
  search_space = {'criterion': 'gini',
        'max_depth': hp.quniform('max_depth', 1, 10, 1),
        'max_features': hp.choice('max_features', ['sqrt','log2', None]),
        'min_samples_leaf': hp.quniform('min_samples_leaf', 3, 10, 1),
        'min_samples_split' : hp.quniform ('min_samples_split', 2, 5, 1),
        'n_estimators' : hp.quniform('n_estimators', 100, 200, 5)
        }
  ```

  100%|██████████| 85/85 [46:35<00:00, 32.89s/trial, best loss: -0.6333237609135937]

  {'max_depth': 10.0, 'max_features': 2, 'min_samples_leaf': 3.0, 'min_samples_split': 3.0, 'n_estimators': 165.0}

  best run_id: 0ea345a3613140548c2f86095cc3b9ff

---
