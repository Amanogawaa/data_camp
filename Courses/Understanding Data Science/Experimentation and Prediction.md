- ## A/B Testing & Data Science Experiments

	- #### **What Are Experiments in Data Science?**
		- Experiments help **drive decisions** and **draw conclusions** based on data.
		- They involve:
		    - **A question** (e.g., "Which blog title gets more clicks?")
		    - **A hypothesis** (e.g., "Both titles will get the same number of clicks.")
		    - **Data collection** (e.g., split audience into two groups)
		    - **A statistical test** to analyze results
		    - **Interpretation** of findings
		    
	- #### **What is A/B Testing?**
		- A **controlled experiment** comparing two options (A vs. B) to determine which performs better.
		- Also called **Champion/Challenger testing**.
		- Used widely in **marketing, UI/UX, product optimization, and more**.
		
	- #### **Key A/B Testing Terminology**
		- ✅ **Sample size** – Number of data points collected in an experiment.  
		- ✅ **Statistical significance** – Ensures that observed differences are **not due to random chance**.  
		- ✅ **Sensitivity** – How small of a change in a metric the test can detect.

- ### **A/B Testing Process**
	- #### **1️⃣ Pick a Metric to Track**
		- Choose a **performance metric** to measure success.
		- Example: **Click-through rate (CTR)** – percentage of people who click a link after seeing the title.
	
	- #### **2️⃣ Calculate Sample Size**
		- The sample size should be large enough to ensure results **aren’t random**.
		- Depends on:
		    - **Baseline metric** (e.g., typical click-through rate for blog titles)
		    - **Sensitivity** – how small of a difference we care about detecting
		- **Larger sample sizes** allow detection of smaller changes.
	
	- #### **3️⃣ Run the Experiment**
		- Randomly assign users to **Variant A** or **Variant B**.
		- **Wait until the target sample size is reached**.
		- Stopping too soon or too late **leads to biased results**.
	
	- #### **4️⃣ Check for Statistical Significance**
		- A **statistical test** (e.g., t-test, chi-square test) determines if the difference is **real** or **due to chance**.
		- **Significant results** → Strong evidence that one version is better.
		- **Not significant?**
		    - The difference is too small to matter.
		    - Running the test longer **won’t help** because we've already decided what difference matters.

- ## Time Series Forecasting & Predictive Modeling
	- #### **What is Modeling in Data Science?**
		- **Models** represent real-world processes using **statistics and historical data**.
		- They **define relationships** between variables using **equations**.
		
	- #### **Predictive Modeling**
		- A type of modeling used for **making predictions**.
		- Example: Predicting **unemployment rates**, **tweet authenticity**, or **stock prices**.
		- Can be as simple as a **linear equation** or as complex as **deep learning models**.
		
	- ## Time Series Data
		- #### **1️⃣ What is Time Series Data?**
			- **A sequence of data points** collected over time.
			- Examples:
			    - **Stock prices** (daily)
			    - **Gas prices** (monthly)
			    - **CO₂ levels** (yearly)
			    - **Heart rate during surgery** (every second)
			    
		- #### **2️⃣ Plotting Time Series Data**
			- Time series data is **plotted on a line graph**, with:
			    - **X-axis** → Time (days, months, years, etc.)
			    - **Y-axis** → Value being measured
		
		- #### **3️⃣ Seasonality in Time Series**
			- **Seasonality** = **Repeating patterns** related to time (e.g., daily, monthly, yearly).
			- Examples:
			    - **Temperature in Boston** peaks in summer, drops in winter.
			    - **Ice cream sales** rise in summer.
			    - **Spending increases** at the end of the month (payday effect).
			    
		- ### **Time Series Forecasting**
		- #### **1️⃣ What is Time Series Forecasting?**
			- Using past **time series data** to **predict future trends**.
			- Examples:
			    - **Rainfall next month**
			    - **Stock market trends in a few hours**
			    - **Population growth over decades**
			    
		- #### **2️⃣ Case Study: Pea Prices in Rwanda**
			- **Data:** Pea prices in Rwandan Francs (2011–2016).
			- **Findings:**
			    - Prices are **lowest in December–January**.
			    - Prices **peak in August**, sometimes in April.
			    - Prices **generally increase over time**.
			
		- #### **3️⃣ Forecasting Pea Prices**
			- A **predictive model** forecasts prices with **seasonality & price trends**.
			- **Confidence Intervals** (blue shaded regions):
			    - **80% Confidence Interval** → The model is 80% sure the true price falls within this range.
			    - **95% Confidence Interval** → The model is 95% sure the true price falls within this range.
			- **Use Case:** Helps businesses and policymakers **prepare for price fluctuations**.