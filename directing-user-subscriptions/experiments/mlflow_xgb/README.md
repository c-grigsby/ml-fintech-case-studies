# mlflow_xgb

Hyperopt trials for XGBClassifier

- Experiment ID: 880003663376093159, Name: hyperopt_tuning_66393

  Description: MLflow runs from XGBClassifier hyperparameter tuning to maximize **AUC (Area Under the ROC Curve)** scores. Models fit on the training data of a train-validation-test split.

  ```python
  num_evals = 80
  search_space = {
    'objective': 'binary:logistic',
    'eval_metric': 'auc',
    'n_estimators': scope.int(hp.quniform('n_estimators', 100, 1000, 10)),
    'max_depth': scope.int(hp.quniform('max_depth', 4, 12, 1)),
    'subsample': hp.uniform('subsample', .5, 1.0),
    'learning_rate': hp.loguniform('learning_rate', -7, 0),
    'min_child_weight': hp.loguniform('min_child_weight', -1, 7),
    'reg_alpha': hp.loguniform('reg_alpha', -10, 10),
    'reg_lambda': hp.loguniform('reg_lambda', -10, 10),
    'gamma': hp.loguniform('gamma', -10, 10),
    'use_label_encoder': False,
    'verbosity': 0,
    }

  ```

  100%|██████████| 80/80 [16:50<00:00, 12.64s/trial, best loss: -0.8625258090829855]
  {'gamma': 0.06452469202559104, 'learning_rate': 0.025467532325811212, 'max_depth': 7.0, 'min_child_weight': 6.539288994604176, 'n_estimators': 400.0, 'reg_alpha': 2.978329442686076, 'reg_lambda': 6.4187421917346645, 'subsample': 0.6502970843845121}

  best loss run_id: caddb0ac9d0c4194b83ea3c26d977f97

---

- Experiment ID: 19, Name: hyperopt_tuning_57778

  Description: MLflow runs from XGBClassifier hyperparameter tuning to maximize **F-beta** scores, where beta equals 0.75 in favor of precision. Models fit on the training data of a train-validation-test split.

  ```python
  num_evals = 120
  search_space = {
    "objective": "binary:logistic",
    "eval_metric": "auc",
    "n_estimators": scope.int(hp.quniform('n_estimators', 100, 1000, 1)),
    "max_depth": scope.int(hp.quniform('max_depth', 4, 12, 1)),
    "subsample": hp.uniform('subsample', .5, 1.0),
    "learning_rate": hp.loguniform('learning_rate', -7, 0),
    "min_child_weight": hp.loguniform('min_child_weight', -1, 7),
    "reg_alpha": hp.loguniform('reg_alpha', -10, 10),
    "reg_lambda": hp.loguniform('reg_lambda', -10, 10),
    "gamma": hp.loguniform('gamma', -10, 10),
    "use_label_encoder": False,
    "verbosity": 0
    }

  ```

  100%|██████████| 120/120 best loss: -0.7854921322480317]

  {'gamma': 0.0058070705817357335, 'learning_rate': 0.02266056614193427, 'max_depth': 9.0, 'min_child_weight': 1.4049131427499348, 'n_estimators': 647.0, 'reg_alpha': 0.7126508780262765, 'reg_lambda': 63.71632269911593, 'subsample': 0.9998138605426556}

  best loss run_id: d630509aed81407d98143970c26dd3fc

  Best scoring run so far ⭐

**_To reduce repository size, the SQLite database and artifacts from Hyperopt trials are excluded from git_**
