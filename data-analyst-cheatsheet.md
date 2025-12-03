# 📘 Data Analyst Master Cheat Sheet

## 🐼 Pandas (Python)
- Inspect: `df.head()`, `df.info()`, `df.describe()`
- Select: `df['col']`, `df.loc[row, col]`, `df.iloc[row, col]`
- Filter: `df[df['col'] > 10]`, `df.query("col > 10")`
- Merge/Join: `pd.merge(df1, df2, on='key')`
- GroupBy: `df.groupby('col')['val'].mean()`
- Missing Data: `df.dropna()`, `df.fillna(value)`
- Export: `df.to_csv('file.csv')`, `df.to_excel('file.xlsx')`

---

## 🗄️ SQL
- Basic Query: `SELECT col1, col2 FROM table WHERE condition;`
- Joins: `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL JOIN`
- Aggregates: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`
- Grouping: `GROUP BY col HAVING condition`
- Window Functions: `ROW_NUMBER() OVER (PARTITION BY col ORDER BY col2)`

---

## 📊 Excel
- Formulas: `=SUM(A1:A10)`, `=IF(A1>10,"Yes","No")`, `=VLOOKUP(value, range, col, FALSE)`
- Pivot Tables: Summarize datasets quickly
- Conditional Formatting: Highlight cells by rules
- Charts: Line, bar, scatter, combo
- Data Cleaning: `TRIM()`, `CLEAN()`, Text-to-Columns

---

## 📈 Tableau
- Connect Data: CSV, Excel, SQL databases
- Dimensions vs Measures: Categories vs numeric values
- Filters: Quick filters, context filters
- Calculated Fields: `IF [Sales] > 1000 THEN "High" ELSE "Low" END`
- Visualizations: Bar charts, scatter plots, maps, dashboards
- Best Practices: Simplicity, highlight insights, use color sparingly

---

## 🎨 Python Visualization

### Matplotlib
- Plot: `plt.plot(x, y)`
- Scatter: `plt.scatter(x, y)`
- Bar: `plt.bar(categories, values)`
- Histogram: `plt.hist(data, bins=10)`

### Seaborn
- Distribution: `sns.histplot(data['col'])`
- Box Plot: `sns.boxplot(x='category', y='value', data=df)`
- Heatmap: `sns.heatmap(df.corr(), annot=True)`

### Plotly (Interactive)
- Scatter: `px.scatter(df, x="col1", y="col2", color="category")`
- Line: `px.line(df, x="date", y="sales")`

---

## 📈 Python Statistical Analysis

### SciPy
- T-test: `stats.ttest_ind(group1, group2)`
- Chi-Square: `stats.chisquare(observed, expected)`

### Statsmodels
- Linear Regression:
  ```python
  X = df[['col1','col2']]
  y = df['target']
  X = sm.add_constant(X)
  model = sm.OLS(y, X).fit()
  print(model.summary())
