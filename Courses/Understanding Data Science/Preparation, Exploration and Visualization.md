## Data Prep
	- #### **What is Data Preparation?**
		- Data preparation is the process of cleaning and structuring raw data for analysis.
		- It happens after data collection and storage.
	
	- #### **Why is Data Cleaning Important?**
		- Real-world data is messy and needs cleaning to avoid incorrect results.
		- Skipping this step can lead to errors in analysis and machine learning models.
	
	- #### **Key Steps in Data Cleaning**
	
	- ✅ **Tidy Data**
		- Observations (rows) should represent individual entities (e.g., people).
		- Features (columns) should represent attributes of those entities.
		- Tools like Python and R help transform messy data into a structured format.
	
	- ✅ **Remove Duplicates**
		- Duplicate records should be removed to prevent redundancy.
		- If names are repeated, a **unique ID** should be assigned to each entity.
	
	- ✅ **Ensure Homogeneity**
		- Standardize measurements (e.g., feet to meters) and formats (e.g., country names).
		- Convert all data to a consistent unit system.
	
	- ✅ **Check Data Types**
		- Columns should have the correct data types (e.g., numbers for Age, not text).
		- Incorrect data types can cause errors in calculations and analysis.
	
	- ✅ **Handle Missing Values**
		- Missing values can be filled using:
		    - Exact values (if available).
		    - Aggregate values (mean, median, etc.).
	    - Dropping incomplete observations (only if necessary).
	    - Keeping them if the algorithm can handle missing data.
## Exploratory Data Analysis (EDA)
- #### **What is EDA?**
	- **Exploratory Data Analysis (EDA)** is a process promoted by **John Tukey**, a statistician.
	- It helps explore data, **formulate hypotheses**, and **understand key characteristics**, with a strong focus on **visualization**.

- #### **EDA in the Data Workflow**
	- EDA happens **after data preparation**, but they often mix.
	- EDA may **reveal more issues** that require additional cleaning.

- #### **The Importance of Visualization**
	- Looking at raw data provides **little insight**.
	- Descriptive statistics (mean, variance, correlation) **can be misleading**.
	- **Example: Anscombe’s Quartet**
	    - Four datasets have the same **mean, variance, correlation, and regression line**.
	    - But when visualized, they tell **completely different stories** (linear, non-linear, or skewed by outliers).

- #### **EDA on a Real Dataset: SpaceX Launches**
- ✅ **Know Your Data**
	- Understand what features you have (e.g., **flight number, payload, mission success**).
	- Check if **data types** are correct.

- ✅ **Preview the Data**
	- Scan tables to **spot missing values** (e.g., missing **payload mass** in first two rows).

- ✅ **Calculate Descriptive Statistics**
	- Compute summary stats like:
	    - **Count** of launches.
	    - **Average payload mass**.
	    - **Number of failed missions** (only 1 out of 55).
	    - **Launch counts per year**.

- ✅ **Visualize Data**
	- **Graphing launches per year** shows trends (e.g., no launches in 2011, steady growth, then a jump in 2017).
	- **Visualizing launch sites** shows shifts in location usage over time.
	- **Mission outcomes**: Only **1 failure** in 2015.

- ✅ **Find Outliers**
	- Outliers can distort results.
	- Example: Only **5 launches** had a payload **>7,000 kg**, while the average was **~3,800 kg**.

## Visualization
- #### **The Power of Visualization**
	- **"A picture is worth a thousand words."**
	- However, **not all visualizations are effective**—design matters!

- #### **Best Practices for Effective Graphs**
	- ✅ **Use Color Purposefully**
		- **One color is enough** for simple charts (e.g., launch count per year).
		- **Too many colors** can be confusing, especially if they don't represent anything meaningful.
	
	- ✅ **Consider Colorblind Accessibility**
		- Many people have **color vision deficiencies**.
		- Use **colorblind-friendly palettes** for better accessibility.
	
	- ✅ **Use Readable Fonts**
		- **Sans-serif fonts** are easier to read.
		- Avoid fancy fonts—focus should be on the data, not typography.
	
	- ✅ **Label Everything!**
		- Always include a **title** to describe the graph.
		- Label **X and Y axes**—without labels, the data loses meaning.
		- Use a **legend** when using multiple colors/patterns.
	
	- ✅ **Be Careful with Axes**
		- Axes **should generally start at zero** to avoid misleading representations.
		- In some cases (e.g., showing small variations), zooming in can be useful but should be done transparently.
	
	- ✅ **Avoid Misleading Graphs**
		- Poorly designed graphs confuse the audience.
		- Use proper scaling, avoid unnecessary complexity, and ensure clarity.
	
	- #### **What’s Better Than a Picture? A Dashboard!**
		- **Dashboards** group multiple visualizations together to provide more **context and insights**.
		- Example: A car dashboard shows speed, fuel level, and engine status **together**, making driving safer.
		- In business, a **sales dashboard** can show sales trends, customer count, and revenue comparisons **in one place**.
	
	- #### **Business Intelligence (BI) Tools**
		- BI tools allow **data cleaning, exploration, visualization, and dashboard building**—often with no coding required.
		- Popular BI tools:
		    - **Tableau**
		    - **Looker**
		    - **Power BI**
		- **Coding alternatives**: Python (Matplotlib, Seaborn, Plotly), R (ggplot2), JavaScript (D3.js).
	
	- #### **The Next Level: Interactive Dashboards**
		- Interactivity **engages users** and allows **customization**.
		- Examples:
		    - **Hovering over elements** to show details.
		    - **Applying filters** (e.g., selecting sales by type or quarter).
		- **BI tools make interactivity easy**, but it can also be done with code (e.g., using Plotly Dash or Streamlit in Python).