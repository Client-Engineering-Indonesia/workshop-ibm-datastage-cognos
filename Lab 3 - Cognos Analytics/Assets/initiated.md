# 🧠 IBM Cognos Analytics Dashboard — Step-by-Step Guide  
*(Following image sequence: 0 → 21)*  

This guide walks through how to build a Cognos dashboard exactly as shown in your provided images.

---

## 🪜 Step-by-Step Instructions

---

### Step 1 – Add the ID field
From **Sources → Fields**, drag the **`ID`** field into your canvas. This provides a unique identifier for grouping and validation.  
![1. add id]()

---

### Step 2 – Duplicate and delete extra columns
Duplicate your table or widget. Right-click → **Delete column** to remove unnecessary fields so you can isolate metrics.  
![2. duplicate and right clic del column]()

---

### Step 3 – Add Loan Amount (Average)
Drag **`Loan Amount`** into the Summarize widget. Set aggregation to **Average (Avg)** instead of Sum.  
![3. add loan amount and summa avg]()

---

### Step 4 – Rename data item
Rename the field to something clear, e.g., **`Loan Amount (Avg)`** for better readability.  
![4. Customize loan amount data name to avg]()

---

### Step 5 – Check average result
Verify that the value displayed matches your expectations (filters, context, aggregation).  
![5. Examp avg loan amount]()

---

### Step 6 – Remove Income column
Clean up by removing redundant columns (e.g., the 4th **Income** column).  
![6. remove col 4 income]()

---

### Step 7 – Create Min Income summary
Add **`Income`** into a Summarize widget and set aggregation to **Minimum**.  
![7. Min Income]()

---

### Step 8 – Rename Min Income
Rename the measure to **`Income (Min)`** to maintain naming consistency.  
![8. income name custom]()

---

### Step 9 – Verify example value
Inspect the resulting minimum value for correctness.  
![9. example min income ]()

---

### Step 10 – Add a Pie Chart
Add a **Pie** visualization to analyze categorical distribution (e.g., **Application Channel**, **Region**).  
![9. Pie chart select]()

---

### Step 11 – Drag and drop “Applied Online”
Add **`Applied Online`** into your Pie (or Bar) to visualize **Online vs. Non-Online** applications.  
![10. drag drop applied online]()

---

### Step 12 – Open Visualization panel
Open the **Visualization** properties panel to adjust labels, legends, and formats.  
![11. visualization]()

---

### Step 13 – Use Custom options
Switch to **Custom** in properties to fine-tune style, number formats, and labels.  
![12. Custom]()

---

### Step 14 – Select Gas Gauge Chart
Add a **Gauge** visualization for an executive KPI (e.g., **DTI**, **Approval Rate**, **Avg Loan**).  
![13. Select gas Gauge chart]()

---

### Step 15 – Create a new calculation
Right-click in the field list → **Create calculation** to compute derived KPIs.  
![14. Right Click and create calculation]()

---

### Step 16 – Name your calculation
Give it a clear name such as **`Debt to Income %`**.  
![14.1 name calculation]()

---

### Step 17 – Edit calculation
Re-open the **Calculator editor** to refine your expression or adjust aggregation behavior.  
![15. select calculator edition]()

---

### Step 18 – Select Summaries in Components
Within the calculation editor, go to **Components → Summaries** to use aggregated measures (Avg, Min, Sum).  
![16. select summaries in components]()

---

### Step 19 – Build the calculation
Write the Income average by calculation editor, for example:
```cognos
Total (INCOME)] / COUNT(INCOME)]
```

### Step 20 – Preview result
Click **Preview** to validate that the calculation returns the expected numeric output.  
![18. preview result]()

---

### Step 21 – Drag Income (Avg) into the Gauge
Drag your **Income (Avg)** field into the gauge widget as part of the measure or denominator.  
![19. drag and drop income average]()

---

### Step 22 – Drag Total Debt
Add **Total Debt** as the numerator or second component of your gauge.  
![20. drag and drop total debt]()

---

### Step 23 – Reorder fields
Swap the order of fields so the logic reads correctly (e.g., **Debt ÷ Income**).  
Check that gauge thresholds make visual sense.  
![21. drag and switch position income avg with total debt]()
