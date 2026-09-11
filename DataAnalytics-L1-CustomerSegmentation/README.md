# OIBSIP Task 2 - Customer Segmentation Analysis

## Objective
Segment an e-commerce customer base into distinct groups using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering, then recommend targeted marketing actions.

## Dataset
Kaggle Online Retail Dataset: https://www.kaggle.com/datasets/ersany/online-retail-dataset

The notebook downloads the public Kaggle dataset automatically with `kagglehub`, so the raw Excel file does not need to be manually uploaded.

## Tech Stack
- Python
- pandas
- scikit-learn
- matplotlib
- seaborn
- Jupyter Notebook / Google Colab
- KMeans
- StandardScaler

## Project Workflow
1. Download and load Kaggle Online Retail data.
2. Inspect structure and missing values.
3. Clean cancelled/invalid transactions and missing CustomerID records.
4. Calculate purchase value and customer-level RFM features.
5. Standardize Recency, Frequency and Monetary values.
6. Use the Elbow Method to identify K.
7. Run K-Means clustering.
8. Profile clusters using mean RFM values.
9. Visualize clusters with scatter plots and a customer-count bar chart.
10. Recommend marketing actions for each segment.

## Files
- `CustomerSegmentation.ipynb` - main notebook
- `CustomerSegmentation_Colab.py` - Colab-ready script that downloads the Kaggle data
- `CustomerSegmentation.py` - local version
- `requirements.txt` - required packages
- `data/` - dataset source notes
- `screenshots/` - place final charts/screenshots here if required
- `output/` - generated CSVs after running the notebook

## How to run in Google Colab
1. Upload `CustomerSegmentation_Colab.py` or copy its cells into a new Colab notebook.
2. Run all cells from top to bottom.
3. The script downloads the Kaggle dataset automatically.
4. The final RFM table, cluster summary, customer segments and insights are saved in `output/`.
5. Download `OIBSIP_Customer_Segmentation_Output.zip` for submission if required.

## Expected Submission Evidence
Include screenshots of:
- Dataset inspection
- Missing-value check
- RFM summary
- Elbow Method chart
- Frequency vs Monetary scatter plot
- Recency vs Monetary scatter plot
- Customers per cluster bar chart
- Cluster profile table
- Marketing recommendations

## Note
The raw Online Retail file is large. For GitHub, it is better to keep the Kaggle source link rather than commit the raw dataset directly.
