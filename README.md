# Bank-Fraud-Analysis-Project
# Bank Fraud Detection Analysis

## Project Overview
This project implements multiple machine learning methodologies to detect fraudulent banking transactions. Using a real-world dataset with significant class imbalance (284,315 legitimate vs. 492 fraudulent transactions), this analysis demonstrates effective techniques for identifying anomalous financial activity.

## Dataset Information
- **Total transactions**: 284,807
- **Legitimate transactions**: 284,315 (99.83%)
- **Fraudulent transactions**: 492 (0.17%)
- **Features**: 31 columns per transaction

## Detection Methodologies
This project implements five distinct approaches to fraud detection:

1. **K-Means Clustering**
   - Identifies anomalies based on distance from centroids
   - Groups transactions into clusters and flags outliers

2. **Z-Score Analysis**
   - Flags extreme outliers in numeric features
   - Standardizes features and identifies transactions with unusual values

3. **DBSCAN Analysis**
   - Detects density-based anomalies as noise points
   - Effective at finding clusters of arbitrary shapes without requiring predefined cluster numbers

4. **Logistic Regression**
   - Classifies transactions as fraud or non-fraud using supervised learning
   - Balances precision and recall for minority class detection

5. **Isolation Forest**
   - Highlights anomalous transactions using tree-based partitioning
   - Particularly effective for imbalanced datasets

## Key Findings
- The dataset shows extreme class imbalance with only 0.17% fraudulent transactions
- Legitimate transactions have a mean amount of $88.29 with standard deviation of $250.11
- Transaction amounts range from $0.00 to $25,691.16
- The model performance metrics demonstrate effective fraud detection despite imbalance

## Technical Implementation
- Python-based analysis using Jupyter Notebooks
- Pandas for data manipulation and preprocessing
- Scikit-learn for implementing machine learning algorithms
- Matplotlib/Seaborn for data visualization

## Results
- Comparative performance metrics across all five methodologies
- Analysis of false positives and false negatives
- Recommendations for real-world implementation

## Installation and Usage
1. Clone this repository
```bash
git clone https://github.com/yourusername/bank-fraud-detection.git
cd bank-fraud-detection
```

2. Create and activate a virtual environment (recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required dependencies
```bash
pip install -r requirements.txt
```

4. Run the Jupyter notebook
```bash
jupyter notebook
```

5. Open `fraud2.ipynb` to view the analysis

## Project Structure
```
bank-fraud-detection/
├── data/                   # Dataset files (if public)
├── notebooks/              # Jupyter notebooks
│   └── fraud2.ipynb        # Main analysis notebook
├── models/                 # Saved model files
├── README.md               # Project documentation
└── requirements.txt        # Dependencies
```

## Future Work
- Implement neural network approaches (Autoencoders, GAN)
- Explore time-based features and sequence analysis
- Develop real-time fraud detection system
- Implement model explainability techniques
- Optimize for deployment in production environments

