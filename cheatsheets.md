# Data Analyst Cheat Sheets

## 🐼 Pandas
- `df.head()`, `df.info()`, `df.describe()`
- `df['col']`, `df.loc[row, col]`, `df.iloc[row, col]`
- `pd.merge(df1, df2, on='key')`
- `df.groupby('col')['val'].mean()`
- `df.dropna()`, `df.fillna(value)`
- `df.to_csv('file.csv')`

## 🗄️ SQL
- `SELECT col1, col2 FROM table WHERE condition;`
- `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL JOIN`
- `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`
- `GROUP BY col HAVING condition`
- `ROW_NUMBER() OVER (PARTITION BY col ORDER BY col2)`

## 📊 Excel
- `=SUM(A1:A10)`, `=IF(A1>10,"Yes","No")`
- `=VLOOKUP(value, range, col, FALSE)`
- Pivot Tables, Conditional Formatting, Charts
- `TRIM()`, `CLEAN()`, Text-to-Columns

## 📈 Tableau
- Connect to CSV, Excel, SQL
- Dimensions vs Measures
- Filters, Calculated Fields
- Bar charts, scatter plots, maps, dashboards
- Best practices: simplicity, highlight insights, use color sparingly
