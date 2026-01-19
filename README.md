# Common Complaints with Management Companies in Champaign/Urbana

## Analysis of Leasing Company Reviews Across Three University Towns

This project analyzes Google reviews for leasing companies and apartment complexes in three campustowns:
- **Brigham Young University** (Provo, UT)
- **Penn State University** (University Park, PA)  
- **University of Illinois at Urbana Champaign** (Champaign/Urbana, IL)

The analysis identifies common complaint patterns and evaluates how well different property management companies handle these issues.

## Dataset

The dataset contains:
- **16,850 reviews** across 142 properties
- **Pre-processed token analysis** (lemmatized words, excluding stop words)
- **Pre-computed sentiment analysis** (using DistilBERT)
- **Metadata** including owner responses, timestamps, and rating scores

Data is sourced from [Outscraper](https://outscraper.com/) and hosted on GitHub.

## Key Findings

### 1. Keywords Associated with Positive and Negative Sentiments

- **Strongly Negative Complaints (80–93% negative):** Water leaks, unreturned deposits, security issues, elevator problems, and pest control
- **Maintenance:** When handled well, 60% of reviews remain positive (vs. 52% at BYU)
- **UIUC Performance:** Slightly outperforms on elevator and water leak handling

### 2. Owner Response Time Correlation

- **Within 1 day:** 59% positive, 33% negative (best outcome)
- **Within 1 week:** 61% positive, 31% negative (~20% lift vs. no response)
- **Key Finding:** Quick replies improve sentiment by approximately 20 percentage points

### 3. Review Length vs. Rating Distribution

- **Negative reviews are much longer:** 1-star reviews average 693 chars vs. 5-star reviews at 245 chars
- **Length-Likes Correlation:** r = 0.40 (moderate positive)
- Longer reviews attract more engagement, making negative reviews more visible

### 4. UIUC Comparison & Startup Priorities

**Overall Performance Ranking:**
- UIUC: 3.74 avg (market leader)
- PSU: 3.61 avg (competitive)
- BYU: 3.15 avg (struggling)

**Most Critical Aspects to Address:**
1. **Responsive Maintenance & Repair Service** (Highest Impact)
2. **Fair & Transparent Security Deposit Handling**
3. **Water Leak Prevention & Emergency Response**
4. **Elevator Maintenance for Multi-Story Buildings**
5. **Security Infrastructure & Package Management**

## Requirements

```bash
pip install pandas numpy plotly
```

## Usage

Open `case-study-07-campustown-reviews-starter.ipynb` in Jupyter Notebook or JupyterLab to run the analysis.

The notebook:
- Loads data from remote GitHub repositories
- Performs data preprocessing and merging
- Creates keyword flags for complaint analysis
- Generates visualizations using Plotly
- Provides detailed insights for each research question

## Files

- `case-study-07-campustown-reviews-starter.ipynb` - Main analysis notebook
- `Common-Complaints-in-ChampaignUrbana-Management-Companies (1).pdf` - Supporting documentation

## License

This project is for educational and research purposes.
