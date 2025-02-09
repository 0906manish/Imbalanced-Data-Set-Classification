# 📌 Fraud Detection Using Dynamic Prime-Based Clustering

This project applies **Dynamic Prime-Based Clustering** to detect fraudulent transactions in a **credit card fraud detection dataset**. The approach leverages **mathematical transformations using prime numbers** to group transactions into clusters and identify **anomalies (fraudulent transactions)**.

---

## 📌 Features
✔ **Clustering Based on Prime Factorization:** Transactions are grouped using prime-based transformations.  
✔ **Anomaly Detection:** Transactions in **small or unique clusters** are flagged as fraudulent.  
✔ **Custom Threshold for Fraud Detection:** Set the threshold for defining fraudulent clusters.  
✔ **Matplotlib Visualization:** Displays **clusters** and **fraudulent transactions**.  
✔ **Implemented in Jupyter Notebook (`clustering.ipynb`)** for easy execution and visualization.  

---

## 📌 Dataset 📂
- Kaggle Dataset: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- The model uses a **CSV file** containing **credit card transactions**.
- The file should have a column named **"Amount"**, which contains transaction amounts.
- The model uses a **CSV file** containing **credit card transactions**.
- The file should have a column named **"Amount"**, which contains transaction amounts.

---

## 📌 Installation & Setup 🚀
### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/0906manish/Imbalanced-Data-Set-Classification.git
cd Imbalanced-Data-Set-Classification
```

### **2️⃣ Install Dependencies**
```sh
pip install pandas matplotlib
```

### **3️⃣ Add the Dataset**
- Place your **credit card transaction CSV file** inside the project directory.
- Ensure the CSV has a **column named "Amount"**.

### **4️⃣ Run the Notebook**
- Open **Jupyter Notebook**
```sh
jupyter notebook
```
- Open and run **clustering.ipynb**.

---

## 📌 How It Works 🔬
1. **Prime-Based Clustering:**  
   - Each transaction amount is transformed based on the **largest power of a prime number** that divides it.
   - The transaction is assigned to a **cluster based on the smallest transformation value**.

2. **Fraud Detection:**  
   - Clusters with very few transactions (below a set threshold) are flagged as **fraudulent**.
   - These clusters indicate **anomalous spending behavior**.

3. **Visualization:**  
   - A **bar chart** shows the distribution of transactions per cluster.
   - A **red bar chart** highlights **fraudulent transactions**.

---

## 📌 Example Output 📊
```
Fraudulent Transactions:
Transaction: 5000, Cluster: Cluster (Divisible by 11 smallest)
Transaction: 7500, Cluster: Cluster (Divisible by 13 smallest)
```

### **Cluster Visualization**
![Cluster Visualization](cluster_distribution.png)

### **Fraudulent Transactions**
![Fraud Detection](fraud_detection.png)

---

## 📌 Customization ⚙️
- Modify the **fraud threshold** in `clustering.ipynb`:
```python
fraudulent_transactions = detect_fraudulent_transactions(transaction_amounts, clusters, threshold=3)
```
- Change the **input file path** if needed:
```python
input_file = "creditcard.csv"
```

---

## 📌 Contributing 🤝
Want to improve this project? Fork the repo and submit a **pull request**!

---

## 📌 License 📜
This project is licensed under the **MIT License**.

---

## 📌 Author ✍️
**[Manish](https://github.com/0906manish)**  
📧 manishaamt0906@gmail.com  


