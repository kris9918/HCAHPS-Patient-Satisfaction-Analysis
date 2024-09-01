# HCAHPS Patient Satisfaction Analysis

<img src="https://github.com/user-attachments/assets/55d46300-b074-4645-8362-f0dbba73b9e3" alt="description" width="800"/>

## Overview
The Hospital Consumer Assessment of Healthcare Providers and Systems (HCAHPS) is a standardized survey that measures patients' perspectives on their hospital care experiences. Developed by the Centers for Medicare & Medicaid Services (CMS) in partnership with the Agency for Healthcare Research and Quality (AHRQ), HCAHPS provides a national standard for collecting and publicly reporting data on patients' experiences in hospitals across the United States. The survey includes 29 questions that assess various aspects of patient care, such as communication with nurses and doctors, responsiveness of hospital staff, cleanliness and quietness of the environment, pain management, and overall satisfaction.

This project aims to explore HCAHPS data through a comprehensive analysis using SQL for data wrangling and Tableau for visualization. By cleaning, transforming, and analyzing the survey data, this project seeks to identify key trends and insights into patient satisfaction and hospital performance. The visualizations created in Tableau will help stakeholders easily interpret the data, enabling healthcare providers to make informed decisions to improve the quality of care and patient experience.

## Data Source
The data used in this project comes from the Hospital Consumer Assessment of Healthcare Providers and Systems (HCAHPS) survey, publicly available through the Centers for Medicare & Medicaid Services (CMS) website. The HCAHPS data provides detailed insights into patient feedback across various dimensions of hospital care, collected from patients discharged from hospitals in the United States.

## Tools and Technologies
 - Microsoft Excel: Used for initial data exploration, cleaning, and quick analysis. Excel's functionalities such as sorting, filtering, and basic statistical functions help in understanding the structure of the data before deeper analysis.

- PostgreSQL: used for data wrangling, cleaning, and transformation. PostgreSQL allows for efficient querying and manipulation of large HCAHPS datasets, enabling complex data operations such as joins, aggregations, and filtering to prepare the data for analysis.

- Tableau: used to create interactive dashboards and visual representations of the HCAHPS survey data. Tableau enables the transformation of raw data into easy-to-understand visualizations that highlight key trends, patterns, and insights, making it accessible for stakeholders to interpret and act upon.

## Methodology

This project employs a structured approach to data cleaning, transformation, and visualization to ensure that the HCAHPS survey data is accurate and ready for analysis. Data preparation is conducted using SQL in PostgreSQL, followed by visualization in Tableau.

### 1. Data Cleaning and Preparation
Data cleaning focuses on standardizing and integrating information from the HCAHPS survey and related hospital data:

- **Extracting Raw Data**: The initial step involves selecting raw survey data, which includes patient satisfaction metrics and hospital identifiers.

- **Preparing Hospital Bed Data**: A Common Table Expression (CTE) is used to clean and format hospital bed data. Key actions include standardizing provider numbers to a consistent format and converting date fields to a usable format.

- **Joining Data**: The cleaned hospital bed data is then joined with the HCAHPS survey data to enrich the dataset, ensuring that each hospital's data is correctly aligned with the most recent bed information.

### 2. Data Transformation
- **Standardization**: Date fields are standardized, and identifiers are formatted consistently to ensure data integrity.
- **Integration**: Combines patient survey results with hospital characteristics, providing a comprehensive view for analysis.

### 3. Visualization
The cleaned data is imported into Tableau, where interactive dashboards are created to visualize patient satisfaction scores, hospital performance trends, and key insights.

### 4. Analysis and Insights
- **Insights**: Data visualizations are analyzed to identify trends, patterns, and areas for improvement in patient care and hospital operations.


## Conclusions

The dashboard offers valuable insights through five key sections, each providing crucial information for stakeholders:

### 1. Percent of Patient Rating 9 or 10
Displays the percentage of patients who rated their experience as 9 or 10. This metric highlights overall patient satisfaction and identifies hospitals with exceptional performance.

### 2. Survey Response Rate
Shows the rate of completed surveys relative to those distributed. A higher response rate indicates more reliable data and helps ensure a representative sample of patient feedback.

### 3. Number of Completed Surveys
Indicates the total number of surveys collected. This metric reflects the volume of feedback and the robustness of the data for analysis.

### 4. Number of Completed Surveys (Distinct Count)
Highlights the count of unique patients who completed the survey. Ensures the accuracy of feedback by avoiding duplicate responses.

### 5. Question Delta from Mean Percentage
Shows the deviation of each question’s percentage score from the mean percentage. Identifies specific areas of concern or excellence by comparing individual question scores to the average.


## Future Work

### 1. Enhanced Data Integration
Future work will focus on integrating additional data sources, such as demographic information and operational metrics, to provide a more comprehensive view of patient satisfaction.

### 2. Advanced Analytics
Implement advanced analytics techniques, including machine learning models, to predict trends in patient satisfaction and identify potential areas for improvement more accurately.

### 3. Improved Data Collection
Enhance data collection methods to increase the survey response rate and ensure a more representative sample of patient feedback.
