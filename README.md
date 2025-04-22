# SkyGeni Data Engineer Assignment – Client Subscription Insights Analysis

The goal of the Data Engineer assignment was to analyze subscription, industry, payment, and financial data to extract business insights related to client behavior, renewal trends, inflation influence, and payment patterns.

As a beginner in data analysis, I’ve completed this assignment using Python and Jupyter Notebook, with as many comments as possible to explain my approach.

---

## Repository Contents

| File Name                                                        | Description |
|------------------------------------------------------------------|-------------|
| `Skygeni Data Engineer Assignment – Client & Industry Insights.ipynb` | Main notebook with step-by-step analysis |
| `industry_client_details.csv`                                    | Industry and client mapping |
| `subscription_information.csv`                                   | Subscription type, duration, and renewal |
| `payment_information.csv`                                        | Payment amounts, dates, and methods |
| `finanical_information.csv`                                      | Inflation and GDP data by quarter |
|`Assignment Info.docx` | Document with the assignment questions |

---

## Assignment Questions and My Answers

### 1. **How many finance lending and blockchain clients does the organization have?**

![image](https://github.com/user-attachments/assets/bf4a22ed-d9c2-4cf2-9f82-11f94d131150)


Filtered the industry data by category and counted unique client IDs.

---

### 2. **Which industry has the highest renewal rate?**

![image](https://github.com/user-attachments/assets/639c8eaf-ff9d-41d3-b16a-0d41322e7ba8)


Merged industry and subscription data and calculated the renewal percentage by industry.

---

### 3. **What was the average inflation rate when subscriptions were renewed?**

- **Answer**: Calculated by mapping `end_date` of renewed subscriptions to the corresponding quarter in financial data.
   
![image](https://github.com/user-attachments/assets/d507a7d9-d632-4786-b9e5-f9a7d3329c25)


Used financial date ranges to find matching inflation rates during renewal time.

---

### 4. **What is the median amount paid each year for all payment methods?**

- Calculated medians for each combination of `year` and `payment_method`.
  
  ![image](https://github.com/user-attachments/assets/cdd963a7-e87f-4865-a12f-546fe047f0cb)

- Created a line plot to show how median payments varied across years and methods.
  
  ![image](https://github.com/user-attachments/assets/9969653a-c244-4f73-a485-255a5b2bf20a)


---

## 🛠️ Tools and Libraries Used

- **Python 3.7**
- **Jupyter Notebook**
- **pandas, numpy**
- **matplotlib, seaborn**
