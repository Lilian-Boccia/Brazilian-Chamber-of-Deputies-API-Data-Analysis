# Brazilian Chamber of Deputies API Data Analysis
This project leverages the Brazilian Chamber of Deputies API to collect, process, and analyze legislative data. The goal is to transform public information into accessible insights, promoting greater transparency and engagement with legislative processes.

**Features and Capabilities**
- Direct API Connection: Automated data collection from the legislative API in real time.
- Data Processing: Cleaning and organizing retrieved data to ensure consistency and quality.
- Visualizations: Analysis of legislative trends and patterns presented through clear visuals.
- Modular Code: Organized structure to facilitate future contributions and maintenance.

**Technologies Used**
- Python for API integration, data cleaning, and generating insights.
- Key Libraries: Requests, Pandas, Matplotlib/Seaborn for analysis and visualizations.

**Data Pipeline Architecture**

The project utilizes a robust data pipeline to process and analyze parliamentary expenses efficiently. Below is an overview of the architecture:

Steps in the Pipeline:
1. Data Ingestion: Batch data is sourced from the Brazilian Chamber of Deputies' API.
2. Raw Data Storage (Bronze Layer/Data Lake): Data is stored in Hive in Delta format, preserving the raw state for traceability and reprocessing.
3. Data Transformation and Cleaning (Silver Layer): Databricks processes raw data by applying normalizations, corrections, and aggregations. Transformed data is stored in Snowflake as transactional and normalized tables.
4. Structured Data Storage (Gold Layer): Final data is stored in Snowflake as cubes and metrics, optimized for analysis and tailored to departmental needs such as Sales, Marketing, and Finance.
5. Self-Service Consumption Layer (BI): Looker Studio is integrated to allow end users to explore and analyze data stored in Snowflake independently.

![Data Pipeline](https://github.com/Lilian-Boccia/Brazilian-Chamber-of-Deputies-API-Data-Analysis/blob/main/Data%20Pipeline%20-%20Brazilian%20Chamber%20of%20Deputies'%20API.drawio.png)

**How to Use**
1. Download the Project:
- Clone the repository using:
git clone https://github.com/Lilian-Boccia/Brazilian-Chamber-of-Deputies-API-Data-Analysis.git  

2. Set Up Your Environment:
- Ensure you have Python installed on your system. Install required libraries directly using:
pip install requests pandas matplotlib seaborn  

3. Run the Notebook:
Open the _Camara_dos_Deputados.ipynb_ file in a Jupyter Notebook or Google Colab.
Execute the cells step by step to start collecting and analyzing data from the API.

**Contribute**
Contributions are welcome! Please open a pull request or submit suggestions to improve the project.

**Contact**
For questions or suggestions, feel free to reach out:
📧 lilian.boccia@gmail.com
🌐 LinkedIn: https://www.linkedin.com/in/lilianboccia/
