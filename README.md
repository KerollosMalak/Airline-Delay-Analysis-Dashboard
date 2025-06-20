# Airline Delay Causes Analysis - Power BI Dashboard
---

## Project Overview

This project presents a comprehensive Power BI dashboard designed to analyze and visualize the causes and trends of airline delays, cancellations, and diversions. Leveraging a publicly available dataset from Kaggle, this solution provides actionable insights into the factors impacting airline punctuality, helping identify key areas for operational improvements.

---

**Key features of the dashboard include:**

* **Overall Flight Performance:** Track total flights, delayed flights, cancellations, and diversions.
* **Delay & Cancellation Rates:** Monitor performance metrics over time and across different dimensions.
* **Detailed Delay Cause Analysis:** Break down delay minutes by specific causes (Carrier, Weather, National Airspace System (NAS), Security, Late Aircraft).
* **Carrier & Airport Specific Insights:** Analyze performance and delay causes for individual airlines and airports.
* **Time-based Trends:** Observe seasonal and monthly patterns in flight disruptions.

---

## Data Source

The dataset used for this analysis is sourced from:
**Kaggle:** [Airline Delay Causes](https://www.kaggle.com/datasets/giovamata/airlinedelaycauses)

This dataset typically includes monthly summary statistics for U.S. domestic flights, detailing arrival flights, delays (15+ minutes), cancellations, diversions, and the minutes of delay attributed to various causes.

---

## Technical Stack & Methodologies

* **Power BI Desktop:** The primary tool used for data modeling, DAX calculations, and dashboard visualization.
* **Power Query :** Used extensively for data extraction, transformation, and loading (ETL) processes, including data cleaning, type conversion, and custom column creation.
* **DAX (Data Analysis Expressions):** Utilized to create robust measures and calculated columns for key performance indicators (KPIs) and complex analytical calculations.
* **Star Schema Data Modeling:** Implemented a star schema design to optimize query performance, improve data clarity, and facilitate easier analysis. This includes:
    * **Fact Table:** `Flight Delays` (containing metrics like `arr_flights`, `arr_del15`, `arr_delay`, etc.)
    * **Dimension Tables:** `DimDate`, `DimCarrier`, `DimAirport` (created using Power Query for better context and filtering).

---

## Dashboard Screenshots

Here are some snapshots of the Power BI dashboard:

### 1. Overview Dashboard![overview](https://github.com/user-attachments/assets/9cc9fa77-11f0-402b-b3de-fba8a7ca15f8)

*Provides a high-level summary of total flights, delays, and cancellations, along with key performance rates and top contributing airports.*

### 2. Delay Overview
![delay overview](https://github.com/user-attachments/assets/be5b4747-74b8-4dbc-92a0-80914a33596b)


*Focuses on the distribution of delays by their primary causes, offering a quick understanding of the biggest contributors to flight disruptions.*

### 3. Delay in Details
![delay in details](https://github.com/user-attachments/assets/06a713df-7a8c-44d5-b104-524434c177e4)

*Offers a deeper dive into delay causes, allowing for analysis by specific airports and carriers, providing granular insights into operational pain points.*

### 4. Semantic Model (Star Schema)
![Semantic model](https://github.com/user-attachments/assets/ac8cc865-36a5-47ad-b459-156d5f49fbc9)

*A visual representation of the underlying star schema data model, showcasing the relationships between fact and dimension tables.*

---

## Key Insights & Potential Decisions

Based on the analysis from this dashboard, several critical insights emerge:

* **Dominant Delay Causes:** The dashboard consistently highlights **National Airspace System (NAS) delays** and **Late Aircraft delays** as significant contributors to overall flight disruption minutes. This suggests challenges related to air traffic control, airport congestion, and the cascading effect of delayed inbound flights.
* **Seasonal Trends:** Specific periods (e.g., winter months) often show spikes in weather-related delays and overall disruptions.
* **Carrier/Airport Specific Issues:** By filtering down, it's possible to identify particular airlines or airports that disproportionately contribute to certain types of delays.

---

**Actionable Decisions:**

* **For Airlines:** Focus on strategies to mitigate "Late Aircraft" delays, such as optimizing turnaround times, improving maintenance schedules, and potentially adjusting flight schedules to build in more buffer time for high-risk routes. Additionally, work with airport authorities to address shared infrastructure challenges contributing to NAS delays.
* **For Airports & Regulators:** Address capacity constraints and air traffic management inefficiencies that lead to NAS delays, especially during peak hours or adverse conditions. Investments in modernizing air traffic control systems could yield significant improvements.
* **Collaborative Efforts:** The interdependence of "Late Aircraft" and "NAS" delays underscores the need for greater collaboration between airlines, airports, and air traffic control to develop holistic solutions for improving punctuality across the aviation network.

---
##  Download the Power BI Report File (.pbix):
   *Due to its large size, the `.pbix` file is hosted on Google Drive.
    ** **Download the Power BI Report Here:** [**[Link to your Google Drive Power BI file]**](https://drive.google.com/drive/folders/1O7U-3OMSH1igK_TnY2vhVYEFNrNI4cqL?usp=drive_link)
        * *

**Open the Power BI file:**
    * Open the downloaded `.pbix` file in Power BI Desktop.
    * You might need to refresh the data connection if the data files were placed in a different directory than specified in Power Query.

--

## 🧑‍💻 Author

**Kerollos Malak**  
Data Analyst  | Python, SQL, Excel ,Power BI  
📧 keroartph@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/kerollos-malak-207998211/) | [GitHub](https://github.com/KerollosMalak)
