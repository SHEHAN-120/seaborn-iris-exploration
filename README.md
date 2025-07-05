# 🌸 Iris Dataset Visualization with Seaborn & Matplotlib

This project performs **Exploratory Data Analysis (EDA)** and **visualization** on the classic **Iris dataset** using Python libraries **Seaborn** and **Matplotlib**.

It includes distribution plots, KDE plots, and pairwise visualizations that help understand the relationships between different features and species.

---

## 📊 Dataset

We use the built-in **Iris dataset** from the Seaborn library:

* Features:

  * `sepal_length`
  * `sepal_width`
  * `petal_length`
  * `petal_width`
* Target:

  * `species` (setosa, versicolor, virginica)

---

## 🔍 What’s Included

✔ Load dataset with `sns.load_dataset("iris")`
✔ Use `df.head()`, `len(df)` for overview
✔ Count species values: `df.species.value_counts()`
✔ Horizontal bar plot of species
✔ KDE plots for each numerical feature
✔ Distribution plot of `sepal_length`
✔ `pairplot` with hue by species

---

## 🖼️ Visualizations

### 📌 Species Count Plot (Horizontal Bar)

```python
df.species.value_counts().plot(kind='barh')
```

### 📌 KDE Plots for Features

```python
sns.kdeplot(df['sepal_length'], shade=True)
sns.distplot(df['sepal_length'])

for col in ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']:
    sns.kdeplot(df[col], shade=True)
```

## 🛠️ Technologies

* Python 3
* Seaborn
* Jupyter Notebook / Google Colab



## 🧪 Sample Output

* KDE plots showing the spread of sepal/petal features
* Bar plot of class distribution
* Pairwise plots showing clustering patterns by species



