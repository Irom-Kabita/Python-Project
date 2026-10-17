# Employee & Project Management Analysis (Python)
📖 **Project Overview**
Developed a Python-based data analysis project to clean, transform, and analyze employee, project, and designation datasets. The project demonstrates essential data preprocessing techniques, business rule implementation, and data aggregation using Pandas and NumPy to generate meaningful employee and project insights.

🎯 **Business Objective**
- Consolidate employee, project, and designation data into a single dataset.
- Improve data quality by handling missing values and restructuring data.
- Automate bonus calculations and designation updates based on business rules.
- Generate employee and project performance metrics for decision-making.

📊 **Key Metrics & KPIs**
- Total Project Cost per Employee
- Project Completion Status (Finished, Ongoing, Failed)
- Employee Bonus Eligibility
- Designation Level Changes (Promotion & Demotion)
- Employee Distribution by City

🔑 **Key Features**
- Cleaned missing project cost values using a running average approach.
- Split employee names into First Name and Last Name.
- Merged multiple datasets using Employee ID.
- Applied business rules for bonus calculation and designation updates.
- Calculated total project cost for each employee using aggregation.
- Filtered employee records based on business requirements.

🛠️ **Tools & Technologies**
- Python
- Pandas
- NumPy
- Jupyter Notebook

📂 **Files Included**
- Python capstone project.ipynb – Python Notebook

**Generated outputs**
- employee.csv
- project.csv
- seniority.csv

**⚙️ Setup and How to Run**

Requirements

- Python 3.13.9
- Jupyter Notebook 
- Pandas 2.3.3
- NumPy 2.3.5

Installation

Make sure Python is installed on your computer. Open a terminal or Command Prompt and run:

pip install pandas numpy notebook

Running the Notebook

1. Download or clone this repository.

2. Open a terminal or Command Prompt in the project folder.

3. Launch Jupyter Notebook by running:
   
   jupyter notebook

4. Open "Python capstone project.ipynb".

5. Run all cells in order, starting from the first cell.

Note: The notebook generates "employee.csv", "project.csv", and "seniority.csv". Run the notebook from the beginning so these files are created before later cells attempt to read them.

📝 **Data Handling, Transformations and Business Rules**

- Data cleaning: Remove unnecessary columns, including the gender column, as implemented in the notebook.
- Name transformation: Split employee names into first and last names and use NumPy ("np.where") to assign titles such as "Mr." and "Mrs." based on the project's defined conditions.
- Missing project costs: Replace missing costs with the running average of previously encountered non-missing project costs.
- Bonus calculation: Assign a bonus equal to 5% of project cost to projects marked "Finished". Other project statuses receive zero bonus.
- Designation updates: Adjust designation levels according to the notebook's rules, including age-based promotion and failed-project demotion. Keep designation levels within the defined limits.
- Project cost aggregation: Calculate total project cost for each employee using Pandas grouping and aggregation.
- Data filtering: Filter employee records according to specified conditions, such as selecting cities containing the letter "o", regardless of case.
- Dataset integration: Combine employee, project and designation data using Employee ID.

Note: This project is a sample data analysis exercise. The transformations and business rules demonstrate Python data manipulation techniques and do not represent actual company HR policies.
