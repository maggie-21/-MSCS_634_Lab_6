### MSCS_634_Lab_6
## MSCS 634 - Lab 6: Association Rule Mining with Apriori and FP-Growth

### 👤 Student Name:
Muluwork Geremew

### 🎓 Course:
MSCS 634 - Advanced Big Data and Data Mining

### 🧪 Lab Objective:
This lab explores association rule mining using the **Online Retail Dataset**. The focus is on extracting frequent itemsets and generating strong association rules using two popular algorithms:

- **Apriori Algorithm**
- **FP-Growth Algorithm**

The lab also emphasizes comparative analysis of the algorithms and uses visualizations to uncover and explain hidden patterns.

---

### 📈 Methods & Metrics:

#### Algorithms Implemented:
- Apriori
- FP-Growth

#### Evaluation Metrics:
- **Support**: Frequency of itemset occurrence
- **Confidence**: Probability of consequent given antecedent
- **Lift**: Strength of association between itemsets

#### Visualizations:
- Top frequent itemsets (Seaborn barplots)
- Association rules: Confidence vs. Lift (Scatter plot)

---

### 📊 Summary of Results:

#### 🔹 Top Frequent Itemsets:
- `white hanging heart t-light holder`
- `jumbo bag red retrospot`
- `regency cakestand 3 tier`
- `party bunting`
- `lunch bag red retrospot`

#### 🔹 Association Rules (Example):
| Antecedent                          | Consequent                          | Support | Confidence | Lift   |
|-------------------------------------|--------------------------------------|---------|------------|--------|
| (wooden heart christmas scandinavian) | (wooden star christmas scandinavian) | 0.0202  | 0.7229     | 27.46  |
| (pink regency teacup and saucer)   | (green regency teacup and saucer)   | 0.0270  | 0.8544     | 16.24  |

---

### 🔍 Key Insights:

- **FP-Growth** outperformed Apriori in execution speed while producing identical frequent itemsets.
- Top products revealed customer preferences for decorative home items.
- Strong association rules indicate common co-purchases (e.g., matching teacup sets).
- Rules with high lift and confidence (e.g., > 0.7 confidence and > 15 lift) suggest strong marketing recommendations.

---

### ⚠️ Challenges Faced:

- Dealing with sparse high-dimensional basket matrix (InvoiceNo × Product).
- Selecting appropriate `min_support` and `min_confidence` thresholds.
- Handling null values and transforming transactional data into one-hot format.

---

### 📂 Repository Contents:

- `Association_Rule.ipynb` – Jupyter Notebook with all code, plots, and explanations.

---

### ✅ How to Run:

1. Clone the repository.
2. Open `Association_Rule.ipynb` in Jupyter Notebook or VS Code.
3. Run all cells in order.
4. Ensure the following packages are installed:

```bash
pip install pandas numpy matplotlib seaborn mlxtend openxyl
restart the notebook kernel
