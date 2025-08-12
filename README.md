# Insurance Oversight Dashboard

## Project Overview
End-to-end TPA oversight dashboard built during insurance industry internship. Processes 1-100 million rows from 120,000+ policies to monitor risk, quality, and regulatory compliance through automated scoring and executive reporting.

## Technical Architecture

**ETL Pipeline** (`zinnia_data_processing.Rmd`)
- AWS Enterprise Data Warehouse integration
- Harmonizes 7+ data sources (transactions, claims, disbursements, policies, valuations)
- Monthly delta processing with performance optimization

**Interactive Dashboard** (`insurance_oversight_app.R`)
- Reactive R Shiny application with dynamic forms
- Plotly/ggplot2 visualizations for KPI tracking
- Weighted quality scoring with 80% pass/fail thresholds
- Parquet-based data persistence

## Key Features
- **Executive KPIs**: Real-time contract tracking, completion rates, risk distribution
- **Quality Assessment**: Standardized checklists with weighted scoring algorithms
- **Risk Monitoring**: Dollar threshold analysis and compliance exception tracking
- **Trend Analytics**: Multi-period performance analysis with predictive insights

## Business Impact
- 60% reduction in manual review time through automation
- Standardized oversight across all TPAs for regulatory compliance
- C-suite dashboard enabling proactive risk management
- Presented to 50-60 stakeholders including executives

## 🔒 Privacy Notice
**This code is anonymized from a real insurance project.** All company names, proprietary systems, business rules, and data have been replaced with generic placeholders to protect confidential information. Technical architecture and methodologies remain unchanged.

## Technology Stack
- **Data**: R (tidyverse, dplyr, lubridate), AWS, Apache Arrow
- **Visualization**: Shiny, Plotly, ggplot2
- **Analytics**: Statistical modeling, logistic regression, weighted scoring

## Usage
```r
# Install dependencies
install.packages(c("shiny", "shinydashboard", "DT", "dplyr", 
                   "plotly", "arrow", "tidyverse"))

# Run ETL pipeline
source("zinnia_data_processing.Rmd")

# Launch dashboard
shiny::runApp("insurance_oversight_app.R")
```

## Skills Demonstrated
- Large-scale ETL pipeline development and AWS integration
- Interactive dashboard design with reactive programming
- Statistical modeling and business intelligence
- Stakeholder communication and cross-functional leadership

---
*Developed during data engineering internship demonstrating enterprise-level analytics capabilities*
