# Insurance Oversight Dashboard

**End-to-end TPA oversight system processing 1-100M rows from 120,000+ insurance policies for risk monitoring, quality assessment, and regulatory compliance.**

## Architecture

**ETL Pipeline** (`insurance_data_processing.Rmd`)
- AWS Enterprise Data Warehouse integration with optimized sampling
- Harmonizes 7 data sources: transactions, claims, disbursements, policies, automated activities, annuity/life valuations
- Monthly delta processing with performance optimization for large datasets

**Interactive Dashboard** (`insurance_oversight_app.R`)
- Reactive R Shiny application with dynamic quality assessment forms
- Weighted scoring algorithms with 80% pass/fail thresholds
- Real-time KPI tracking and multi-period trend analysis
- Parquet-based persistence for review history and audit trails

## Key Features

- **Executive KPIs**: Contract tracking, completion rates, dollar risk analysis
- **Quality Assessment**: Activity-specific checklists with weighted category scoring
- **Risk Monitoring**: Configurable thresholds, compliance tracking, exception management  
- **Analytics**: Historical performance trends with statistical modeling

## Business Impact

- **60% reduction** in manual review time through automated quality assessment
- **Standardized oversight** across all TPAs ensuring regulatory compliance
- **Executive visibility** with C-suite dashboard for proactive risk management
- **Presented to 50+ stakeholders** including C-level executives

## 🔒 Anonymization Notice

**This code is anonymized from a real insurance industry project.** All company names, proprietary systems, business rules, and data have been replaced with generic placeholders. Technical architecture and methodologies remain unchanged to demonstrate capabilities.

## Technology Stack

- **Data**: R (tidyverse, dplyr, lubridate), AWS Enterprise Data Warehouse, Apache Arrow
- **Visualization**: Shiny, Plotly, ggplot2, DT
- **Analytics**: Statistical modeling, weighted scoring, logistic regression

## Usage

```r
# Install dependencies
install.packages(c("shiny", "shinydashboard", "DT", "dplyr", 
                   "plotly", "arrow", "tidyverse", "lubridate"))

# Configure database connection in .creds.R
# Run ETL pipeline
source("insurance_data_processing.Rmd")

# Launch dashboard  
shiny::runApp("insurance_oversight_app.R")
```

## Skills Demonstrated

- **Data Engineering**: Large-scale ETL, AWS integration, performance optimization
- **Full-Stack Development**: Interactive dashboards, reactive programming, database integration
- **Analytics**: Statistical modeling, business intelligence, regulatory compliance tracking
- **Leadership**: Stakeholder management, cross-functional collaboration, executive reporting

---
*Developed during data engineering internship showcasing enterprise-level analytics and dashboard development*
