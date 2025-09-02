# Zomato Data Analysis - EDA Observations

## 📊 Dataset Information

### Main Dataset: `zomato.csv`
- **Records**: 9,551 restaurants
- **Columns**: 21 features
- **Memory Usage**: 1.5+ MB
- **Encoding**: Latin-1

### Supporting Dataset: `Country-Code.xlsx`
- **Records**: 15 countries
- **Purpose**: Maps country codes to country names

## 🔍 Key Observations from EDA Analysis

### 1. **Geographical Distribution**
- **Zomato maximum record and transaction from India**, after that USA and then United Kingdoms

### 2. **Rating System Analysis**
The rating system follows these ranges:
- **4.5 to 4.9**: Excellent
- **4.0 to 4.4**: Very Good
- **3.5 to 3.9**: Good
- **2.5 to 3.4**: Average
- **1.8 to 2.4**: Poor

### 3. **Zero Rating Analysis**
- **Maximum number of 0 rating from Indian customer**

### 4. **Online Delivery Services**
- **Online delivery only available in India and UAE**

### 5. **Data Quality**
- **Missing Values**: Only the "Cuisines" column has missing data (9 missing values out of 9,551 records)
- **Data Types**: 
  - float64: 3 columns
  - int64: 5 columns  
  - object: 13 columns

### 6. **City Distribution**
- Analysis includes top 5 cities by restaurant count
- Pie chart visualization shows restaurant concentration across major cities

## 📈 Analysis Performed

### 1. **Data Exploration**
- Missing value analysis
- Numerical and categorical variable exploration
- Feature relationship analysis

### 2. **Data Merging**
- Combined main dataset with country code mapping
- Created final dataset with country names

### 3. **Visualizations**
- Pie chart for top 3 countries by restaurant count
- Bar plot for rating distribution with color coding
- Pie chart for top 5 cities by restaurant count

## 🛠️ Technical Details

### Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- openpyxl

### Key Operations
- Data merging and joining
- Groupby operations for aggregations
- Statistical analysis
- Missing value detection
- Data type verification

## 📁 File Structure

```
zomato_data/
├── README.md                 # This documentation file
├── EDA_zomato.ipynb         # Main analysis notebook
└── data/
    ├── zomato.csv           # Main restaurant dataset
    └── Country-Code.xlsx    # Country mapping file
```

## 🚀 Getting Started

1. **Install Dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
   ```

2. **Run the Analysis**:
   - Open `EDA_zomato.ipynb` in Jupyter Notebook
   - Execute cells sequentially to reproduce the analysis

---

**Data Source**: Zomato Sample Dataset 
**Analysis Type**: Exploratory Data Analysis (EDA)
