# Greater Manchester Domestic Energy Performance Analyser (2013 - 2023)

## Overview
This project analyzes the Energy Performance Certificates (EPC) dataset for Greater Manchester between 2013 and 2023. The goal is to gain insights into energy efficiency, CO2 emissions, and potential cost savings for properties in the region. The data is processed using Microsoft Azure SQL Database and visualized in Power BI.

## Features
- **Data Import and Processing**: The dataset is imported into an Azure SQL Database and managed using SQL Server Management Studio (SSMS).
- **Database Operations**: Views, Common Table Expressions (CTEs), and stored procedures are used to analyze EPC data.
- **Power BI Dashboard**: Interactive dashboards provide insights into energy performance, cost savings, and environmental impact.
- **Recommendations**: Energy-saving recommendations are provided based on data analysis.

## Dataset
The dataset consists of three files:
1. **Certificates** - Contains EPC calculation data.
2. **Columns** - Provides descriptions of column headers.
3. **Recommendations** - Suggests energy efficiency improvements.

Dataset source: [EPC Open Data](https://epc.opendatacommunities.org/login#local-authorit)

## Database Utilization
1. **Azure SQL Database Creation**: The database was created using Microsoft Azure following `dp900-01-sql-lab.md` guidelines.
2. **Data Import Process**:
   - Imported the dataset using SSMS Import Data Wizard.
   - Adjusted column widths for better data storage.
   - Verified data integrity by identifying missing values and anomalies.
3. **Views and Stored Procedures**:
   - Filtered data for the years 2013-2023.
   - Created stored procedures to summarize energy ratings by property type and calculate energy savings.

## Power BI Visualization
1. **Home Page**: Overview of energy performance analysis.
2. **Energy Performance Overview**:
   - **KPIs**: CO2 emissions, energy efficiency, total energy consumption.
   - **Charts**: Bar charts, gauge charts, line charts, and maps to display geographical energy trends.
   - **Slicers**: Filters for property type, year, and energy rating.
3. **Energy Cost Analysis**:
   - **KPIs**: Current and potential energy costs.
   - **Stacked Bar Charts**: Comparison of current vs. potential energy costs across property types.
   - **Matrix**: Breakdown of heating, lighting, and hot water costs by constituency.
4. **Energy Performance & Potential Upgrades**:
   - **KPIs**: Potential CO2 reduction and energy efficiency improvements.
   - **Tree Maps**: CO2 emissions by property type.
   - **Tables**: Suggested upgrades for properties.
5. **Energy Efficiency & Environmental Impact**:
   - **KPIs**: Potential energy efficiency and environmental impact.
   - **Line Charts**: Trends in CO2 emissions from 2013-2023.
   - **Bar Charts**: Environmental impact based on EPC ratings.
   - **Pie Charts**: Contribution of different property types to environmental degradation.

## Recommendations
1. Install loft insulation and fix draughts to improve EPC ratings quickly.
2. Use renewable energy solutions like solar panels and air-source heat pumps.
3. Upgrade windows to energy-efficient alternatives.
4. Switch to energy-efficient boilers (e.g., system or combi boilers).
5. Install cavity wall insulation to reduce heat loss.

## References
- [EPC Rating Guide](https://www.greenhub.tandem.co.uk/blog/epc-rating)
- [UK Government EPC Guide](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/671018/A_guide_to_energy_performance_certificates_for_the_marketing__sale_and_let_of_dwellings.pdf)
- [Green Home Plan](https://greenhomeplan.tandem.co.uk/tools)

## How to Use
1. Clone the repository:
   ```sh
   git clone <repository-url>
   ```
2. Import the SQL dataset into an Azure SQL Database.
3. Connect Power BI to the database and load the stored procedures and views.
4. Explore insights using the interactive Power BI dashboard.




