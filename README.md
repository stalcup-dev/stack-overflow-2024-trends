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

## 📊 Visualizations & Insights

All 20+ visualizations from the analysis are displayed below with detailed insights and recommendations.

---

### 1. Top 10 Skills and Tools

![Top Skills](images/01_top_skills_tools.png)

**Insights**: Concentrated adoption in core technologies (JavaScript, SQL, Python) with long-tail opportunities in niche tools. Multi-select responses mean totals exceed respondent count.

**Recommendations**: Compare "Have vs Want" to identify demand gaps; segment by experience/role for targeted skill development.

---

### 2. Age Distribution

![Age Distribution](images/02_age_distribution.png)

**Insights**: Distribution reflects survey reach patterns. Age midpoint conversion introduces approximation.

**Recommendations**: Use broader cohorts for stability; cross-reference with experience metrics.

---

### 3. Top 15 Countries

![Top Countries](images/03_top_countries.png)

**Insights**: US, Germany, and India lead responses. Counts reflect survey reach, not workforce proportions.

**Recommendations**: Normalize by population; set minimum sample thresholds for comparisons.

---

### 4. Job Satisfaction

![Job Satisfaction](images/04_job_satisfaction.png)

**Insights**: Most developers report satisfaction levels of 7-8/10. Context-dependent (role, comp, remote status).

**Recommendations**: Segment by workplace factors; track trends over time.

---

### 5. Compensation Distribution

![Compensation Distribution](images/05_compensation_distribution.png)
![Compensation Box Plot](images/06_compensation_boxplot.png)

**Insights**: Right-skewed distribution; median more representative than mean. Wide variance within experience bands.

**Recommendations**: Use medians; apply log scales; segment by role/region.

---

### 6. Compensation by Remote Work

![Compensation by Remote](images/07_compensation_by_remote.png)

**Insights**: Compensation differences across remote/hybrid/in-office reflect geography and policy.

**Recommendations**: Control for cost-of-living; track policy evolution.

---

### 7. Experience vs Compensation

![Experience vs Compensation](images/08_experience_vs_compensation.png)

**Insights**: Positive correlation with substantial noise. Experience alone explains limited variance.

**Recommendations**: Add median bands; segment by role/location.

---

### 8. Correlations Heatmap

![Correlations](images/09_correlations_heatmap.png)

**Insights**: Experience metrics highly correlated; weak correlation with compensation.

**Recommendations**: Use for multivariate model screening; investigate multicollinearity.

---

### 9. Remote Work by Country

![Remote Work by Country](images/10_remote_work_by_country.png)

**Insights**: Significant variation across countries reflects cultural/policy differences.

**Recommendations**: Consider regulatory environments; compare with satisfaction/compensation.

---

### 10. Compensation by Education

![Compensation by Education](images/11_compensation_by_education.png)

**Insights**: Education effect varies by role; professional degrees show highest median.

**Recommendations**: Cross-reference with experience; group similar degrees.

---

### 11. AI Tools Adoption

![AI Tools](images/12_ai_tools_adoption.png)

**Insights**: "Writing code" and "Search for answers" dominate current usage. Gap between current and interested reveals opportunities.

**Recommendations**: Prioritize high-interest/low-usage tools for training.

---

### 12. Compensation by Developer Type

![Compensation by DevType](images/13_compensation_by_devtype.png)

**Insights**: Engineering managers and executives earn highest median. Specialization impacts compensation.

**Recommendations**: Include sample sizes; stratify by geography.

---

### 13. Languages Gap Analysis

![Languages Dumbbell](images/14_languages_gap_dumbbell.png)
![Languages Ranking](images/15_languages_gap_ranking.png)
![Languages Heatmap](images/16_languages_heatmap.png)

**Insights**: Rust and Go show largest positive gaps. Gap leaders signal next-wave technologies.

**Recommendations**: Treat gap leaders as hiring priorities; balance with absolute counts.

---

### 14. Databases Gap Analysis

![Databases Dumbbell](images/14_databases_gap_dumbbell.png)
![Databases Ranking](images/15_databases_gap_ranking.png)
![Databases Heatmap](images/16_databases_heatmap.png)

**Insights**: PostgreSQL and Redis show strong positive gaps. Emerging databases gaining interest.

**Recommendations**: Update skill roadmaps; focus training on gap leaders.

---

### 15. AI Adoption Leaderboard

![AI Leaderboard](images/20_ai_adoption_leaderboard.png)
![AI Quadrant](images/21_ai_quadrant.png)

**Insights**: Predictive analytics, deployment monitoring, and code review show high acceleration scores.

**Recommendations**: Focus AI strategy on high-acceleration tools; monitor quadrant shifts.

---

### 16. Job Satisfaction Drivers

![Job Satisfaction Drivers](images/22_job_satisfaction_drivers.png)

**Insights**: Work experience and years coding show strongest correlations with satisfaction.

**Recommendations**: Treat as directional signals; validate with multivariate models.

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
git clone https://github.com/stalcup-dev/stack-overflow-2024-trends.git
cd stack-overflow-2024-trends
```

2. Launch Jupyter Notebook:
```bash
jupyter notebook survey_data_exploration_cleaning_insights.ipynb
```

3. Execute cells sequentially to reproduce the analysis

> **Note**: The notebook requires a source data file (`survey_data_updated.csv`) which is not included in this repository. Please ensure you have access to a compatible survey dataset.

## 📈 Key Recommendations

### For Learners
- Prioritize skills with high demand gaps (Rust, Go, PostgreSQL, Redis)
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
