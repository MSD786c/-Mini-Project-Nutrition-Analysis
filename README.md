
# 🍽️ Mini Project: Nutritional Insights from 500+ Foods

This project explores a dataset of **551 foods** with **35+ nutrients**, including calories, macros, vitamins, and minerals.  
The goal is to practice **data cleaning, exploratory data analysis (EDA), and visualization** using Python (Pandas, Seaborn, Matplotlib).

---

## 📂 Dataset
- **Source**: FOOD-DATA-GROUP1.csv (provided dataset)
- **Shape**: 551 foods × 35 nutrients
- **Columns include**:
  - `Caloric Value`, `Fat`, `Carbohydrates`, `Protein`, `Sugars`, `Dietary Fiber`
  - `Vitamins (A, B1–B12, C, D, E, K)`
  - `Minerals (Calcium, Iron, Magnesium, Potassium, Zinc, etc.)`
  - `Nutrition Density` score

---

## 🛠️ Steps Performed

### 1. Data Cleaning
- Dropped unnecessary index columns (`Unnamed: 0`, `Unnamed: 0.1`).
- Standardized food names (stripped & title-cased).
- Checked and dropped duplicates (none found).
- Converted all nutrient columns to numeric types.

✅ **Final dataset**: 551 foods × 35 columns.

---

### 2. Descriptive Statistics
- Average calories per food: `~237 kcal`
- Calorie range: **min = 3 kcal (Crayfish/Salmon raw)** → **max = 1578 kcal (General Tso’s Chicken)**
- Average protein: `~18 g`
- Average fat: `~11 g`
- Average carbs: `~16 g`

---

### 3. Insights from Analysis

#### 🔹 Calorie Insights
- Most foods fall in the range **100–400 kcal**.  
- Lowest-calorie foods: seafoods like raw salmon, crayfish.  
- Highest-calorie foods: fried/processed dishes (General Tso’s chicken).  

#### 🔹 Protein Insights
- Protein-rich foods include meats and legumes.  
- Top foods for **protein density (protein per calorie)** are lean seafoods.  

#### 🔹 Sugar & Carbohydrates
- Some foods are almost **100% sugar-based carbs**.  
- High sugar ratio foods stand out as clear outliers.  

#### 🔹 Nutrient Density
- Nutrient-dense foods aren’t always high-calorie.  
- Leafy greens and vegetables often deliver **high micronutrients per kcal**.

---

### 4. Visualizations
This project includes the following plots (Seaborn + Matplotlib):

- **Histogram**: distribution of calories, protein, fat, and carbs.  
- **Boxplot**: detecting outliers in calories across categories.  
- **Scatterplot**:  
  - Calories vs Protein  
  - Carbohydrates vs Sugars  
  - Calories vs Nutrition Density  
- **Correlation Heatmap**: relationships among nutrients.

---

## 📊 Example Plots

*(Add saved charts here, e.g., histograms, scatterplots, heatmaps)*

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.histplot(df_clean["Caloric Value"], bins=40, kde=True)
plt.title("Distribution of Caloric Values")
plt.show()
```

---

## 🚀 How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/food-nutrition-analysis.git
   cd food-nutrition-analysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

3. Open Jupyter Notebook:
   ```bash
   jupyter notebook 📊_Mini_Project_Nutrition_Analysis.ipynb
   ```

---

## ✅ Deliverables
- Cleaned dataset (`food_clean.csv`)
- Jupyter Notebook (`📊_Mini_Project_Nutrition_Analysis.ipynb`)
- Visualizations (`/charts/*.png`)
- GitHub README with summary + insights

---

## 📌 Key Takeaways
- Raw foods like seafood are among the lowest calorie per 100g.  
- Fried/processed dishes dominate the highest calorie end.  
- Protein density highlights lean protein sources.  
- Nutrient density shows that calories ≠ nutrition.

---


