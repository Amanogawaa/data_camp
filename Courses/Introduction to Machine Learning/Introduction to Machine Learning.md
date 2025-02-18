
### ***What is Machine Learning?***

- **Machine Learning (ML)** is a **subset of Artificial Intelligence (AI)** used to make predictions and inferences from data.
- It powers **self-driving cars, medical diagnostics, intelligent assistants, and even art**.

---
### ***Understanding AI vs. Machine Learning***

#### **Artificial Intelligence (AI)**

- AI is a **broad field** that includes **robotics, expert systems, and machine learning**.
- **Machine Learning is the most widely used subset** of AI today.

#### **Machine Learning (ML)**

- ML **allows computers to learn patterns from data** without being explicitly programmed.
- Used for:
    - **Spam detection**
    - **Weather prediction**
    - **Stock price forecasting**

---
### ***Machine Learning Tasks***

#### **Prediction vs. Inference**

- **Prediction** → Forecasting future outcomes (e.g., Will it rain tomorrow?).
- **Inference** → Understanding patterns & causes (e.g., Why does it rain?).
- **Example:** Weather models use **humidity, temperature, and time of year** to both **predict rain and infer weather patterns**.

#### **How Does Machine Learning Work?**

- Uses **statistics & computer science** to **learn from past data** and apply knowledge to new data.
- Example: A spam filter learns from archived emails and detects spam in new emails.
- **High-quality data** is critical for effective learning.

---
### ***Machine Learning in Data Science***

- **Data Science** = Extracting insights from data.
- ML is an **important tool** in Data Science, especially for **predicting future trends**.

---
### ***Machine Learning Models***

- **ML models** are **statistical representations** of real-world processes.
- Example Models:
    - **Traffic Prediction:** Input → Future date → Output → Estimated traffic.
    - **Fake News Detection:** Input → Tweet → Output → Probability of being fake

---
### ***Types of Machine Learning***

#### **1️⃣ Reinforcement Learning (RL)**

- Used for **decision-making in sequential actions** (e.g., robots, chess-playing AIs).
- Based on **game theory** and complex mathematics.
- **Not as commonly used** as the other types.

#### **2️⃣ Supervised Learning (SL)**

- **Uses labeled data** (data where the correct answer is already known).
- **Example:** Predicting **heart disease** based on features like **age, cholesterol, and smoking habits**.
- The model learns by associating **features (inputs)** with **labels (outputs)**.

#### **3️⃣ Unsupervised Learning (UL)**

- **Uses unlabeled data** (data without predefined answers).
- **Example:** Clustering patients into different groups based on similar health features.
- The model **finds hidden patterns** in the data on its own.

---
### ***Training a Machine Learning Model***

#### **What is Training Data?**

- Machine learning **learns from training data** to find patterns.
- **Training a model** involves feeding it existing data so it can learn.
- Training time varies: **from nanoseconds to weeks**, depending on dataset size.

#### **Supervised Learning Example: Heart Disease Prediction**

- **Target variable:** `"heart disease"` (True/False)
- **Observations (rows):** Patients' data.
- **Features (columns):** Age, cholesterol level, smoking habits, etc.
- Model **learns from past data** and predicts outcomes for **new patients**.

#### **Unsupervised Learning Example: Clustering Patients**

- We only have **features**, no labels.
- The model **groups patients into categories** based on shared characteristics.
- **Use-case:** Discovering which types of patients respond best to different treatments.

---
### ***Why Use Unsupervised Learning?***

- **Sometimes, labeling data is too expensive or impossible.**
- Example: Labeling **millions of road images** for self-driving cars is impractical.
- Instead, models **discover patterns themselves**, making them highly scalable.

---
### ***Key Differences: Supervised vs. Unsupervised Learning***

|**Aspect**|**Supervised Learning**|**Unsupervised Learning**|
|---|---|---|
|**Data Type**|Labeled data (has known outputs)|Unlabeled data (no predefined answers)|
|**Task**|Predicting outcomes|Finding hidden patterns|
|**Example**|Diagnosing heart disease|Grouping patients by health similarities|
|**Common Uses**|Spam detection, medical diagnoses, stock price forecasting|Customer segmentation, anomaly detection, recommendation systems|

---
### ***Machine Learning Workflow: Steps to Building a Model***
#### ***Scenario: Predicting Apartment Prices***

We have a dataset containing details about apartment sales in New York City. Each record includes:

- **Square feet**
- **Neighborhood**
- **Year built**
- **Sale price (our target variable)**

Since we have labeled data (sale prices), this is a **supervised learning** problem.

---
#### *The 4-Step Machine Learning Workflow*
#### **Step 1: Extract Features**

- Datasets don’t come in a perfect format.
- **Feature selection** is crucial:
    - **Good features:** Square feet, neighborhood, distance to subway.
    - **Irrelevant features:** Seller’s name, apartment color, etc.
- More relevant features → Better predictions.

---

#### **Step 2: Split Dataset**

- The dataset is split into two parts:
    - **Training dataset (80%)** → Used to train the model.
    - **Test dataset (20%)** → Used to evaluate the model.
- This ensures the model is tested on **unseen data** to check real-world performance.

---

#### **Step 3: Train the Model**

- The training dataset is fed into a **machine learning algorithm**.
- Examples of models:
    - **Linear Regression** (for predicting prices)
    - **Neural Networks** (for complex patterns)
    - **Logistic Regression** (for classification tasks)
- The model **learns patterns** from training data.

---

#### **Step 4: Evaluate the Model**

- We test the model on **unseen data (test dataset)** to measure accuracy.
- **Evaluation metrics:**
    - **Mean Absolute Error (MAE):** Average prediction error.
    - **Mean Squared Error (MSE):** Penalizes large errors more.
    - **Accuracy within 10% of actual price.**
- If performance is poor, we **tune the model**:
    - Adjust parameters (hyperparameters).
    - Add/remove features.
    - Gather more data.

---
#### ***If the Model Fails?***

- If **80% accuracy is acceptable**, we’re done! ✅
- If not, we go back to **Step 3 (Training)** and improve it.