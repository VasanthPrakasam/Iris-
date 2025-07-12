---
# **🌷 Iris Dataset Overview**  
A classic dataset for **classification tasks**, predicting iris species based on sepal/petal measurements.  

---

## **📊 Column Descriptions**  

| Column | Description | Data Type |  
|--------|-------------|-----------|  
| `sepal_length` | Length of the sepal (cm) | `float64` |  
| `sepal_width` | Width of the sepal (cm) | `float64` |  
| `petal_length` | Length of the petal (cm) | `float64` |  
| `petal_width` | Width of the petal (cm) | `float64` |  
| `species` | Iris species (`setosa`, `versicolor`, `virginica`) | `object` → `int64` (encoded) |  

---

## **🧹 Data Preprocessing**  

### **✅ Cleaning Steps**  
1. **No missing values** → All 150 entries are complete.  
2. **No spelling errors** → Consistent labels in `species`.  
3. **Encoding** → Converted `species` to numeric using `OrdinalEncoder`.  

### **🔍 Before vs. After**  

**Before Cleaning** (`species` as object):  
```python
RangeIndex: 150 entries  
Data columns (total 5):  
 #   Column        Non-Null Count  Dtype    
---  ------        --------------  -----    
 0   sepal_length  150 non-null    float64  
 1   sepal_width   150 non-null    float64  
 2   petal_length  150 non-null    float64  
 3   petal_width   150 non-null    float64  
 4   species       150 non-null    object   # ← Categorical
```

**After Cleaning** (`species` as float64):  
```python
 4   species       150 non-null    float64  # ← Numeric (encoded)
```

---

## **🎯 Conclusion**  
✔ **Perfect for classification** (e.g., logistic regression, decision trees).  
✔ **No preprocessing needed** beyond encoding.  
✔ **Key Use Case**: Predict species from sepal/petal dimensions.  

---
