# Data-Analytics-Internship-Project-Syscorp-Technology-Pvt-Ltd

# End-to-End Business Data Analytics and Visualization System

A comprehensive, production-ready business analytics system that demonstrates the complete data pipeline from raw data to actionable insights.

## Project Overview

This project showcases a 120-day structured workflow implementation including:
- Excel Analytics
- SQL Database Management  
- Python Data Analysis
- Power BI Dashboard Design
- Final Capstone Project

## Architecture

```
Deepu-Analytics-System/
|
|-- 01_Excel_Analytics/          # Excel-based analysis and reporting
|   |-- datasets/                # Sample sales datasets
|   |-- analysis_files/          # Pivot tables and chart data
|   |-- reports/                 # Excel reports
|
|-- 02_SQL_Database/             # Database layer
|   |-- schema/                  # Table creation scripts
|   |-- queries/                 # Business analytics queries
|   |-- procedures/              # Stored procedures
|   |-- sample_data/             # Sample data insertion
|
|-- 03_Python_Analysis/          # Python analytics
|   |-- scripts/                 # Data processing scripts
|   |-- notebooks/               # Jupyter notebooks
|   |-- modules/                 # Python modules
|   |-- outputs/                 # Generated outputs
|
|-- 04_Data_Visualization/      # Visualization layer
|   |-- powerbi/                 # Power BI dashboard models
|   |-- dashboards/              # Dashboard configurations
|   |-- assets/                  # KPI definitions
|
|-- 05_Capstone_Project/         # End-to-end implementation
|   |-- backend/                 # Data pipeline
|   |-- analysis/                # Business insights
|   |-- dashboard/               # Interactive dashboard
|   |-- reports/                 # Generated reports
|
|-- data/                        # Data management
|   |-- raw/                     # Raw data files
|   |-- cleaned/                 # Cleaned data
|   |-- processed/               # Processed data
|
|-- docs/                        # Documentation
|-- config/                      # Configuration files
|-- scripts/                     # Utility scripts
|-- tests/                       # Test files
```

## Features

### 1. Excel Analytics
- Sample sales, customer, and product datasets
- Pivot table templates for analysis
- Chart-ready data structures
- Automated report generation

### 2. SQL Database
- Complete MySQL schema with 7 tables
- 20+ business analytics queries
- 10 stored procedures for common analyses
- Views for complex reporting
- Sample data for testing

### 3. Python Analysis
- Data cleaning and preprocessing
- Exploratory data analysis
- Advanced visualizations
- Statistical analysis
- Machine learning insights

### 4. Data Visualization
- Power BI dashboard models
- Interactive dashboard configurations
- KPI definitions and metrics
- Executive and sales dashboards

### 5. Capstone Project
- End-to-end data pipeline
- Automated insights generation
- Interactive Streamlit dashboard
- Customer segmentation
- Revenue forecasting

## Quick Start

### Prerequisites
- Python 3.8+
- MySQL 8.0+
- Microsoft Excel (for Excel analytics)
- Power BI Desktop (for visualization)

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd Deepu-Analytics-System
```

2. **Install Python dependencies**
```bash
cd 03_Python_Analysis
pip install -r requirements.txt
```

3. **Set up MySQL database**
```bash
cd 02_SQL_Database/schema
mysql -u root -p < create_tables.sql
mysql -u root -p < ../sample_data/insert_sample_data.sql
```

4. **Run data cleaning pipeline**
```bash
cd 03_Python_Analysis/scripts
python data_cleaning.py
```

5. **Generate insights**
```bash
python eda.py
python visualization.py
```

6. **Launch interactive dashboard**
```bash
cd 05_Capstone_Project/dashboard
streamlit run app.py
```

## Usage

### Excel Analytics
1. Navigate to `01_Excel_Analytics/datasets/`
2. Open `sales_data.csv`, `customers.csv`, `products.csv` in Excel
3. Use pivot tables in `analysis_files/` for analysis
4. Review reports in `reports/` folder

### SQL Database
1. Connect to MySQL database
2. Run queries from `02_SQL_Database/queries/`
3. Execute stored procedures from `02_SQL_Database/procedures/`

### Python Analysis
1. Run data cleaning: `python data_cleaning.py`
2. Perform EDA: `python eda.py`
3. Create visualizations: `python visualization.py`
4. Open Jupyter notebooks for interactive analysis

### Interactive Dashboard
1. Run pipeline: `python ../backend/data_pipeline.py`
2. Launch dashboard: `streamlit run app.py`
3. Access at `http://localhost:8501`

## Key Components

### Data Pipeline
- **Extract**: CSV files, database tables, APIs
- **Transform**: Data cleaning, validation, enrichment
- **Load**: CSV outputs, database tables, reports

### Analytics Modules
- **Customer Segmentation**: K-means clustering, RFM analysis
- **Product Analysis**: Affinity analysis, performance metrics
- **Revenue Forecasting**: Time series analysis, trend prediction
- **Churn Prediction**: Customer behavior analysis

### Visualizations
- **Executive Dashboard**: High-level KPIs and trends
- **Sales Dashboard**: Detailed sales performance metrics
- **Customer Dashboard**: Customer analytics and segmentation
- **Product Dashboard**: Product performance and profitability

## Business Insights

The system provides insights in:
- **Revenue Performance**: Trends, forecasts, growth analysis
- **Customer Analytics**: Segmentation, LTV, churn risk
- **Product Performance**: Affinity analysis, profitability
- **Regional Analysis**: Geographic performance comparison
- **Operational Metrics**: Efficiency, fulfillment rates

## Configuration

### Database Configuration
Edit `config/config.yaml`:
```yaml
database:
  host: localhost
  port: 3306
  database: business_analytics
  user: root
  password: your_password
```

### Environment Variables
Create `.env` file:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=business_analytics
```

## Testing

Run the test suite:
```bash
cd tests
python test_pipeline.py
python test_analytics.py
```

## Deployment

### Docker Deployment
```bash
docker-compose up -d
```

### Manual Deployment
1. Set up MySQL database
2. Configure environment variables
3. Install Python dependencies
4. Run data pipeline
5. Deploy dashboard

## Monitoring

- Pipeline logs: `data_pipeline.log`
- Analysis logs: `eda_analysis.log`, `visualization.log`
- Dashboard metrics: Available in Streamlit interface

## Contributing

1. Fork the repository
2. Create feature branch
3. Make changes
4. Add tests
5. Submit pull request

## License

This project is for educational and demonstration purposes.

## Support

For questions or issues:
1. Check the documentation
2. Review the logs
3. Create an issue in the repository

---

**Project Status**: Production Ready
**Last Updated**: 2024-04-15
**Version**: 1.0.0
