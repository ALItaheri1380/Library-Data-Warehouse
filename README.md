# Library Data Warehouse

This repository contains the implementation of a data warehouse system designed for managing and analyzing data related to a library system. The goal of this project is to build an ETL (Extract, Transform, Load) pipeline that aggregates data from different sources and stores it in a well-structured data warehouse, allowing for efficient querying and analysis.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [ETL Process](#etl-process)
- [Data Model](#data-model)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The Library Data Warehouse project aims to create a comprehensive data warehouse for a library system. The system integrates data from various sources, processes it through an ETL pipeline, and stores it in a structured format to support business intelligence and reporting.

## Project Structure

The repository is organized as follows:

```
Library-Data-Warehouse/
│
├── data/                # Raw data and data sources
├── etl/                 # ETL scripts and processes
├── sql/                 # SQL scripts for data warehouse management
├── models/              # Data models and schemas
├── reports/             # Analysis and reporting scripts
└── README.md            # Project documentation
```

## Technologies Used

This project uses the following technologies and tools:

- **SQLSERVER**: All the codes of this project are written with sql server


## Usage

This guide outlines the steps for setting up and running the data warehouse:

1. Create Data Source Tables:
   * Define and create the tables that will house your raw data, directly from your data sources. This is the foundation of your data warehouse.

2. Load Data into Data Source Tables:
   * Execute the data loading scripts (likely in your ETL package) to populate the data source tables. Ensure the data is accurate and complete.

3. Create Staging Area Tables:
   * Construct staging area tables to temporarily hold the transformed data before it's loaded into the final data warehouse tables.

4. Execute the ETL Process:
   * Run the ETL scripts (which might be separate from the data loading scripts) to transform and load data from the staging area into the final data warehouse tables.

5. Clean and Validate Data:
   * Implement data cleansing and validation procedures to identify and remove inaccurate or incomplete data in your staging area. This is crucial for maintaining data quality.

6. Create Dimension Tables:
   * Design and build dimension tables to store reference data and metadata associated with your data warehouse's facts. 

7. Build Temporary Tables and Logging:
   * Create temporary tables for logging the ETL process. This will help you track errors and monitor the pipeline's progress.

8. Execute Procedures and Processes:
   * Develop and execute stored procedures to automate various tasks, including data cleaning, transformation, and loading.

Important Note:  
This process is highly iterative. You may need to refine your data source table definitions and ETL processes as you gain a better understanding of your data and business requirements.

## ETL Process

The ETL process in this project involves the following steps:

1. **Extract**: Data is extracted from various sources such as CSV files, APIs, or databases.
2. **Transform**: The extracted data is cleaned, transformed, and organized into a suitable format for loading into the data warehouse.
3. **Load**: The transformed data is loaded into the PostgreSQL data warehouse, structured according to the defined data models.

## Data Model

The data warehouse is designed to accommodate the following entities:

- **Books**: Information about books available in the library.
- **Authors**: Details about authors of the books.
- **Members**: Data about library members.
- **Borrowing**: Records of books borrowed by members.

The data model is designed to be scalable and supports efficient querying for reporting purposes.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or need further assistance, feel free to reach out:
- Email: taheri.a@ec.iut.ac.ir
