# **Hospitality Revenue Analysis – AtliQ Grands**  
### **📊 Data-Driven Insights for Strategic Revenue Management**  

## **📌 Project Overview**  
AtliQ Grands, a luxury hotel chain in India, has been facing a decline in revenue and market share due to strategic competition and management inefficiencies. To regain traction, they seek **data-driven insights** to optimize revenue strategies.  


📌 **Live Dashboard:** [🔗 Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOWE4ZTgzNTMtZTg1Yy00N2Q1LWE4YmEtMTAyMjczOTBkNDMxIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)  

---

## **📈 Key Insights & Findings**  
1️⃣ **Mumbai leads revenue generation** – ₹669M, followed by Bangalore, Hyderabad, and Delhi.  
2️⃣ **AtliQ Exotica performs best** with ₹320M revenue, an occupancy rate of 57%, and cancellation rate of 24.4%.  
3️⃣ **AtliQ Bay has the highest occupancy** at **66%**.  
4️⃣ **Week 24 recorded peak revenue** at **₹139.6M**.  
5️⃣ **Elite rooms dominate bookings** but also show a **high cancellation rate**.  
6️⃣ **AtliQ lost ₹298M due to cancellations** – cancellation policies need refinement.  

---

## **📊 Data Modeling**  
### **🔹 Entity Relationships & Structure**  
![Data Modeling](INSERT_YOUR_IMAGE_LINK_HERE)  

Our **data model** includes the following **fact and dimension tables**:  

### **📂 Dimension Tables**  
| Table Name   | Key Columns |
|-------------|------------|
| `dim_date`  | `date`, `Day`, `Day_type` |
| `dim_hotels`  | `category`, `city`, `property_id`, `property_name` |
| `dim_rooms`  | `room_class`, `room_id` |
| `Day Table`  | `Day`, `Order` |

### **📊 Fact Tables**  
| Table Name | Key Columns |
|-----------|------------|
| `Fact_Bookings`  | `booking_id`, `booking_date`, `booking_platform`, `booking_status`, `check_in_date`, `checkout_date`, `no_guests`, `property_id`, `ratings_given`, `revenue_generated`, `revenue_realized`, `room_category` |
| `Fact_aggregated_Bookings`  | `capacity`, `check_in_date`, `property_id`, `room_category`, `successful_bookings` |

### **📈 Key Measures & Metrics**  
Our calculated metrics allow us to track key revenue and occupancy indicators:  
✔️ `ADR (Average Daily Rate)`  
✔️ `RevPAR (Revenue Per Available Room)`  
✔️ `Occupancy %`  
✔️ `Cancellation Rate`  
✔️ `Revenue Loss due to Cancellation`  
✔️ `Booking % by Platform`  
✔️ `Week-over-Week Performance Trends`  

✔️ **20+ DAX Measures Created** to calculate KPIs such as **RevPAR, ADR, Occupancy Rate, Realization %**, and trend analysis.  

---

### **🔗 Relationships & Business Impact**  
- **Fact tables are linked to dimension tables using primary keys** for **efficient data slicing and filtering**.  
- **Aggregated measures** like **ADR, Occupancy %, RevPAR** utilize `Fact_Bookings` and `Fact_aggregated_Bookings`.  
- **Temporal analysis** is driven by `dim_date` for **week-over-week and monthly trends**.  
- **Room class and booking platform segmentation** help optimize targeted **pricing strategies**.  

---

## **📊 Dashboard Visuals**  
### **🔹 Data Modelling**  

![Data Modelling](https://github.com/SachinSavkare/Power-Bi-AtliQ-Hospitality-Analtysis/blob/main/Data%20Modelling%20and%20Measures.JPG) 

### **🔹 Overall Analysis : Revenue & Booking Analysis**  

![Revenue Analysis](
https://github.com/SachinSavkare/Power-Bi-AtliQ-Hospitality-Analtysis/blob/main/Overall%20Analysis.JPG)  

- **Trend indicators highlight revenue growth & declines.**  
- **Cancellation impact visualized to identify revenue leakages.**  

### **🔹 Weekly Revenue Trends**  

![Weekly Trends](
https://github.com/SachinSavkare/Power-Bi-AtliQ-Hospitality-Analtysis/blob/main/Weekly%20Analysis.JPG)  

- **Week-over-week comparisons drive strategic planning for peak periods.**  

### **🔹 Property Performance Breakdown**  

![Property Analysis](
https://github.com/SachinSavkare/Power-Bi-AtliQ-Hospitality-Analtysis/blob/main/Property%20Analysis.JPG)  

- **Property-wise deep dive identifies top performers & areas of improvement.**  

---

## **🔍 Business Recommendations**  
💡 **Optimize Elite Room Type Strategy** – High revenue potential but high cancellations.  
💡 **Strengthen partnerships with OTA platforms** – "MakeMyTrip" and "LogTrip" contribute significantly to revenue.  
💡 **Revenue dipped by 28.17% in the last 4 days** – Targeted campaigns needed.  
💡 **Occupancy rates in June dipped by 0.24% due to high cancellations (25.09%)** – Improve cancellation policies.  

---

## **🎓 What I Learned from This Project**  
1️⃣ **Building a Calendar Visual** – Using the Matrix table creatively to generate a **calendar-style visualization** for better insights.  
2️⃣ **Understanding Cancellation Policies** – Deep-diving into industry standards to analyze cancellation trends and impact on revenue.  
3️⃣ **Advanced UI Techniques** – Using **Bookmarks & Selections** for interactive page navigation and filter clearing.  
4️⃣ **Color Consistency & Branding** – Implementing **color palettes** for a cohesive dashboard design, enhancing user experience.  
5️⃣ **Data Storytelling** – Turning raw numbers into **actionable business narratives** that help stakeholders make informed decisions.  

---

## **🛠️ Tech Stack Used**  
✅ **Power BI** – Dashboard creation, DAX formulas, and visualization.  
✅ **SQL** – Data transformation, query optimization.  
✅ **Excel** – Pre-analysis, dataset validation.  
✅ **DAX** – Creating dynamic measures like **ADR, RevPAR, Occupancy %, Trend Analysis**.  
✅ **Power Query** – Data cleaning and transformation before modeling.  

---

## **🎯 Skills Developed**  
✔️ **Business Analysis** – Understanding hospitality metrics like ADR, RevPAR, Occupancy % to drive insights.  
✔️ **Data Modeling** – Structuring relationships for efficient filtering and analysis.  
✔️ **Dashboard Aesthetics** – Designing visually appealing dashboards using **color palettes, smart narration, and UI refinement**.  
✔️ **Storytelling with Data** – Presenting insights in a way that drives **actionable decisions** for stakeholders.  
✔️ **Advanced DAX** – Iterative refinement of formulas for **Week-over-Week comparisons, revenue breakdowns, and trend analysis**.  
✔️ **Stakeholder Perspective** – Designing solutions that align with business **goals, usability, and impact**.  

---


