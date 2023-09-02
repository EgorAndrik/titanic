<h1 align="center">Titanic - Machine Learning from Disaster</h1>

## Used technology stack:

<img src="https://img.shields.io/badge/PYTHON-black?style=for-the-badge&logo=python&logoColor=gold"/><img src="https://img.shields.io/badge/SKLEARN-black?style=for-the-badge&logo=scikit-learn&logoColor=blue"/><img src="https://img.shields.io/badge/JUPYTER-black?style=for-the-badge&logo=jupyter&logoColor=orange"/><img src="https://img.shields.io/badge/GIT-black?style=for-the-badge&logo=git&logoColor=orange"/><img src="https://img.shields.io/badge/NUMPY-black?style=for-the-badge&logo=NumPy&logoColor=013243"/><img src="https://img.shields.io/badge/PANDAS-black?style=for-the-badge&logo=Pandas&logoColor=pink"/><img src="https://img.shields.io/badge/VSC-black?style=for-the-badge&logo=Visual Studio Code&logoColor=007ACC"/><img src="https://img.shields.io/badge/GITHUB-black?style=for-the-badge&logo=GitHub&logoColor=white"/><img src="https://img.shields.io/badge/KAGGLE-black?style=for-the-badge&logo=Kaggle&logoColor=blue"/>

## Best submission score: 0.78468

## Progress
<h4>In this competition with kaggel, I used algorithms such as:</h4>

- <b>KNeighborsClassifier</b>
- <b>LogisticRegression</b>
- <b>RandomForestClassifier</b>
- <b>GradientBoostingClassifier</b>
- <b>CatBoostClassifier</b>

<h4>4 models showed themselves better, and for them I did a search of the parameters along the grid. In the end it all turned out like this:</h4>

## Best hyperparametrs for each model
- <b>LogisticRegression:</b>
```python
{'C': 0.5,
 'dual': False,
 'fit_intercept': True,
 'multi_class': 'auto',
 'penalty': 'l1',
 'solver': 'liblinear',
 'warm_start': True}
```

- <b>RandomForestClassifier:</b>
```python
{'criterion': 'log_loss',
 'max_depth': 5,
 'min_samples_leaf': 1,
 'min_samples_split': 6,
 'n_estimators': 200}
```

- <b>GradientBoostingClassifier:</b>
```python
{'criterion': 'squared_error',
 'learning_rate': 0.01,
 'loss': 'exponential',
 'max_depth': 5,
 'max_features': 'log2',
 'n_estimators': 200,
 'subsample': 0.25}
```

- <b>CatBoostClassifier:</b>
```python
{'border_count': 56,
 'depth': 4,
 'iterations': 500,
 'l2_leaf_reg': 10,
 'learning_rate': 0.01}
```

<h4>Then from these 4 models I made an ensemble and predicted a test sample.</h4>
