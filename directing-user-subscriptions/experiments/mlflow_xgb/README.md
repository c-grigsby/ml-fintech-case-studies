# mlflow_xgb

Hyperopt trials for XGBoost Classifier

- Experiment ID: 880003663376093159, Name: hyperopt_tuning_66393

  Description: MLflow runs from XGBClassifier hyperparameter tuning to maximize **AUC (Area Under the ROC Curve)** scores. Models fit on the training data of a train/validation/test split. Files excluded from git: meta.yaml, tags.

  ```python
  num_evals = 80
  search_space = {
    'n_estimators':scope.int(hp.quniform('n_estimators', 100, 300, 10)),
    'eval_metric': 'auc',
    'max_depth': scope.int(hp.quniform('max_depth', 4, 15, 1)),
    'subsample': hp.uniform('subsample', .5, 1.0),
    'learning_rate' : hp.quniform('learning_rate', 0.01, 0.5, 0.01),
    'min_child_weight': hp.loguniform('min_child_weight', -1, 7),
    'reg_alpha': hp.loguniform('reg_alpha', -10, 10),
    'reg_lambda': hp.loguniform('reg_lambda', -10, 10),
    'gamma': hp.loguniform('gamma', -10, 10),
    'use_label_encoder': False,
    'verbosity': 0,
    }
  ```

  100%|██████████| 80/80 [14:29<00:00, 10.87s/trial, best loss: -0.8622906149292368]

  {'gamma': 0.0022788464778158196, 'learning_rate': 0.029003908033482288, 'max_depth': 7.0, 'min_child_weight': 0.8170911337892932, 'n_estimators': 400.0, 'reg_alpha': 0.00010215677382178698, 'reg_lambda': 5.890998154323654, 'subsample': 0.8923501519435082}

  Best Scoring Run ID: [95578a56d15a4e539cbcd74cff84be56](./880003663376093159/95578a56d15a4e539cbcd74cff84be56/)
