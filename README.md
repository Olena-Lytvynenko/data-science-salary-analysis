# Data Science Salary Analysis - Comprehensive Market Dynamics Study (2020-2025)

The Data Science job market has experienced unprecedented transformation over the past five years. But what really drives salary differences in this field? Is it company size, geographic location, experience level, or perhaps the emergence of revolutionary AI technologies like ChatGPT?

This project takes a comprehensive dive into all these factors to understand what actually determines Data Science compensation. The goal is to uncover which workplace characteristics, economic conditions, and technological trends drive higher salaries, and which factors professionals should prioritize for career growth.

The analysis is built around evidence-based insights that can help data professionals optimize their career strategies and help companies develop competitive compensation frameworks that attract top talent in an increasingly competitive market.

The project is divided into 3 key blocks, each focusing on specific market forces and providing actionable findings with strategic recommendations for both job seekers and employers. After each section, I deliver key insights and practical advice that can be directly applied to career planning, hiring strategies, and business decision-making.

**Data sources**: 
- [Kaggle - Salaries for Data Science Jobs](https://www.kaggle.com/datasets/adilshamim8/salaries-for-data-science-jobs/data)
- [World Bank Open Data API](https://datahelpdesk.worldbank.org/) (95 countries)
- [Wikimedia REST API](https://wikimedia.org/api/rest_v1/) (English Wikipedia only)

## Dataset Description

The analysis integrates three comprehensive datasets spanning 2020-2025, capturing both traditional market factors and emerging technological trends. Below is a detailed description of the key data sources:

### Salary Dataset
| Column Name | Description |
|-------------|-------------|
| `work_year` | Year salary was reported (2020-2025) |
| `experience_level` | EN (Entry), MI (Mid), SE (Senior), EX (Executive) |
| `employment_type` | FT (Full-time), PT (Part-time), CT (Contract), FL (Freelance) |
| `job_title` | Specific position (Data Scientist, ML Engineer, etc.) |
| `salary_in_usd` | Standardized salary in USD |
| `remote_ratio` | 0 (On-site), 50 (Hybrid), 100 (Fully remote) |
| `company_location` | Country code where company is located |
| `company_size` | S (Small 1-50), M (Medium 51-500), L (Large 501+) |
| `employee_residence` | Country where employee lives |

### World Bank Economic Indicators
| Column Name | Description |
|-------------|-------------|
| `country_code` | ISO country code (AD, AE, US, etc.) |
| `country_name` | Full country name (Andorra, United States, etc.) |
| `year` | Data year (2020-2025) |
| `value_population` | Total population count |
| `value_gdp_per_capita` | GDP per capita in current USD |
| `value_education` | Percentage with Bachelor's degree or higher |
| `value_internet` | Internet penetration rate (%) |

### Wikipedia Page Views
| Column Name | Description |
|-------------|-------------|
| `date` | Collection date (2020-01-01 to 2025-06-29) |
| `keyword` | Technology term (chatgpt, ai, ml, dl, python) |
| `views` | Daily page views count (English Wikipedia only) |
| `category` | Technology category (AI, Programming) |
| `period` | ChatGPT release period (before, after) |

**Data Format:**
- **CSV format**: All datasets provided in CSV format for seamless integration
- **Temporal coverage**: Complete 2020-2025 timeline capturing pre/post-ChatGPT eras
- **Geographic scope**: 95 countries with comprehensive economic indicators
- **Technology focus**: AI/ML keyword tracking measuring public interest trends

## Analytical Methods and Tools Used

This project employs rigorous statistical methods to uncover salary determinants across workplace, economic, and technological dimensions:

**Tools:**
- **Python Libraries:**
 - `pandas`, `numpy`: Data manipulation and statistical analysis
 - `matplotlib`, `seaborn`, `plotly`: Advanced data visualization
 - `scikit-learn`: Machine learning and correlation analysis
 - `scipy`: Statistical hypothesis testing (t-tests)
 - `aiohttp`, `asyncio`: Asynchronous data collection

**Analysis Methods:**
- Correlation analysis and multivariate comparisons
- Statistical hypothesis testing for salary difference validation
- Time series analysis for trend identification
- Cross-sectional analysis by demographic and geographic factors
- Before/after comparative analysis for ChatGPT impact assessment

## Research Focus Areas

**Block 1: Workplace & Professional Factors**
Comprehensive analysis of how company characteristics and professional positioning affect Data Science compensation. This block examines company size impact on salaries, remote work patterns across different organizational scales, highest-paying positions in the field, career progression potential from entry to senior levels, employment type distributions, and experience level effects on work flexibility. Key findings include actionable insights for professionals choosing between companies of different sizes and remote work preferences.

**Block 2: Economic Factors Impact**
In-depth investigation of macroeconomic influences on Data Science salaries globally. The analysis tests whether high-GDP countries provide premium compensation, examines correlations between economic indicators and salary levels, and identifies optimal geographic targets for maximum earning potential. This block provides strategic guidance for international career planning and helps companies understand global compensation benchmarks.

**Block 3: AI Revolution Impact on Data Science**
Revolutionary analysis of how ChatGPT's emergence transformed both public interest in AI and Data Science compensation structures. This block tracks Wikipedia search trends for AI technologies, measures ChatGPT's explosive growth compared to traditional technologies, analyzes the creation of new AI-specific roles, and quantifies salary premiums for AI specialization. The findings reveal how technological breakthroughs create market opportunities and guide career specialization decisions.

## Tableau Dashboard

A comprehensive interactive Tableau dashboard was created to explore key findings, including:

- Salary trends across company sizes, experience levels, and geographic regions
- ChatGPT impact visualization with before/after comparisons
- AI vs traditional Data Science role compensation analysis
- Digital nomad flow patterns and remote work trends
- Interactive filters for company size, employment type, experience level, remote work ratio, role category, and work year 

[Tableau - Dashboard link](https://public.tableau.com/views/DataScienceSalaryDashboard2020-2025/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## How to Use This Project

1. **Start with data collection notebooks** - understand data sources and collection methodology
2. **Review data cleaning procedures** - see how raw data was processed and validated
3. **Explore the main analysis notebook** - comprehensive findings across all three research blocks
4. **Interact with the Tableau dashboard** for dynamic exploration of insights
5. **Clone the repository** for full analysis reproduction and customization
6. **Apply strategic insights** to your Data Science career planning or hiring strategy

## Data Science Salary Analysis Project Structure

This project is organized into focused Jupyter notebooks that systematically address different aspects of the Data Science market, from data collection to comprehensive analysis. Each notebook serves a specific purpose in building a complete picture of salary determinants.

### Notebooks Overview

**Data Collection Phase:**
- `00_data_collection_wikipedia.ipynb ` - AI/ML technology interest trends via Wikipedia API
- `01_data_collection_worldbank.ipynb` - Economic indicators collection via World Bank API

**Data Cleaning Phase:**
- `02_data_cleaning_salaries.ipynb` - Salary dataset preprocessing and quality validation
- `03_data_cleaning_worldbank.ipynb` - World Bank data cleaning and standardization

**Main Analysis:**
- `04_comprehensive_salary_analysis.ipynb` - Complete analysis across all three research blocks
 - Workplace & Professional Factors analysis
 - Economic Factors correlation study  
 - AI Revolution impact assessment with ChatGPT analysis

**Tableau Data Preparation:**
- `05_data_preparation_tableau.ipynb` - Systematic data preprocessing and transformation for interactive dashboard visualization

### Who This Project Benefits

**For Data Science Professionals:**
- Career optimization strategies based on market evidence
- Geographic targeting for maximum salary potential
- Specialization recommendations for highest growth trajectories
- Remote work insights for lifestyle and compensation balance

**For Companies and HR Teams:**
- Competitive compensation benchmarking across markets
- Talent acquisition strategies for different company sizes
- Understanding of AI skills premium and market demand
- Remote work policy insights for talent retention

**For Researchers and Analysts:**
- Methodology for technology impact assessment on job markets
- Economic factor integration techniques for salary analysis
- Before/after analysis framework for technological disruptions
- Multi-source data integration best practices

### Purpose

The project provides a comprehensive framework for understanding Data Science market dynamics through the lens of workplace characteristics, economic foundations, and technological disruption. Each analysis block delivers both statistical findings and practical recommendations, making complex market data accessible and actionable for career planning, business strategy, and academic research.
