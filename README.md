# Secure Data Governance Project

## Overview
The Secure Data Governance project aims to enhance data quality and security by implementing governance techniques such as data cleaning, profiling, and schema validation. The project focuses on automotive industry datasets to analyze competitive factors influencing car pricing.

## Dataset Description
The project utilizes two datasets from different car companies, with key features including:
- **Make** (Brand of the car)
- **Year of Publication**
- **Car Components** (Engine type, fuel type, usage, number of doors, etc.)
- **Pricing Factors** (Market competitiveness and pricing based on features)

## Problem Definition
The datasets contained various issues:
1. **Null Values**:
   - Dataset 1: `Engine Cylinders`, `Market Category`, `Engine HP`, `Engine Fuel Type`
   - Dataset 2: `Make`, `Model`, `Trim`, `Body`, `Condition`, `Odometer`, `Color`, `Interior`, `MMR`, `Selling Price`, `Sale Date`
2. **Duplicates**:
   - Presence of duplicate records that could skew analysis

## Methodology
### Data Cleaning
- **Handling Duplicates**:
  - Removed duplicate records to ensure data integrity.
- **Handling Null Values**:
  - Replaced missing values in numerical columns with the **mean** of the respective column.

### Data Profiling
- Used `dataprofiler` to analyze dataset structure and identify inconsistencies.

### Schema Validation
- **Defined schema** using `cerberus` to enforce expected data formats and constraints.
- **Inferred schema** using `pandera` to validate data types dynamically.

### Security Measures
- Implemented governance techniques to ensure dataset integrity and prevent unauthorized modifications.

## Results
- **Cleaned datasets**: All null values and duplicates were removed, ensuring consistent data types.
- **Enhanced data quality**: Improved dataset informativeness for better analysis and decision-making.

## Conclusion
By applying rigorous data governance practices, the project successfully improved dataset reliability and accuracy. This ensures better analytical insights, aiding automotive companies in market competitiveness and strategic planning.

## Technologies Used
- **Python Libraries**: Pandas, NumPy, dataprofiler, cerberus, pandera
- **Jupyter Notebook**: Data processing and visualization

## Getting Started
### Prerequisites
Ensure you have the following dependencies installed:
```bash
pip install pandas numpy dataprofiler cerberus pandera
```

### Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/Anasmahmoud00/Secure-Data-Data-Governance.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Secure-Data-Data-Governance
   ```
3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook Governace_project-1.ipynb
   ```




