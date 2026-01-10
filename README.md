
## 📄 Actual Dataset

| OrderID | OrderDate | Region | State | City | Category | SubCategory | Sales | Quantity | Discount | Profit |
|--------|-----------|--------|-------|------|----------|------------|-------|----------|----------|--------|
| O001 | 1/1/2025 | South | Telangana | Hyderabad | Technology | Phones | 25000 | 2 | 0.05 | 4500 |
| O002 | 2/1/2025 | West | Maharashtra | Mumbai | Furniture | Chairs | 18000 | 3 | 0.10 | 3200 |
| O003 | 2/1/2025 | North | Delhi | New Delhi | Office Supplies | Paper | 4000 | 10 | 0 | 1200 |
| O004 | 3/1/2025 | East | West Bengal | Kolkata | Technology | Laptops | 55000 | 1 | 0.15 | 7000 |
| O005 | 3/1/2025 | South | Tamil Nadu | Chennai | Furniture | Tables | 22000 | 2 | 0.05 | 2800 |
| O006 | 4/1/2025 | West | Gujarat | Ahmedabad | Office Supplies | Binders | 6000 | 5 | 0 | 1500 |
| O007 | 4/1/2025 | North | Uttar Pradesh | Lucknow | Technology | Accessories | 9000 | 4 | 0.10 | 1800 |
| O008 | 5/1/2025 | East | Bihar | Patna | Office Supplies | Labels | 3000 | 6 | 0 | 900 |
| O009 | 5/1/2025 | South | Karnataka | Bengaluru | Technology | Phones | 32000 | 3 | 0.05 | 5200 |
| O010 | 6/1/2025 | West | Rajasthan | Jaipur | Furniture | Bookcases | 26000 | 2 | 0.20 | 3500 |
| O011 | 6/1/2025 | North | Punjab | Amritsar | Office Supplies | Storage | 7500 | 5 | 0 | 1600 |
| O012 | 7/1/2025 | East | Odisha | Bhubaneswar | Technology | Accessories | 8500 | 4 | 0.10 | 1700 |
| O013 | 7/1/2025 | South | Kerala | Kochi | Furniture | Chairs | 19500 | 3 | 0.05 | 3100 |
| O014 | 8/1/2025 | West | Madhya Pradesh | Indore | Office Supplies | Paper | 4500 | 8 | 0 | 1100 |
| O015 | 8/1/2025 | North | Haryana | Gurugram | Technology | Laptops | 60000 | 1 | 0.10 | 8500 |
| O016 | 9/1/2025 | East | Assam | Guwahati | Furniture | Tables | 21000 | 2 | 0.05 | 2600 |
| O017 | 9/1/2025 | South | Andhra Pradesh | Vijayawada | Office Supplies | Binders | 6800 | 6 | 0 | 1400 |
| O018 | 10/1/2025 | West | Goa | Panaji | Technology | Phones | 28000 | 2 | 0.15 | 3900 |
| O019 | 10/1/2025 | North | Himachal Pradesh | Shimla | Office Supplies | Labels | 3200 | 7 | 0 | 950 |
| O020 | 11/1/2025 | East | Jharkhand | Ranchi | Furniture | Bookcases | 24000 | 2 | 0.10 | 3300 |
| O021 | 11/1/2025 | South | Telangana | Warangal | Technology | Accessories | 7800 | 3 | 0.05 | 1400 |
| O022 | 12/1/2025 | West | Maharashtra | Pune | Office Supplies | Storage | 9200 | 4 | 0 | 1900 |
| O023 | 12/1/2025 | North | Rajasthan | Udaipur | Furniture | Chairs | 16500 | 2 | 0.10 | 2700 |
| O024 | 13/1/2025 | East | West Bengal | Siliguri | Office Supplies | Paper | 3800 | 9 | 0 | 1000 |
| O025 | 14/1/2025 | South | Tamil Nadu | Coimbatore | Technology | Phones | 30000 | 2 | 0.05 | 4800 |
| O026 | 15/1/2025 | West | Gujarat | Surat | Furniture | Tables | 20000 | 2 | 0.05 | 2600 |
| O027 | 16/1/2025 | North | Uttar Pradesh | Noida | Technology | Laptops | 58000 | 1 | 0.10 | 7800 |
| O028 | 17/1/2025 | East | Bihar | Gaya | Office Supplies | Binders | 6400 | 5 | 0 | 1350 |
| O029 | 18/1/2025 | South | Karnataka | Mysuru | Furniture | Bookcases | 23000 | 2 | 0.15 | 3200 |
| O030 | 19/1/2025 | West | Rajasthan | Jodhpur | Technology | Accessories | 8700 | 4 | 0.10 | 1600 |

---

## 1️⃣ Conditional Formatting, IF, COUNTIF, SUMIF, AVERAGE, CONCAT

| Function | Purpose | Syntax | Example Formula |
|--------|--------|--------|----------------|
| Conditional Formatting | Highlight Sales > 50,000 | Greater Than | Apply on `H2:H31 > 50000` |
| IF | Category based condition | `IF(condition,value_if_true,value_if_false)` | `=IF(F2="Technology","Good","False")` |
| COUNTIF | Count Technology orders | `COUNTIF(range,criteria)` | `=COUNTIF(F2:F31,"Technology")` |
| SUMIF | Total Sales of Technology | `SUMIF(range,criteria,sum_range)` | `=SUMIF(F2:F31,"Technology",H2:H31)` |
| AVERAGE | Average Sales | `AVERAGE(range)` | `=AVERAGE(H2:H31)` |
| CONCAT | Combine State & City | `CONCAT(text1,text2)` | `=CONCAT(D2,"-",E2)` |

---

## 2️⃣ INDEX, MATCH, UNIQUE, IFS, COUNTIFS, SUMIFS, AVERAGEIFS

| Function | Purpose | Example Formula |
|-------|--------|----------------|
| INDEX + MATCH | OrderID where Sales = 6000 | `=INDEX(A2:A31,MATCH(6000,H2:H31,0))` |
| MATCH | Position of Sales = 4000 | `=MATCH(4000,H2:H31,0)` |
| UNIQUE | Unique Regions | `=UNIQUE(C2:C31)` |
| IFS | Sales classification | `=IFS(H2>50000,"High",H2>20000,"Medium",TRUE,"Low")` |
| COUNTIFS | Technology orders in South | `=COUNTIFS(F2:F31,"Technology",C2:C31,"South")` |
| SUMIFS | Sales of Technology in South | `=SUMIFS(H2:H31,F2:F31,"Technology",C2:C31,"South")` |
| AVERAGEIFS | Avg Sales of Furniture in West | `=AVERAGEIFS(H2:H31,F2:F31,"Furniture",C2:C31,"West")` |

---

## 3️⃣ VLOOKUP, HLOOKUP, XLOOKUP, COUNT, COUNTA

| Function | Purpose | Example Formula |
|--------|--------|----------------|
| VLOOKUP | Sales for OrderID O009 | `=VLOOKUP("O009",A2:K31,8,FALSE)` |
| HLOOKUP | Sales from row 10 | `=HLOOKUP("Sales",A1:K31,10,FALSE)` |
| XLOOKUP | Profit for O015 | `=XLOOKUP("O015",A2:A31,K2:K31)` |
| COUNT | Count numeric Sales | `=COUNT(H2:H31)` |
| COUNTA | Count OrderIDs | `=COUNTA(A2:A31)` |

---

## 4️⃣ Text Functions

| Function | Example Formula |
|--------|----------------|
| LEFT | `=LEFT(A2,2)` |
| MID | `=MID(A2,2,3)` |
| RIGHT | `=RIGHT(A2,2)` |
| LEN | `=LEN(E2)` |
| SUBSTITUTE | `=SUBSTITUTE(F2," ","_")` |
| SEARCH | `=SEARCH("a",E2)` |
| ISNUMBER | `=ISNUMBER(SEARCH("a",E2))` |

---

## 5️⃣ Date & Time Functions

| Function | Example Formula |
|--------|----------------|
| TODAY | `=TODAY()` |
| NOW | `=NOW()` |
| YEAR | `=YEAR(B2)` |
| MONTH | `=MONTH(B2)` |
| NETWORKDAYS | `=NETWORKDAYS("1/1/2025","31/1/2025")` |
| EOMONTH | `=EOMONTH(B2,0)` |

---

## 6️⃣ Advanced & Dynamic Functions

| Function | Example Formula |
|--------|----------------|
| OFFSET | `=OFFSET(H2,2,0)` |
| CHOOSE | `=CHOOSE(2,"South","West","North","East")` |
| LET | `=LET(x,H2:H31,MAX(x))` |
| MAX | `=MAX(H2:H31)` |
| SORT | `=SORT(H2:H31,1,-1)` |
| SORTBY | `=SORTBY(A2:A31,H2:H31,-1)` |
| RANK | `=RANK(H2,H2:H31,0)` |

---


## 8️⃣ Excel Tools (Conceptual)

### 📊 Pivot Table
- Rows: Region → SubCategory  
- Values: Sales, Profit, Quantity  

### 🎯 What-If Analysis (Goal Seek)
- Set Cell: Profit  
- To Value: 10000  
- By Changing: Sales  

### ✔ Data Validation
- Quantity: Whole Number (1–10)

### ➕ Subtotals
```excel
=SUBTOTAL(9,H2:H31)
