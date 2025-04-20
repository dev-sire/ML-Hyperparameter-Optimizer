# 🤖 Machine Learning Hyperparameter Optimization App (Regression Edition)

This web app provides a **simple and interactive interface** to perform hyperparameter tuning for regression models using **Random Forest Regressor**. Built with [Streamlit](https://streamlit.io/) and [Scikit-learn](https://scikit-learn.org/), it allows users to upload their dataset, tune hyperparameters, and visualize the impact on model performance — all in the browser.

---

## 📌 Features

- Upload your own CSV dataset or use a built-in example (Diabetes dataset)
- Select and tune key Random Forest hyperparameters:
  - `n_estimators`
  - `max_features`
  - `min_samples_split`
  - `min_samples_leaf`
  - `criterion` (`mse`, `mae`)
  - `bootstrap`
  - `oob_score`
  - `random_state`
- Perform **Grid Search Cross Validation**
- View performance metrics: **R² Score** and **Mean Squared Error**
- 3D interactive surface plot of hyperparameter tuning results using Plotly
- Download results as CSV

---

## 🧰 Technologies Used

- Python 3.8+
- Streamlit
- Scikit-learn
- NumPy
- Pandas
- Plotly

---

# Reproducing this web app
To recreate this web app on your own computer, do the following.

### Create conda environment
Firstly, we will create a conda environment called *mlopt*
```
conda create -n mlopt python=3.7.9
```
Secondly, we will login to the *mlopt* environement
```
conda activate mlopt
```
### Install prerequisite libraries

Download requirements.txt file

```
wget https://raw.githubusercontent.com/dataprofessor/ml-opt-app/main/requirements.txt

```

Pip install libraries
```
pip install -r requirements.txt
```

###  Download and unzip contents from GitHub repo

Download and unzip contents from https://github.com/dataprofessor/ml-opt-app/archive/main.zip

###  Launch the app

```
streamlit run app.py
```