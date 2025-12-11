# Call-Center-Data-analysis-and-Dashboard

# “Power BI Dashboard & Data Cleaning on Call Center Dataset”

# 1. Data Import & Initial Exploration

I started the project by importing the CSV dataset into Power BI Power Query Editor.
Once loaded, I spent 1 to 2 hours fully understanding the dataset. Instead of rushing to visuals, I focused on analyzing:

-> Identified column meanings (Agent Name, Date, Call Duration, Customer Satisfaction Score, etc.)
-> Understood how the fields were related
-> Reviewed value ranges and patterns
-> Counted missing values
-> Checked inconsistent labels (e.g., “Yes/No” vs “Y/N”)
-> Verified column data types
-> Observed wrong date formats
-> Spotted numeric fields stored as text

   This deep understanding helped me plan how to clean and structure the data effectively.

# 2. Data Cleaning, Formatting & Transformation (Power Query)

After gaining familiarity with the dataset, I performed comprehensive data cleaning:

# Handling Missing Values
-> Removed rows containing null values in critical columns like
   Date, Agent Name, Call Answered, Call Duration
-> Replaced or standardized minor missing category values if feasible

# Fixing Incorrect Data Types
-> I ensured every column had the correct format:
-> Date columns → Date format
-> Call duration → Whole number or decimal
-> Customer Satisfaction Score ratings → Number
-> Agent names & categories → Text

Incorrect data types were converted to avoid calculation errors during DAX measures.

# Formatting & Standardization
-> Converted inconsistent text to proper categorical format
   Example: "resolved", "Resolved", "RESOLVED" → "Resolved"
-> Renamed columns to follow a clean and readable structure
-> Removed unnecessary symbols or spaces from text columns
-> Cleaned special characters in categorical fields

# Filtering Out Unwanted Rows
-> Removed blank entries
-> Eliminated system-generated or irrelevant data
-> Filtered out test records or incomplete logs

# Final Data Validation
-> I performed a final scan across all columns to ensure:
-> No formatting issues
-> No unexpected blanks
-> No mismatched date ranges
-> Values were logical (e.g., negative call duration doesn’t exist)
-> This resulted in a reliable, accurate, and analysis-ready dataset.

# 3. DAX Measures Creation
-> To build a powerful analytics dashboard, I created several DAX measures such as:

-> Total Calls Received
-> Total Calls Answered
-> Total Calls Dropped
-> Average Handle Time 
-> Average Call Duration
-> Customer Satisfaction Score Average
-> Response Rate %
-> Agent Performance %
-> Call Distribution by Category

   These measures allowed me to generate accurate KPIs and comparisons across agents, dates, and categories.

   After the data cleanup and measure creation, I moved to dashboard development.

   # 4. Building the Power BI Dashboard

  #  Dashboard Layout Planning
-> Before placing visuals, I decided on a structured layout:
-> Top Section: Key KPIs for quick understanding
-> Middle Section: Agent performance breakdown
-> Bottom Section: Call trends, categories, and customer satisfaction patterns
-> Right Side: Filters & Slicers for dynamic analysis
-> This provided a clean, intuitive flow for users.

# Creating Visualizations
-> I used a combination of visuals to bring insights to life:

# KPIs Cards
-> Total Calls
-> Answered Calls
-> Dropped Calls
-> Average Handling Time
-> Average Customer Satisfaction Score

# Bar Chart
-> Agent-wise performance comparison
-> Calls answered vs dropped by agent
-> Average duration by agent

# Donut Charts
-> Call category breakdown
-> Issue type distribution

# Tables
-> Detailed call-level information
-> Agent-wise summary with conditional formatting

# Slicers
-> Date
-> Agent Name
-> Call Category

These slicers made the dashboard fully interactive.

# 5. Applying Design Principles
-> To make the dashboard professional and readable:
-> Used consistent color themes
-> Added data labels where necessary
-> Used icons for KPIs
-> Ensured visual spacing and alignment
-> Avoided overcrowding by grouping visuals logically

# 6. Insights Extraction
-> Finally, I reviewed the dashboard to capture key insights such as:
-> Peak call times
-> Best performing agents
-> Most common issue categories
-> Relationship between call volume and customer satisfaction
-> Patterns in call duration
-> Areas where service needs improvement

# 7. Final Review & Export
-> Validated all DAX calculations
-> Checked slicers and filters
-> Ensured accuracy of KPI numbers
-> Exported dashboard for sharing

The final dashboard provided a full analytical view of call center operations with actionable insights.
