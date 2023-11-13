# mlflow_gbc

Hyperopt trials for GradientBoostingClassifier

- Experiment ID: 473782803715669826, Name: hyperopt_tuning_85615

  Description: MLflow runs from hyperparameter tuning with scikit-learn GradientBoostingClassifier models aiming to maximize **accuracy** scores. To reduce repository size, only runs with the highest loss scores persisted. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

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

  best loss run_id: [be1341227be3421ab22c5c49410627cb](./473782803715669826/be1341227be3421ab22c5c49410627cb/)

---

- Experiment ID: 471826949328499785, Name: hyperopt_tuning_27275

  Description: MLflow runs from hyperparameter tuning with scikit-learn GradientBoostingClassifier models aiming to maximize **accuracy** scores. To reduce repository size, only runs with the highest loss scores persisted. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

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

  best loss run_id: [72d6080d9f5a4c54bd602012d622cb94](./471826949328499785/72d6080d9f5a4c54bd602012d622cb94/)

---

- Experiment ID: 741470921111613064, Name: hyperopt_tuning_72801

  Description: MLflow runs from hyperparameter tuning with scikit-learn GradientBoostingClassifier models aiming to maximize **accuracy** scores. To reduce repository size, only runs with the highest loss scores persisted. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 90
  search_space = {
    'n_estimators': hp.quniform('n_estimators', 300, 500, 10),
    'max_depth': hp.quniform('max_depth', 5, 7, 1),
    'min_samples_split': hp.quniform('min_samples_split', 9, 11, 1),
    'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 3, 1),
    'learning_rate': hp.loguniform('learning_rate', np.log(0.015), np.log(0.03)),
    'subsample': hp.uniform('subsample', 0.7, 0.8),
    'max_features': None
    }
  ```

  100%|██████████| 90/90 [52:05<00:00, 34.73s/trial, best loss: -0.6437944375747264]

  {'learning_rate': 0.020537900334065485, 'max_depth': 7.0, 'min_samples_leaf': 2.0, 'min_samples_split': 11.0, 'n_estimators': 300.0, 'subsample': 0.7628578451766926}

  best loss run_id: [d1ae942cb52e49209243d247494f3586](./741470921111613064/d1ae942cb52e49209243d247494f3586/)

---

- Experiment ID: 504706898397860315, Name: hyperopt_tuning_21802

  Description: MLflow runs from hyperparameter tuning with scikit-learn GradientBoostingClassifier models aiming to maximize **accuracy** scores. To reduce repository size, only runs with the highest loss scores persisted. Models will need to be fit before inference. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 60
  search_space = {
    'n_estimators': hp.quniform('n_estimators', 200, 450, 10),
    'max_depth': hp.quniform('max_depth', 5, 8, 1),
    'min_samples_split': hp.quniform('min_samples_split', 2, 10, 1),
    'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 10, 1),
    'learning_rate': hp.loguniform('learning_rate', np.log(0.01), np.log(0.2)),
    'subsample': hp.uniform('subsample', 0.7, 1.0),
    'max_features': None
    }
  ```

  100%|██████████| 60/60 [56:47<00:00, 56.79s/trial, best loss: -0.6451206843427608]

  {'learning_rate': 0.03610888652938746, 'max_depth': 5.0, 'min_samples_leaf': 3.0, 'min_samples_split': 10.0, 'n_estimators': 290.0, 'subsample': 0.9224316008981079}

  best loss run_id: [ba26710b072f4e71830210a46bbf1c06](./504706898397860315/ba26710b072f4e71830210a46bbf1c06/)

---

- Experiment ID: 224708608558611348, Name: hyperopt_tuning_28319

  Description: MLflow runs from hyperparameter tuning with scikit-learn GradientBoostingClassifier models aiming to maximize **AUC (Area Under the ROC Curve)** scores. Models fit on the training set of a train-validation-test split. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 90
  search_space = {
    'n_estimators': hp.quniform('n_estimators', 100, 400, 10),
    'max_depth': hp.quniform('max_depth', 5, 10, 1),
    'min_samples_split': hp.quniform('min_samples_split', 2, 10, 1),
    'min_samples_leaf': hp.quniform('min_samples_leaf', 1, 10, 1),
    'learning_rate': hp.loguniform('learning_rate', np.log(0.01), np.log(0.2)),
    'subsample': hp.uniform('subsample', 0.7, 1.0),
    'max_features': None
    }
  ```

  100%|██████████| 90/90 [54:15<00:00, 36.17s/trial, best loss: -0.7019982364013503]
  {'learning_rate': 0.020813922863003702, 'max_depth': 8.0, 'min_samples_leaf': 1.0, 'min_samples_split': 8.0, 'n_estimators': 220.0, 'subsample': 0.7489880854309083}

  best loss run_id: [75bdabb8181e4752a842c55efcc725af](./224708608558611348/75bdabb8181e4752a842c55efcc725af/)

  Best scoring run so far ⭐
