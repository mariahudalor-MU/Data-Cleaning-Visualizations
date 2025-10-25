# 📊 Consultant Project Data Analysis
A data analytics project demonstrating how Excel formulas, data modeling, and conditional logic can be used to consolidate, clean, and analyze consultant work data. This project simulates a real-world business intelligence workflow by merging multiple data sources, estimating missing values, and summarizing key performance insights.

🧾 Dataset Overview
The consolidated dataset integrates information from three sources:

#Table Name	# Description
C.data	Consultant details – Consultant ID, Name, Role
P.assignments	Project assignments – Consultant ID, Project ID, Hours Worked, Service Type
P.data	Project-level details – Project ID, Project Name, Category, Billable Rate
Data was merged using Excel lookup functions (VLOOKUP) to link related records by matching IDs, forming a single unified dataset for analysis.

🧰 Techniques & Tools
Data Cleaning

Removed duplicates with “Data → Remove Duplicates”

Estimated missing “Hours Worked” using logical and averaging formulas

Standardized Service Type labels and formatted date fields

Data Merging

Linked multiple sheets using VLOOKUP

Consolidated consultant and project records into a single dataset

Data Analysis

Estimated missing hours using:


=IF(ISBLANK(E2), AVERAGEIF($I:$I, I2, $E:$E), E2)
Summed total hours per service type using:


=SUMIF($I:$I, "Consulting", $E:$E)
Created pivot tables to summarize project and consultant performance

📈 Key Insights
Certain Service Types consistently logged fewer hours, suggesting underutilization or project imbalance.

Missing revenue entries were imputed accurately using consultant-level averages.

The consolidated dataset supports further visualization and KPI tracking in Power BI or Excel Dashboards.

💡 Learnings
This project demonstrates:

Data consolidation across multiple Excel sheets

The power of conditional and lookup formulas (IF, AVERAGEIF, VLOOKUP, SUMIFS)

Data imputation using formula logic

Building a foundation for advanced BI and Power Query workflows

🚀 Next Steps
Develop a Power BI dashboard with KPIs:

Total Hours

Revenue by Service Type

Consultant Utilization Rate

Automate imputation logic using Power Query

Extend profitability analysis by month or project type

📂 Project Files
File Name	Description
SampleData.xlsx	Merged dataset used for analysis
README.md	Documentation explaining project workflow
(Optional) Dashboard.pbix	Power BI dashboard visualization
👩🏽‍💻 Author
Mariah Udalor
Business Intelligence & Data Analyst
📍 Calgary, Canada

Passionate about data storytelling, process improvement, and analytics-driven decision-making.

🪪 License
This project is made available under the MIT License.

🗝️ Tags
#Excel #DataAnalysis #BusinessIntelligence #PowerBI #VLOOKUP #SUMIFS #IFFunction #DataCleaning


