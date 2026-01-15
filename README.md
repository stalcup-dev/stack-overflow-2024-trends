# Developer Survey Analysis - Data Analyst Capstone Project

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## 📊 Project Overview

This repository contains a comprehensive data analysis of developer survey data, providing actionable insights into skill trends, compensation patterns, technology adoption, and workforce demographics. The analysis was performed as part of a professional data analyst capstone project.

### 🎯 Key Objectives

- **Data Exploration & Cleaning**: Standardize survey responses and prepare data for analysis
- **Skill Gap Analysis**: Identify emerging technologies and learning priorities
- **Compensation Insights**: Analyze salary distributions across experience levels and roles
- **Technology Trends**: Track adoption patterns for languages, databases, platforms, and frameworks
- **Actionable Recommendations**: Deliver evidence-based guidance for learners and hiring managers

## 📁 Repository Contents

| File | Description |
|------|-------------|
| **survey_data_exploration_cleaning_insights.ipynb** | Complete analytical notebook with data cleaning, exploratory analysis, visualizations, and executive insights |
| **DataAnalystPresentation.pdf** | Professional presentation deck summarizing key findings, recommendations, and visual storytelling |

## 🔍 Analysis Highlights

### Data Processing
- **Dataset**: Survey responses from developers worldwide
- **Cleaning Pipeline**: Standardized column names, handled multi-select fields, converted categorical age ranges to midpoints, normalized numeric fields
- **Quality Control**: Addressed missing values, trimmed outliers, and documented data limitations

### Key Insights Discovered

1. **Skill Demand Gaps**: Significant gaps between current usage and desired skills reveal emerging technology priorities
2. **Compensation Patterns**: Right-skewed distributions with wide variance across roles, regions, and experience levels
3. **Technology Stack**: Concentrated adoption in core technologies with long-tail opportunities in niche areas
4. **Remote Work**: Location-specific patterns indicate varying norms and policy environments
5. **AI Tool Adoption**: Strong interest but lower current usage suggests implementation barriers

### Visualizations Included

The notebook features 15+ comprehensive visualizations across multiple analytical dimensions. Each visualization includes contextual notes and actionable suggestions for interpretation.

**🎨 To view all charts and graphs**: [Open the Jupyter Notebook on GitHub](https://github.com/stalcup-dev/stack-overflow-2024-trends/blob/main/survey_data_exploration_cleaning_insights.ipynb) - GitHub automatically renders all saved visualization outputs.

## � Detailed Visualizations & Insights
> **📌 Note**: All visualizations below are rendered with full images in the Jupyter Notebook. [**View the notebook on GitHub**](https://github.com/stalcup-dev/stack-overflow-2024-trends/blob/main/survey_data_exploration_cleaning_insights.ipynb) to see the complete analysis with all charts and graphs.
### 1. **Top 10 Skills and Tools** (4-panel dashboard)
Displays the most commonly used technologies across four categories:
- **Programming Languages** (JavaScript, Python, SQL, etc.)
- **Databases** (PostgreSQL, MySQL, MongoDB, etc.)
- **Platforms** (AWS, Azure, Docker, etc.)
- **Web Frameworks** (React, Node.js, Express, etc.)

**Key Insights:**
- Counts represent multi-select mentions; one respondent can contribute multiple data points
- High counts reflect survey composition rather than absolute market share
- Long-tail tools signal niche opportunities for specialized roles

**Actionable Recommendations:**
- Compare "Have Worked With" vs "Want To Work With" to identify demand gaps
- Segment by country, experience level, or role to reveal meaningful trends
- Use as default dashboard filters for deeper analysis

---

### 2. **Age Distribution**
Histogram showing the age demographics of survey respondents (using midpoint values from age ranges).

**Key Insights:**
- Distribution is approximate due to age range conversion
- Shape reflects survey reach patterns more than overall developer population
- Non-range responses are excluded, potentially reducing sample size

**Actionable Recommendations:**
- Cross-reference with YearsCodePro to validate age-experience alignment
- Use broader age cohorts (e.g., Early Career, Mid-Career, Senior) for stable comparisons
- Consider cohort effects when interpreting technology adoption patterns

---

### 3. **Top 15 Countries by Response Count**
Bar chart showing geographic distribution of survey participants.

**Key Insights:**
- Response concentration varies significantly by country
- Counts reflect survey reach, not proportional tech workforce representation
- Geographic patterns influence other demographic findings

**Actionable Recommendations:**
- Normalize by population or tech workforce size when comparing countries
- Set minimum sample size thresholds for country-level analysis
- Consider regional economic factors when interpreting compensation data

---

### 4. **Job Satisfaction Distribution**
Bar chart displaying self-reported job satisfaction levels across respondents.

**Key Insights:**
- Satisfaction levels depend on multiple factors: role, compensation, remote status, regional context
- Self-reported data may be influenced by survey timing and current employment status

**Actionable Recommendations:**
- Compare job satisfaction by remote work arrangement or compensation band
- Cross-reference with other workplace factors (tenure, company size, benefits)
- Use as a baseline metric for workforce sentiment analysis

---

### 5. **Compensation Distribution** (Trimmed at 99th Percentile)
Histogram and box plot showing annual compensation in USD.

**Key Insights:**
- **Right-skewed distribution**: Medians are more representative than means
- Trimming at 99th percentile reveals typical salary ranges
- Wide variance even within similar experience bands

**Actionable Recommendations:**
- Always use medians for central tendency in compensation analysis
- Apply log scale transformations for better cross-group comparability
- Segment by role, region, and remote status to control for confounding factors

---

### 6. **Compensation by Remote Work Status**
Box plots comparing salaries across remote work categories (Fully Remote, Hybrid, In-Office).

**Key Insights:**
- Remote work categories are self-reported and may vary by regional definitions
- Compensation differences reflect both policy and geographic pay scales

**Actionable Recommendations:**
- Control for country and cost-of-living when comparing remote vs in-office pay
- Track changes over time as remote work policies evolve
- Consider role-specific remote work feasibility in analysis

---

### 7. **Experience vs Compensation Scatter Plot**
Shows relationship between years of professional coding experience and annual compensation.

**Key Insights:**
- Positive correlation but with substantial noise and wide variance
- Experience alone explains limited compensation variation
- Role, geography, and company size are major confounding factors

**Actionable Recommendations:**
- Add trend lines or median bands by experience buckets for clearer patterns
- Segment by role and location to reduce variance
- Treat as directional signal, not deterministic relationship

---

### 8. **Numeric Correlations Heatmap**
Correlation matrix showing relationships between years of experience, age, and compensation variables.

**Key Insights:**
- Highlights linear relationships between numeric variables
- Sensitive to outliers; correlations are descriptive, not causal
- Age and experience show expected positive correlations

**Actionable Recommendations:**
- Use as preliminary screening for multivariate models
- Investigate high correlations for potential multicollinearity issues
- Validate patterns with regression analysis for causal claims

---

### 9. **Remote Work Mix by Top Countries** (Stacked Bar Chart)
Shows the percentage breakdown of remote work arrangements within each top-responding country.

**Key Insights:**
- Each bar totals 100%, showing within-country distribution
- Significant variation across countries reflects cultural and policy differences
- Only top countries by response count included to ensure stability

**Actionable Recommendations:**
- Set minimum sample size thresholds to avoid unstable percentages
- Compare remote work mix with compensation or job satisfaction
- Consider regulatory environments and commute patterns by country

---

### 10. **Compensation by Education Level**
Box plots showing salary distributions across different educational attainment levels.

**Key Insights:**
- Education categories are self-reported and uneven in sample size
- Compensation is trimmed to reduce outlier influence
- Education effect varies by role and experience level

**Actionable Recommendations:**
- Cross-reference with YearsCodePro to add experience context
- Group similar degree types for clearer readability
- Account for geographic differences in educational requirements

---

### 11. **AI Tool Adoption: Current vs Interested** (Dual Bar Chart)
Compares current AI tool usage with expressed interest in learning/using AI tools.

**Key Insights:**
- Significant gap between current usage and stated interest
- Multi-select mentions allow tools to appear in both categories
- Gap reveals training needs and adoption friction points

**Actionable Recommendations:**
- Calculate interest gap (interested − current) to identify growth opportunities
- Prioritize tools with high interest but low current usage for training programs
- Track adoption velocity over time to validate enablement efforts

---

### 12. **Median Compensation by Developer Type** (Top 10)
Bar chart showing median salaries across different developer specializations.

**Key Insights:**
- Developer types are multi-select; respondents may appear in multiple categories
- Median values reduce skew but still reflect regional mix effects
- Specialization significantly impacts earning potential

**Actionable Recommendations:**
- Include sample sizes to avoid over-interpreting small groups
- Stratify by country or company size to control for structural pay differences
- Use for career path planning and skill prioritization

---

### 13. **Technology Gap Analysis: Languages & Databases** (Dumbbell & Gap Charts)
Three-panel visualizations showing the difference between "Have Worked With" and "Want To Work With" for technologies.

**Key Insights:**
- **Positive gap** indicates rising demand and learning interest
- Minimum threshold applied to avoid noise from niche technologies
- Gap leaders signal "next wave" technologies for hiring and training

**Actionable Recommendations:**
- Treat gap leaders as hiring priorities for future-ready teams
- Balance gap analysis with absolute counts to avoid overweighting niche tools
- Update skill development roadmaps based on gap rankings

---

### 14. **AI Tool Adoption Gap Leaderboard** (Acceleration Score)
Ranks AI tools by an acceleration score combining gap size and current adoption base.

**Key Insights:**
- Acceleration score = gap × log(current usage) to balance emerging vs established tools
- High scores indicate tools with both momentum and existing user base
- Filtered to exclude tools with minimal current adoption

**Actionable Recommendations:**
- Focus organizational AI strategy on high-acceleration tools
- Differentiate between mainstream adoption and experimental tools
- Monitor quadrant shifts (current vs interest rate) to identify inflection points

---

### 15. **Job Satisfaction Drivers** (Coefficient/Correlation Chart)
Shows top factors correlated with job satisfaction using linear regression or correlation analysis.

**Key Insights:**
- Directional signals only; not causal claims
- Standardized coefficients allow cross-variable comparison
- Model includes compensation, experience, education, and remote work factors

**Actionable Recommendations:**
- Treat results as hypotheses for deeper qualitative research
- Validate with ordinal regression or classification models
- Expand model with role-specific and country-specific controls for precision

---

## 🛠️ Technical Stack

- **Python 3.8+**
- **pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib & Seaborn**: Data visualization
- **scikit-learn**: Basic modeling (linear regression for satisfaction drivers)
- **Jupyter Notebook**: Interactive analysis environment

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Running the Analysis

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

2. Launch Jupyter Notebook:
```bash
jupyter notebook survey_data_exploration_cleaning_insights.ipynb
```

3. Execute cells sequentially to reproduce the analysis

> **Note**: The notebook requires a source data file (`survey_data_updated.csv`) which is not included in this repository. Please ensure you have access to a compatible survey dataset.

## 📈 Key Recommendations

### For Learners
- Prioritize skills with high demand gaps (identified in gap analysis)
- Build SQL and analytics competencies around top databases
- Develop AI-assisted workflow capabilities (prompting, QA, automation)

### For Hiring Managers
- Align technology stack planning with identified gap leaders
- Use segmented compensation benchmarks by role, region, and remote status
- Avoid over-investment in plateau technologies

### For Organizations
- Implement targeted upskilling programs for emerging tools
- Tailor remote work policies based on regional norms
- Address AI tool adoption barriers through training and integration support

## 📊 Methodology

1. **Data Acquisition**: Survey data ingestion and initial exploration
2. **Data Cleaning**: Standardization, type conversion, and missing value treatment
3. **Feature Engineering**: Age midpoint calculation, multi-select field parsing
4. **Exploratory Analysis**: Distribution analysis, correlation studies, trend identification
5. **Visualization**: Creating publication-ready charts and graphs
6. **Insight Generation**: Translating findings into actionable recommendations
7. **Presentation Development**: Executive summary and stakeholder communication

## ⚠️ Data Limitations

- Multi-select fields represent mentions, not unique respondents
- Self-reported compensation and experience may contain noise
- Country-level counts reflect survey reach, not population share
- Age ranges converted to midpoints introduce approximation
- Sample selection bias may affect generalizability

## 🔮 Future Enhancements

- [ ] Build interest-gap index by country and role for targeted planning
- [ ] Add sample-size thresholds and confidence intervals for group comparisons
- [ ] Track year-over-year movement in adoption gaps
- [ ] Implement predictive models for job satisfaction drivers
- [ ] Normalize country comparisons by population or tech workforce data

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

This is a completed capstone project, but suggestions and improvements are welcome! Feel free to open an issue or submit a pull request.

## 📧 Contact

For questions or collaboration opportunities, please reach out via GitHub issues.

---

**Project Status**: ✅ Completed | **Last Updated**: January 2026

*This project demonstrates end-to-end data analysis capabilities including data wrangling, statistical analysis, visualization, insight generation, and executive communication.*
