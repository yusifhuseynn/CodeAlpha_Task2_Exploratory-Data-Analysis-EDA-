""" CodeAlpha Task 2 - Exploratory Data Analysis (EDA) This project is completed as part of the CodeAlpha Data Analytics Internship for Task 2: Exploratory Data Analysis (EDA).

## Project Overview
This task involves performing an **Exploratory Data Analysis (EDA)** on a dataset containing information about books, including their title, price, rating, author, description, and category. The main goal is to understand the **distribution of key variables**, explore patterns in the data, and visualize relationships that could inform future analysis or predictive modeling.

The dataset used for this task is: `books_toscrape.csv`.

---

## Dataset Description
| Column Name  | Data Type | Description |
|--------------|-----------|-------------|
| Book Title   | object    | Title of the book |
| Price        | float     | Price of the book in GBP (£) |
| Rating       | object    | Book rating in words (e.g., 'One', 'Two', 'Three') |
| Author       | object    | Name of the author (mostly missing) |
| Description  | object    | Short description of the book |
| Category     | object    | Category or genre of the book |

**Notes:**
- The `Price` column originally contained the '£' symbol, which has been removed and converted to numeric type.
- The `Rating` column was mapped from text labels to numeric values (1–5) for analysis purposes.

---

## Key Steps in the Analysis

### 1. Data Loading and Inspection
```python
import pandas as pd

df = pd.read_csv('C:/Users/user/OneDrive/Desktop/books_toscrape.csv')
print(df.info())
print(df.describe())
print(df.head())
