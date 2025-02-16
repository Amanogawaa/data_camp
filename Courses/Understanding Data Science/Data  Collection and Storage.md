- **Introduction to Data Sources**
    - Data collection and storage are the first steps in the **data science workflow**.
    
- **Types of Data Sources**
    - **Company Data:** Internal data collected by businesses.
    - **Open Data:** Freely available data from public sources.
    
- **Company Data Sources**
    - **Web Data:** Tracks user actions (e.g., page visits, clicks, timestamps).
    - **Survey Data:** Collected through interviews, online questionnaires, and focus groups.
    - **Net Promoter Score (NPS):** A common survey metric for customer satisfaction.
    
- **Open Data Sources**
    - **Public APIs:** Provide access to external data (e.g., Twitter, Wikipedia, Google Maps).
    - **Public Records:** Data from organizations like the **World Bank, UN, WTO**, and **government agencies**.
    
- **Example Use Case: Twitter API**
    - Tracking a hashtag (e.g., **#DataFramed**) for sentiment analysis or correlation with downloads.
    
- **Public Data Portals**
    - **US:** [data.gov](https://data.gov)
    - **EU:** [data.europa.eu](https://data.europa.eu)

## Data Types in Data Science
- **Why Data Types Matter**
    - Helps in **storing**, **visualizing**, and **analyzing** data correctly.
    - Some analyses and visualizations work only with specific data types.
    
- **Two General Data Types**
    - **Quantitative Data:** Can be measured numerically (e.g., height, price, count).
    - **Qualitative Data:** Descriptive and conceptual (e.g., color, origin, smell).
    
- **Examples of Data Types**
    - **Quantitative:** "The fridge is 60 inches tall and costs $1,000."
    - **Qualitative:** "The fridge is red and smells like fish."
    
- **Other Important Data Types**
    - **Image Data:** Made of pixels storing color and intensity.
    - **Text Data:** Emails, reviews, social media posts, etc.
    - **Geospatial Data:** Contains location-based information (e.g., Google Maps).
    - **Network Data:** Shows relationships between entities (e.g., social networks).
    
- **Next Step: Data Storage**
    - Different data types require different storage methods.

## Data Storage and Retrieval
- **Why Data Storage Matters**
    - Efficient storage is crucial for managing and retrieving data in data science projects.
- **Key Considerations for Storing Data**
    - **Where to store:** On-premises (clusters/servers) or cloud storage (AWS, Azure, Google Cloud).
    - **What type of data:** Structured (tables) or unstructured (text, images, videos).
    - **How to retrieve:** Querying methods like SQL for relational data and NoSQL for document-based data.
    
- **Storage Location Options**
    - **Parallel storage solutions:** Large datasets are stored across multiple computers in clusters.
    - **Cloud storage:** Third-party providers handle storage, analytics, and ML processing.
    
- **Types of Data Storage**
    - **Document Databases (NoSQL):** Store unstructured data (emails, social media, videos).
    - **Relational Databases (SQL):** Store structured/tabular data (spreadsheets, customer info).
    
- **Data Retrieval & Querying**
    - **SQL (Structured Query Language):** Used for relational databases.
    - **NoSQL (Not Only SQL):** Used for document-based and unstructured databases.
    
- **Analogy: A Library System**
    - **Choosing a location:** On-premises vs. cloud storage.
    - **Selecting shelves:** Document vs. relational databases.
    - **Finding books:** Querying data using SQL or NoSQL.

## Data Pipelines
- **What are Data Pipelines?**
	- Data pipelines help scale data collection and storage efficiently.
	- They automate data movement from sources (APIs, IoT devices) to storage.
	
- **Why Are Data Pipelines Needed?**
	- Data engineers collect and store data for analysts and data scientists.
	- Handling multiple data sources and real-time streaming data can be complex.
	
 - **Components of a Data Pipeline**
	- **Ingestion:** Collects data from APIs, IoT devices, databases, etc.
	- **Transformation:** Cleans, structures, and organizes data for easy access.
	- **Loading:** Stores processed data for analysis and visualization.
	
- **Example: Smart Home Case Study**
	- Data is gathered from APIs (weather updates, tweets) and IoT devices.
	- Extracted raw data must be structured before storage.
	- Transformation includes filtering, formatting, and schema adjustments.
	
- **ETL Framework (Extract, Transform, Load)**
	- **Extract:** Collect data from various sources.
	- **Transform:** Clean and structure the data (e.g., remove unnecessary details).
	- **Load:** Store it in a database for further use.
	
- **Automating Data Pipelines**
	- Automation reduces manual effort (e.g., scheduling hourly/daily tasks).
	- Alerts can notify issues like storage limits or API failures.
	- **Airflow** is a popular tool for managing automated data pipelines.