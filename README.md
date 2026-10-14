# Healthcare Data Exploratory Data Analysis (EDA)

## Project Overview
This project explores a healthcare dataset using Python. It focuses on understanding patient information, admission patterns, medical conditions, billing amounts, and relationships between numerical variables.

## Objectives
- Inspect the dataset structure and summary statistics.
- Check for missing values and clean selected columns.
- Convert admission and discharge dates to datetime format.
- Calculate the length of each patient's stay.
- Explore admission types, medical conditions, gender, and billing amounts.
- Visualize patterns and relationships in the data.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Dataset
The notebook loads a CSV file named `healthcare_data_for_task - healthcare_data_for_task.csv`.

Place the CSV file in the notebook's working directory, or update the file path in the data-loading cell before running the notebook.

The notebook uses fields including:
- `Age`
- `Medical_Code`
- `Admission_Type`
- `Date_of_Admission`
- `Discharge_Date`
- `Billing_Amount`
- `Medical_Condition`
- `Gender`

## Workflow
1. Import the required Python libraries.
2. Load and inspect the dataset using `head()`, `shape`, `info()`, `describe()`, and `columns`.
3. Check missing values and fill missing `Medical_Code` values with `Unknown`.
4. Standardize `Admission_Type` text by trimming spaces and applying title case.
5. Convert admission and discharge dates to datetime values.
6. Calculate `Stay_Days` from discharge date minus admission date.
7. Explore billing statistics, average age by medical condition, and medical-condition counts by gender.
8. Create visualizations:
   - Admission type count bar chart
   - Stacked billing totals by medical condition and admission type
   - Billing amount distribution by medical condition (violin plot)
   - Monthly patient admissions line chart
   - Correlation heatmap for numerical columns

## How to Run
1. Download or clone this project and keep the notebook and dataset together.
2. Install the dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Open `EDA_Task5.ipynb` in Jupyter Notebook or upload it to Google Colab.
4. Make sure the CSV path in the notebook points to the dataset location.
5. Run the notebook cells from top to bottom.

## Notes
- The notebook's current CSV path is `/content/healthcare_data_for_task - healthcare_data_for_task.csv`, which is a Google Colab-style path. Change it if you are running locally.
- The notebook contains exploratory analysis and visualizations; it does not define a predictive model.
- Review the dataset's date columns and missing values before drawing conclusions from the charts.

