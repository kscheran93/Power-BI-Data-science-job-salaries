# Data Science Job Salaries Dashboard

## Snapshot of Dashboard (Power BI Service)

![Dashboard_Snapshot](https://app.powerbi.com/view?r=eyJrIjoiYWM2ZTBmMzAtMzI4NS00ZjcwLWEzYzYtZmUwZTViYTY4NDNhIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

### Dashboard Link: [Your Power BI Dashboard Link](https://app.powerbi.com/view?r=eyJrIjoiYWM2ZTBmMzAtMzI4NS00ZjcwLWEzYzYtZmUwZTViYTY4NDNhIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

## Problem Statement

This dashboard provides insights into the landscape of data science job salaries. It helps analyze factors such as salary distribution across different experience levels, employment types, company locations, and job titles. The insights derived from this dashboard can be valuable for job seekers, employers, and market analysts to understand salary trends and identify factors that influence compensation in the data science field.

### Steps Followed

- **Step 1:** Loaded the dataset into Power BI Desktop from the Kaggle dataset titled [“Data Science Job Salaries”](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries).

- **Step 2:** Cleaned and prepared the data using Power Query Editor, ensuring data integrity by removing any missing or duplicate entries, and converting data types as necessary.

- **Step 3:** In the Report View, I applied a canvas background color of `#F4F4F4` to maintain a clean and professional visual aesthetic.

- **Step 4:** Created visualizations:
  - **Stacked Column Chart:** Displays the average salary in USD by employment type and experience level.
    - **X-Axis:** `experience_level` & `employment_type`
    - **Y-Axis:** Average of `salary_in_USD`
    - **Format Settings:** 
      - Bars colored by experience level
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Average Salary in USD by Employment Type and Experience Level"
      - Divider: On, black color

  - **Clustered Bar Chart:** Shows the top 5 employee residences by count.
    - **Y-Axis:** `company_location`
    - **X-Axis:** Count of `company_location`
    - **Filters:** Applied Top N filter for the top 5 employee residences by using the count of `company_location`
    - **Format Settings:** 
      - Bars colored by company location
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Top 5 Employee Residences"
      - Divider: On, black color

  - **Table Chart:** Displays the average salary in USD by job title and experience level.
    - **Columns:** `job_title`, `experience_level`, Average of `salary_in_USD`
    - **Format Settings:**
      - Font: Black
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Average Salary in USD by Job Title and Experience Level"

  - **Doughnut Chart:** Shows the distribution of companies by size.
    - **Legend:** `company_size`
    - **Values:** Count of `company_size`
    - **Format Settings:**
      - Segments colored by company size
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Companies by Size"
      - Divider: On, black color

  - **Doughnut Chart:** Displays the distribution of experience levels.
    - **Legend:** `experience_level`
    - **Values:** Count of `experience_level`
    - **Format Settings:**
      - Segments colored by experience level
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Experience Levels"
      - Divider: On, black color

  - **Doughnut Chart:** Shows the distribution of employee types.
    - **Legend:** `employment_type`
    - **Values:** Count of `employment_type`
    - **Format Settings:**
      - Segments colored by employment type
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Employee Types"
      - Divider: On, black color

  - **Map Visualization:** Displays the average salary in USD by location.
    - **Location:** `company_location`
    - **Bubble Size:** Average of `salary_in_USD`
    - **Format Settings:**
      - Map Style: Dark
      - Bubble Colors: Conditional formatting based on average salary
      - Background: `#F4F4F4`
      - Title: Black, font size 16, "Average Salary in USD by Location"
      - Divider: On, black color

- **Step 5:** Added filters to allow users to explore the data based on:
  - **Company Location:** Field = `company_location`
  - **Job Title:** Field = `job_title`

- **Step 6:** Published the report to Power BI Service for broader accessibility.

## Insights

The dashboard provides several key insights into the data science job market:

### [1] Average Salary by Employment Type and Experience Level
   - The stacked column chart reveals how average salaries differ based on employment type (e.g., full-time, part-time) and experience level (e.g., junior, senior). This can guide job seekers in negotiating salaries and employers in setting competitive pay scales.

### [2] Top 5 Employee Residences
   - The clustered bar chart highlights the top 5 locations where employees reside, providing insights into geographical trends in data science employment.

### [3] Salary Distribution by Job Title and Experience
   - The table chart shows average salaries across different job titles and experience levels, helping to identify which roles and levels command higher pay.

### [4] Companies by Size
   - The doughnut chart visualizes the distribution of companies by size, giving an idea of the prevalence of small, medium, and large companies in the dataset.

### [5] Experience Levels
   - Another doughnut chart breaks down the experience levels of employees, offering insights into the workforce's composition in terms of experience.

### [6] Employee Types
   - This doughnut chart shows the distribution of employee types, indicating the proportion of full-time, part-time, and other employment types.

### [7] Average Salary by Location
   - The map visualization provides a geographical overview of average salaries, helping to identify which locations offer higher or lower compensation in data science.

### [8] Key Metrics
   - **Top Employee Residences:** [United States - 355]
   - **Top Experience Level:** [SE with 280(46.13%)]
   - **Top Employment Type:** [FT - 96.8%]
   - **Highest Average Salary Location:** [Russia with 157500 USD dollars]
