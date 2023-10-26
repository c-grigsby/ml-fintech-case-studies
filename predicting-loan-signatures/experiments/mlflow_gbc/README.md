# mlflow_gbc

Hyperopt trials for Gradient Boosting Classifier

- ID: 473782803715669826, Name: hyperopt_tuning_85615

  Description: MLflow runs from scikit-learn Gradient Boosting Classifier models with the highest accuracy scores. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 105
  search_space = {
    'n_estimators': hp.quniform('n_estimators', 50, 300, 5),
    'max_depth': hp.quniform('max_depth', 3, 10, 1),
    'min_samples_split': hp.quniform('min_samples_split', 2, 10, 1),
    'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 10, 1),
    'learning_rate': hp.loguniform('learning_rate', np.log(0.01), np.log(0.2)),
    'subsample': hp.uniform('subsample', 0.7, 1.0),
    'max_features': hp.choice('max_features', ['sqrt', 'log2', None]),
    }
  ```

  100%|██████████| 105/105 [20:12<00:00, 11.55s/trial, best loss: -0.642188648302595]

  {'learning_rate': 0.033750928322144595, 'max_depth': 9.0, 'max_features': 1, 'min_samples_split': 6.0, 'min_samples_leaf': 5.0, 'n_estimators': 195.0, 'subsample': 0.9456725930585413}

  best run_id: be1341227be3421ab22c5c49410627cb

---

- ID: 471826949328499785, Name: hyperopt_tuning_27275

  Description: MLflow runs from scikit-learn Gradient Boosting Classifier models with the highest accuracy scores. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 105
  search_space = {
      'n_estimators': hp.quniform('n_estimators', 100, 400, 10),
      'max_depth': hp.quniform('max_depth', 5, 10, 1),
      'min_samples_split': hp.quniform('min_samples_split', 2, 10, 1),
      'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 10, 1),
      'learning_rate': hp.loguniform('learning_rate', np.log(0.01), np.log(0.2)),
      'subsample': hp.uniform('subsample', 0.7, 1.0),
      'max_features': hp.choice('max_features', ['sqrt', 'log2', None]),
  }
  ```

  best loss: 0.6430966788567619

  {'learning_rate': 0.0273666022526306, 'max_depth': 6, 'max_features:' 2, min_samples_split': 10, 'min_samples_leaf': 1, 'n_estimators': 350, 'subsample': 0.703030578436894}

  best run_id: 72d6080d9f5a4c54bd602012d622cb94

---

- ID: 717375715905391499, Name: hyperopt_tuning_68832

  Description: MLflow runs from scikit-learn Gradient Boosting Classifier models with the highest accuracy scores. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 105
  search_space = {
      'n_estimators': hp.quniform('n_estimators', 200, 400, 10),
      'max_depth': hp.quniform('max_depth', 5, 10, 1),
      'min_samples_split': hp.quniform('min_samples_split', 5, 15, 1),
      'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 10, 1),
      'learning_rate': hp.loguniform('learning_rate', np.log(0.02), np.log(0.04)),
      'subsample': hp.uniform('subsample', 0.7, 1.0),
      'max_features': hp.choice('max_features', ['sqrt', 'log2', None]),
  }
  ```

  100%|██████████| 105/105 [38:38<00:00, 22.08s/trial, best loss: -0.6426775237443764]

  {'learning_rate': 0.027821122390237863, 'max_depth': 7.0, 'max_features': 2, 'min_samples_leaf': 9.0, 'min_samples_split': 12.0, 'n_estimators': 240.0, 'subsample': 0.9458859821178202}

  best run_id: 4ffaa2c620e14681a582e67750f15263
