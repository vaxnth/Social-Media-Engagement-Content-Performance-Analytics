# Social Media Engagement & Content Performance Analytics

## Project Overview

This project focuses on analyzing social media engagement and content performance across multiple platforms using Python.

The objective is to clean and transform raw social media data, explore engagement patterns, analyze posting trends over time, and apply statistical hypothesis testing to support data-driven business decisions.

## Objectives

- Clean and transform unstructured social media data using ETL techniques.
- Perform Exploratory Data Analysis (EDA) to understand content performance.
- Analyze relationships between reach, impressions, likes, comments, and shares.
- Identify posting patterns using Time Series Analysis.
- Apply statistical tests to evaluate differences and relationships in social media performance.
- Generate actionable business insights and recommendations.

## Dataset Description

The project uses a synthetic social media engagement dataset containing approximately 20,000 records.

**Dataset columns:**

| Column | Description |
|---|---|
| post_id | Unique post identifier |
| account_id | Social media account identifier |
| post_timestamp | Date and time of publication |
| platform | Social media platform |
| content_type | Type of published content |
| reach | Number of unique users reached |
| impressions | Total number of content views |
| likes | Number of likes |
| comments | Number of comments |
| shares | Number of shares |

The raw dataset intentionally contains missing values, duplicate records, inconsistent category labels, invalid values, and formatting issues for data-cleaning practice.

**Note:** This is a synthetic practice dataset, not real platform data.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Statsmodels
- Jupyter Notebook

## Project Workflow

### 1. ETL – Extract, Transform, Load

- Loaded the raw dataset into Python.
- Identified and handled duplicate records.
- Standardized platform and content-type values.
- Converted numerical columns into appropriate data types.
- Handled missing and invalid values.
- Converted timestamps into datetime format.
- Created additional engagement-related features.
- Prepared the cleaned dataset for analysis.

### 2. Exploratory Data Analysis (EDA)

**Univariate Analysis**
- Content type distribution.
- Reach distribution using Histogram and KDE.
- Reach outlier detection using IQR and Box Plot.

**Bivariate Analysis**
- Reach vs Likes using Scatter Plot.
- Correlation Heatmap.
- Content Type vs Total Engagement using Box Plot.

**Multivariate Analysis**
- Platform vs Content Type vs Average Reach.

### 3. Time Series Analysis

- Daily social media posting trend.
- 7-Day Moving Average.
- 30-Day Moving Average.
- Short-term and long-term posting pattern analysis.

### 4. Hypothesis Testing

The project applies statistical methods to evaluate social media performance.

| Statistical Test | Purpose |
|---|---|
| Independent T-Test | Compare average likes between video and image posts |
| ANOVA | Compare average likes across multiple content types |
| Tukey HSD | Identify significant differences between content-type pairs |
| Paired T-Test | Compare matched before-and-after campaign observations |
| Chi-Square Test | Examine the association between platform and content type |

A significance level of 0.05 is used for hypothesis testing.

## Key Business Insights

- Understand the distribution of social media content.
- Identify reach patterns and potential high-performing posts.
- Examine relationships between reach and audience engagement.
- Compare content performance across platforms.
- Identify short-term and long-term posting trends.
- Use statistical testing to evaluate differences and associations.

## Business Recommendations

- Develop content strategies based on engagement performance.
- Analyze high-reach posts to identify successful content patterns.
- Improve posting consistency using moving average trends.
- Use platform-specific content strategies.
- Monitor multiple engagement metrics instead of relying on reach alone.
- Make data-driven decisions using statistical findings.

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
cd <your-repository-name>
```

### Step 2: Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels jupyter
```

### Step 3: Start Jupyter Notebook

```bash
jupyter notebook
```

### Step 4: Run the Analysis

Open the project notebook and execute the cells in workflow order:

1. ETL
2. EDA
3. Time Series Analysis
4. Hypothesis Testing

## Project Structure

```text
Social-Media-Analytics/
│
├── dataset/
│   ├── social_media_engagement_uncleaned_20000.csv
│   └── social_media_engagement_cleaned.csv
│
├── notebooks/
│   └── social_media_analysis.ipynb
│
├── insights/
│   └── business_insights.md
│
├── README.md
└── requirements.txt
```

*Adjust the structure to match the files actually present in your repository.*

## Conclusion

This project demonstrates an end-to-end data analytics workflow using Python, covering ETL, Exploratory Data Analysis, Time Series Analysis, and Hypothesis Testing.

The analysis helps understand social media content performance, audience engagement patterns, and posting trends while supporting data-driven business recommendations.

## Author

**Vasanthakumar IS**

B.E. Computer Science and Engineering – Cybersecurity
