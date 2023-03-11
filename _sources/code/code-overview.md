# Code overview

## Exam

In the exam, you will get a copy of the following code cheat sheets: 

- [Pandas cheat sheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)

- [Altair marks](../code/altair-marks.md)

- [Scikit-learn cheat sheets (see Moodle)](https://e-learning.hdm-stuttgart.de/moodle/course/view.php?id=2464#section-2)

---

## Week 1

[First Data Analysis (Nr. 4): 💻](../ae/ae1/01-1b-netflix-g.ipynb)


```{note}

You should be able to:

- Import CSV-data
- Create a crosstable

```

---

## Week 2

[GitHub-Repo: umfrage](https://github.com/kirenz/umfrage)



```{note}

You should be able to:

- Get a data overview and show the dataframe metadata
- Rename columns
- Change data types to numeric, category or ordinal (using loops)
- Recode variables (e.g. from integers to likert scale)
- Create "quasi-metric" variables
- Save data as CSV

```

*Not relevant: dummy-variables*

---

## Week 3

- [11. Introduction to Altair](../code/11-altair_introduction_p.ipynb) (not relevant)

<br>

- [12. Loans data](../code/12-data-overview.ipynb)

```{note}

You should be able to:

- Summarize the frequencies of categorical variables 
- Show levels of categorical variables
- Obtain a data summary for categorical variables
```


- [13. Simple bar chart](../code/13-bar-chart-altair.ipynb)
- [14. Dodged bar plot](../code/14-dodged-bar-chart-altair.ipynb) (not relevant)
- [15. Stacked bar plot](../code/15-stacked-bar-chart-altair.ipynb)
- [16. Standardized bar plot](../code/16-standardized-bar-chart-altair.ipynb)
- [17. Pie chart](../code/17-pie-charts-altair.ipynb) (not relevant)
- [18. Contingency tables](../code/18-contingency-table-bar-plot.ipynb)
- [19. Contingency tables with proportions](../code/19-row-column-proportions.ipynb)



```{note}

You should be able to create:

- Bar plots 
- Customized plots (change axis title, sort values, ...)
- Stacked bar plots
- Standardized bar plots 
- Contingeny tables (crosstable) with proportions

```

---

## Week 4

- [20. Data Analysis Case: GitHub "umfrage"](https://github.com/kirenz/umfrage) (see week 2: you should have a local copy of this repo called `umfrage-main`) 

```{note}
You should be able to:

- Obtain statistical summaries of numerical and categorical data
- Create appropriate plots and customize their axes

```

- [21. Scatterplot](../code/21-scatterplot-paired-data-altair.ipynb)
- [22. Dot plot mean median and mode](../code/22-dot-plots-mean-altair.ipynb)
- [23. Histogram ](../code/23-histograms-altair.ipynb)
- [24. Variance and standard deviation (kernel density plot)](../code/24-histograms-kernel-density-altair.ipynb)
- [25. Box Plot](../code/25-box-plot-altair.ipynb)
- [26. Robust statistics and transformations](../code/26-transforming-data-altair.ipynb) (not relevant)
- [27. Comparing numerical data across groups](../code/27-comparisons-across-groups-altair.ipynb)


```{note}
You should be able to create:

- Scatter plots
- Histograms
- Kernel density plots
- Boxplots
- Plots to compare numerical data across groups

```

Optional:

- [Mapping data](../code/mapping-data-altair.ipynb)

---

## Week 5

- [28. Introduction to models](../code/28-ds-happy-scikit.ipynb)

---

Numbers 29 to 32 are application exercises:


- Models 1: Sales and ads (Nr. 29): [💻](../ae/models_1/07a-intro-sales-g.ipynb)
- Models 2: Mean squared error 1 (Nr. 30): [💻](../ae/models_2/07b-1-mse-g.ipynb)
- Models 3: Mean squared error 2 (Nr. 31): [💻](../ae/models_3/07b-2-mse-g.ipynb)
- Models 4: Mean squared error 3 (Nr. 32): [💻](../ae/models_4/07b-3-mse-g.ipynb)

---


- [33. Fitting a model](../code/33-fitting.ipynb)

---



```{note}
You should be able to use scikit-learn to:

- Fit a model
- Make predictions
- Evaluate your model (with MSE and RMSE)

```

---

## Week 6

Market research

- [35. Data splitting](../code/35-ds-happy-scikit-splitting.ipynb)

Statistics

- [36. Correlation](../code/36-correlation.ipynb)
- [37. Least squares regression](../code/37-least-squares.ipynb)
- [38. R squared](../code/38-strength-fit.ipynb)
- [39. Categorical predictors with two levels](../code/39-categorical.ipynb)


```{note}
You should be able to use scikit-learn to:

- Obtain correlations
- Use a categorical predictor in your model
- Fit a model using data splitting
- Evaluate your model with R squared 

```

---

## Week 7


- [43. Multiple predictors regression 1](../code/44-1-multiple.ipynb)
- [44. Multiple predictors regression 2](../code/45-2-multiple.ipynb)
- [45. Multiple predictors regression 3](../code/46-3-multiple.ipynb)

```{note}
You should be able to use scikit-learn to:

- create a model with multiple predictors

```

---


## Week 8

- [48. Randomization experiments](../code/48-discrimination.ipynb) (not relevant for exam: you don't need to memorize the code. See week 9)

- [49. Probability of an event](../code/49-logistic.ipynb)

- [50. Multiple predictors classification](../code/50-logistic.ipynb)


```{note}
You should be able to use scikit-learn to:

- create a train and test set
- create a logistic regression model with cross-fold-validation
- investigate your models performance 

```

---

## Week 9

- [54. Hypothesis tesing opportunity cost ](../code/54-opportunity.ipynb)

- [56. Bootsrapping medical case](../code/56-medical-case.ipynb)

```{note}
You should be able to 

- change the variables to make calculations
- use the code to make all necessary calculations

You don't need to memorize the code (it would be provided in the exam). However, you would need to adapt some of the variables (like `n` or `p` in the bootsrapping example).

```

## Week 10

- [59. Mathematical introduction (exercise)](../code/59-mathematical-c.ipynb)
- [59. Mathematical introduction (solution)](../code/59-mathematical.ipynb)



```{note}
You should be able to 

- change the variables to make calculations
- use the code to make all necessary calculations

You don't need to memorize the code (it would be provided in the exam). However, you would need to adapt some of the variables.

```

---