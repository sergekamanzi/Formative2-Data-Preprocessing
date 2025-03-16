# Formative2
# Data Preprocessing 

## Project Overview
This project focuses on preprocessing two real-world datasets to enhance data quality and prepare it for machine learning. The process involved data augmentation, merging datasets using transitive properties, feature engineering and ensuring data consistency.

## Group Members & Contributions
- **Geofrey Tumwesigye**: Part 1 - Data Augmentation on CSV Files
- **Serge Kamanzi**: Part 2 - Merging Datasets with Transitive Properties
- **Willy Kalisa**: Part 3 - Data Consistency and Quality Checks

## Tasks Overview
### **Part 1: Data Augmentation on CSV files (Geofrey Tumwesigye)**
- **Dataset Loaded**: `customer_transactions.csv`
- **Handling Missing Values**:
  - Applied mean, median and mode imputation.
  - Used predictive modeling to fill missing data.
- **Data Augmentation Strategies**:
  - Introduced synthetic data using random noise to numerical transaction values.
  - Applied **SMOTE** for data balancing.
  - Performed **log transformation** on skewed data.
  - Expanded the dataset by generating synthetic transactions.
- **Final Output**: `customer_transactions_augmented.csv`

### **Part 2: Merging Datasets with Transitive Properties (Serge Kamanzi)**
- **Datasets Merged**:
  - `customer_transactions_augmented.csv`
  - `customer_social_profiles.csv` 
  - `id_mapping.csv` 
- **Steps taken**:
  - Mapped customer IDs using the intermediate mapping dataset.
  - Merged datasets while handling duplicate entries.
  - Created a **Customer Engagement Score** by combining transaction history and social media activity.
  - Engineered new features:
    - Moving averages of transactions.
    - Time-based aggregation of purchases.
    - **TF-IDF vectorization** for customer reviews.
- **Final Output**: `final_customer_data_5.csv`

### **Part 3: Data Consistency and Quality Checks (Willy Kalisa)**
- **Ensured Data Integrity**:
  - Removed duplicate entries.
  - Validated categorical values.
  - Ensured transactions match a valid social profile.
- **Statistical Summary**:
  - Generated summary statistics for numerical columns.
  - Visualized distribution of transaction amounts before and after augmentation.
- **Feature Selection**:
  - Computed a **correlation heatmap** to identify highly correlated features.
  - Applied **SelectKBest** to select the top 10 features for machine learning.
- **Final Output**: `final_dataset_ready_5.csv`

## Deliverables
- **Colab Notebooks**: Contain all preprocessing steps.
- **Final Processed Datasets**:
  - `customer_transactions_augmented.csv`
  - `final_customer_data_5.csv`
  - `final_dataset_ready_5.csv`
- **Report Summary (PDF)**
- **GitHub Repository** (https://github.com/sergekamanzi/Formative2-Data-Preprocessing)
- **Video Presentation** (link to the video)

## How to Use This Project
1. Clone the repository:
   ```sh
   git clone <https://github.com/sergekamanzi/Formative2-Data-Preprocessing>
   ```
2. Navigate to the project folder and run the notebooks in Google Colab.
3. Download and use the preprocessed datasets for training machine learning models.

## Challenges faced
- **Handling Missing Values**: Predictive modeling was required for filling gaps in certain features.
- **Complex Merging**: Transitive mapping added an extra layer of complexity in dataset integration.
- **Feature Engineering**: Required experimentation with different transformations to extract useful insights.



