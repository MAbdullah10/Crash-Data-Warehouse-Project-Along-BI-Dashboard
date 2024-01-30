# Crash-Data-Warehouse-Project-Along-BI-Dashboard
**Road Safety Data Warehouse Project**

### Overview

This project aims to establish a comprehensive Crash Data Warehouse to analyze and visualize data related to road crashes in queensland. The entire process involves creating a Staging Database, performing data extraction, transformation, and loading (ETL) to populate the Data Warehouse, and finally, utilizing Power BI for creating an interactive and insightful dashboard.

### Project Phases

1. **Staging Database Setup:**
   - **Objective:** Establish a staging area to store raw data before transformation.
   - **Actions:**
     - Created a Staging Database with an appropriate schema to accommodate diverse road safety data.
     - Defined tables to match the structure of CSV files (crash locations, alcohol, etc.).

2. **Data Extraction and Transformation:**
   - **Objective:** Extract data from CSV files, transform it, and load it into the Staging Database.
   - **Actions:**
     - Utilized SQL Server tools as well as visual studio integration services to import data from CSV files into the Staging Database.
     - Conducted data type conversions to ensure uniformity and compatibility.
     - Performed necessary data cleansing and dropped unnecessary columns to streamline the dataset.

3. **Data Warehouse Schema Design:**
   - **Objective:** Define a structured schema for the Data Warehouse to organize data efficiently.
   - **Actions:**
     - Created a Warehouse Schema that includes dimension tables (e.g., crash locations, alcohol speed fatigue, vehicle involvement, road casualties, driver involvement, restraint helmet details) and a fact table named as fact road crash for comprehensive analytics.
     - Defined relationships between tables to establish a reliable data model.

4. **ETL Pipeline Implementation:**
   - **Objective:** Develop an ETL pipeline in visual studio to move data from the Staging Database to the Data Warehouse.
   - **Actions:**
     - Implemented SSIS packages in Visual Studio for data extraction, transformation, and loading.
     - Executed the ETL pipeline to populate dimension tables and the fact table.

5. **Derived Attributes in Fact Table:**
   - **Objective:** Enhance the fact table by introducing derived attributes for deeper analysis.
   - **Actions:**
     - Calculated and added derived attributes in the fact table using SQL queries.
     - Examples include crash severity indexes, casualty rates, and other meaningful metrics.

6. **Power BI Dashboard Creation:**
   - **Objective:** Leverage Power BI for interactive and visually appealing data dashboards.
   - **Actions:**
     - Connected Power BI to the Data Warehouse to establish a live connection.
     - Designed a dashboard incorporating key metrics, trends, and visualizations.
     - Implemented slicers, filters, and drill-down functionalities for user interactivity.

7. **Data Visualization and Insights:**
   - **Objective:** Extract actionable insights from the data through visualization.
   - **Actions:**
     - Utilized Power BI's visualization capabilities to create charts, graphs, and maps.
     - Analyzed trends, identified hotspots, and visualized correlations within the road safety data.

### Repository Structure

- **`/ETL`**: Contains SSIS packages for the ETL pipeline.
- **`/SQL`**: Includes SQL scripts for schema creation, data type conversions, and derived attribute calculations.
- **`/PowerBI`**: Holds Power BI files for the created dashboard.

### Getting Started

1. Clone the repository: `git clone https://github.com/yourusername/roadsafety-data-warehouse.git`
2. Follow instructions in the `/ETL` and `/SQL` directories for database setup and ETL execution.
3. Open Power BI files in `/PowerBI` for dashboard exploration.

### Conclusion

This project provides a systematic approach to building a Crash Data Warehouse, empowering users to derive meaningful insights from the analyzed data. The combination of SQL, ETL tools, Visual Studio and Power BI creates a robust framework for comprehensive data analysis and visualization.
