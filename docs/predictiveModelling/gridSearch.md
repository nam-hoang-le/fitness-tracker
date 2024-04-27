# Grid search

We will perform grid search of the most important parameters validate them using a 5 fold cross validation on the training set.

## Example 

```
{
	"min_samples_leaf": [2, 10, 50, 100, 200],
	"n_estimators": [10, 50, 100],
	"criterion": ["gini", "entropy"],
}

rf = GridSearchCV(
    RandomForestClassifier(), tuned_parameters, cv=5, scoring="accuracy"
)
```

[Grid Searching From Scratch using Python](https://www.geeksforgeeks.org/grid-searching-from-scratch-using-python/)