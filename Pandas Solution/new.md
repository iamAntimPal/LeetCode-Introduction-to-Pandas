
# **2890. Reshape Data: Melt**  

## **Problem Statement**  
Write a solution to reshape the data so that each row represents sales data for a product in a specific quarter.

## **DataFrame Schema**  

| Column Name | Type   |
| ----------- | ------ |
| product     | object |
| quarter_1   | int    |
| quarter_2   | int    |
| quarter_3   | int    |
| quarter_4   | int    |

## **Example 1**  

### **Input:**  
```plaintext
+-------------+-----------+-----------+-----------+-----------+
| product     | quarter_1 | quarter_2 | quarter_3 | quarter_4 |
+-------------+-----------+-----------+-----------+-----------+
| Umbrella    | 417       | 224       | 379       | 611       |
| SleepingBag | 800       | 936       | 93        | 875       |
+-------------+-----------+-----------+-----------+-----------+
```  

### **Output:**  
```rb
+-------------+-----------+-------+
| product     | quarter   | sales |
+-------------+-----------+-------+
| Umbrella    | quarter_1 | 417   |
| SleepingBag | quarter_1 | 800   |
| Umbrella    | quarter_2 | 224   |
| SleepingBag | quarter_2 | 936   |
| Umbrella    | quarter_3 | 379   |
| SleepingBag | quarter_3 | 93    |
| Umbrella    | quarter_4 | 611   |
| SleepingBag | quarter_4 | 875   |
+-------------+-----------+-------+
```  

### **Explanation:**  
The DataFrame is reshaped from wide to long format. Each row represents the sales of a product in a quarter.

## **Constraints**  
- The input DataFrame has at most **1000 rows**.  
- The `product` column is always non-null.  
- The `quarter_1` to `quarter_4` columns contain **non-negative integer values**.  

## **Discussion**  
- **Melting Data**: Convert wide-format sales data into long-format where each row represents a unique product-quarter pair.  
- **Sorting**: The final output must be sorted by `product` and `quarter`.  

---

## 🎯 **How to Contribute**  
1. Fork the repository and clone it locally.  
2. Implement the solution and test it.  
3. Create a pull request with detailed explanations.  

## 📂 **File Structure**  
```rb
/solutions  
   ├── pivot_weather.py  
   ├── melt_sales.py  
   ├── README.md  
```  

## 🔥 **Want to Participate?**  
- Follow the discussions on GitHub.  
- Improve existing solutions and contribute new insights.  

## 🔗 **Useful Links**  
- [Pandas Documentation](https://pandas.pydata.org/docs/)  
- [Python Data Manipulation Guide](https://realpython.com/pandas-dataframe/)  

💡 **Let's learn, code, and grow together! 🚀**  