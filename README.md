# 🍽️ Predictive Restaurant Recommender

A machine learning-based recommendation engine that predicts **which restaurant a customer is most likely to order from**, based on their **location**, **order history**, and **vendor features**. This project was built as part of a **real-world data science internship assignment**.

## 📌 Problem Statement

Given customer, location, and vendor data, the objective is to recommend the most likely restaurant (vendor) a customer will order from in the future.

## 📁 Project Structure

```bash
predictive_restaurant_recommender/
│
├── Data/
│   ├── orders.csv
│   ├── train_customers.csv
│   ├── train_locations.csv
│   ├── train_orders.csv
│   ├── test_customers.csv
│   ├── test_locations.csv
│   └── vendors.csv
│
├── Model/
│   ├── restaurant_recommender_model.pkl
│   └── label_columns.pkl
│
├── Output/
│   └── predicted_vendors.csv
│
├── predictive_restaurant_recommender.ipynb  # Main notebook
├── requirements.txt                         # Python dependencies
├── .gitignore
└── README.md
````

## 🚀 How to Run the Project

1. **Clone the repo**:

   ```bash
   git clone https://github.com/ishasahlot/predictive_restaurant_recommender.git
   cd predictive_restaurant_recommender
   ```

2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**:
   Open `predictive_restaurant_recommender.ipynb` in Jupyter Notebook or VS Code and run all cells.

## 🔍 Methodology

1. **Data Loading & Exploration**
   Merged multiple datasets for customers, orders, vendors, and locations.

2. **Preprocessing**

   * Label encoding for categorical variables
   * Handled missing values
   * Removed irrelevant or duplicate columns

3. **Feature Engineering**
   Created a feature-rich dataset by aggregating customer and vendor interactions.

4. **Model Building**

   * Used **Random Forest Classifier**
   * Trained on historical customer-vendor orders
   * Tuned and evaluated for accuracy

5. **Prediction Output**
   Final predictions were stored in `predicted_vendors.csv` in the required format:

   ```
   customer_id,predicted_vendor
   4958,33
   4302,33
   ...
   ```

## 📦 Technologies Used

* **Language**: Python 3.11
* **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib
* **Tools**: Jupyter Notebook, GitHub

## ✅ Results

* Built a working model with reasonable accuracy for vendor prediction.
* Generated submission-ready output file for unseen customer IDs.
* Gained hands-on experience in **data wrangling, machine learning, and recommendation systems**.

## 💡 Future Improvements

* Explore deep learning-based recommenders (e.g. embeddings, neural CF)
* Improve accuracy by incorporating session-based features or delivery timing
* Add UI for real-time recommendations

## 🙋‍♀️ Author

**Isha Sahlot**
Aspiring Business Analyst & Data Science Enthusiast
[GitHub](https://github.com/ishasahlot) | [LinkedIn](https://www.linkedin.com/in/ishasahlot/)


## 📌 License

This project is for **educational purposes only**.

````

### ✅ How to Add It to Your GitHub

1. In VS Code terminal:

```bash
touch README.md
````

2. Paste the above content into `README.md`.

3. Save → Commit → Push:

```bash
git add README.md
git commit -m "Added project README"
git push origin main
```
