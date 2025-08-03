# SQL Data Analysis Projects

A comprehensive collection of SQL data analysis projects showcasing various analytical techniques, data visualization, and insights from different datasets.

## Project Overview

This repository contains multiple SQL analysis projects focused on different domains and datasets. Each project demonstrates various SQL techniques, data manipulation, and analytical insights.

## Project Structure

```
SQL_PROJECT/
├── Excels/
│   ├── coffee/
│   │   ├── coffeedata.xlsx      # Coffee dataset (157KB)
│   │   ├── Dashboard.xlsx       # Interactive dashboard (364KB)
│   │   └── readme.md           # Coffee project documentation
│   └── README.md               # Excel projects documentation
├── MySQL/
│   └── Indian Census Population_SQL_Project/
│       ├── Dataset1.csv        # Census data - demographics
│       ├── Dataset1.xlsx       # Excel version of dataset 1
│       ├── Dataset2.csv        # Census data - population & area
│       ├── Dataset2.xlsx       # Excel version of dataset 2
│       ├── Loading file.sql    # Database setup and data loading
│       ├── Analysis.sql        # Comprehensive SQL analysis (6.5KB)
│       ├── output1.sql         # Analysis output 1
│       └── output2.sql         # Analysis output 2
└── README.md                   # Main project documentation
```

## Projects Included

### 1. Coffee Industry Analysis (Excel/SQL)

**Location**: `Excels/coffee/`

**Description**: Comprehensive analysis of coffee industry data including sales performance, market trends, customer behavior, and product metrics.

**Key Features**:
- Raw coffee dataset analysis
- Interactive dashboard with visualizations
- Sales performance metrics
- Market trend analysis
- Customer behavior insights
- Geographic distribution analysis

**Files**:
- `coffeedata.xlsx` (157KB) - Primary dataset
- `Dashboard.xlsx` (364KB) - Interactive visualizations
- `readme.md` - Project-specific documentation

### 2. Indian Census Population Analysis (MySQL)

**Location**: `MySQL/Indian Census Population_SQL_Project/`

**Description**: In-depth analysis of Indian census data covering population demographics, literacy rates, sex ratios, and growth patterns across different states and districts.

**Key Features**:
- Population analysis by state and district
- Literacy rate calculations and rankings
- Sex ratio analysis
- Growth rate comparisons
- Top and bottom performing states
- Demographic insights

**Files**:
- `Dataset1.csv/xlsx` - Demographics data (Growth, Sex Ratio, Literacy)
- `Dataset2.csv/xlsx` - Population and area data
- `Loading file.sql` - Database setup and data import
- `Analysis.sql` - Comprehensive SQL queries and analysis
- `output1.sql` & `output2.sql` - Analysis results

## Analysis Capabilities

### Coffee Analysis
- Sales performance tracking
- Market trend identification
- Customer segmentation
- Product performance metrics
- Geographic market analysis
- Revenue optimization insights

### Census Analysis
- Population density calculations
- Literacy rate comparisons
- Sex ratio analysis by state
- Growth rate trends
- State-wise performance rankings
- Demographic pattern identification

## Technical Requirements

### Prerequisites
- MySQL Server (for census analysis)
- Microsoft Excel or compatible spreadsheet software
- SQL client (MySQL Workbench, phpMyAdmin, etc.)
- Basic understanding of SQL queries and data analysis

### Database Setup
1. Install MySQL Server
2. Create database using provided SQL scripts
3. Import CSV data using the loading scripts
4. Execute analysis queries

## Getting Started

### For Coffee Analysis
1. Navigate to `Excels/coffee/`
2. Open `coffeedata.xlsx` to explore raw data
3. Review `Dashboard.xlsx` for pre-built visualizations
4. Use SQL queries for custom analysis

### For Census Analysis
1. Navigate to `MySQL/Indian Census Population_SQL_Project/`
2. Execute `Loading file.sql` to set up database
3. Run `Analysis.sql` for comprehensive analysis
4. Review output files for results

## SQL Analysis Examples

### Census Analysis Queries
```sql
-- Total Population of India
SELECT sum(Population) AS 'Total Population' FROM Data2;

-- State-wise Average Growth
SELECT state, avg(Growth)*100 AS 'Average Growth'
FROM data1
GROUP BY State 
ORDER BY 'Average Growth' DESC;

-- Top 3 States by Literacy Rate
SELECT state, round(avg(literacy),0) 'Average Literacy Rate'
FROM data1
GROUP BY State 
ORDER BY 'Average Literacy Rate' DESC
LIMIT 3;
```

## Data Sources

- **Coffee Data**: Industry-specific dataset with sales and market information
- **Census Data**: Official Indian census data with demographic indicators
 
**Project Type**: SQL Data Analysis  
**Primary Focus**: Coffee Industry & Indian Census Analytics  
**Technologies**: MySQL, Excel, SQL Analysis
