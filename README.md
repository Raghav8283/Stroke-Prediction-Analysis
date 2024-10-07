# Stroke Prediction using Power BI

![Alt Text](https://github.com/Raghav8283/Stroke-Prediction-Analysis/blob/main/Images/Stroke%20prediction%20Image.png)

According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths. This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.

## Datafile:

The dataset used in this project consists of 5110 observations with 12 attributes, including information on demographics, medical history, lifestyle factors, and stroke occurrence. The dataset was carefully prepared and explored, including handling missing values, performing descriptive statistics, and visualizing the data distribution.

## Descriptor Information

1. id:unique identifier
2. gender: "Male", "Female" or "Other"
3. age: age of the patient
4. hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5. heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6. ever_married: "Yes" or "No"
7. work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8. Residence_type: "Rural" or "Urban"
9. avg_glucose_level: average glucose level in blood
10. bmi: body mass index
11. smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"
12. stroke: 1 if the patient had a stroke or 0 if not *Note: "Unknown" in smoking_status means that the information is unavailable for this patient

## Data Preparation and Exploration:

The data preprocessing phase involved removing unnecessary columns, addressing missing values, categorizing features, and standardizing the data. Exploratory data analysis was conducted to gain insights into the dataset, including visualizations of categorical and numerical columns, identifying outliers, and examining correlations among variables.

## Univariate and Bivariate Analysis

Univariate analysis focuses on analyzing one variable at a time and Bivariate analysis focuses on analyzing any concurrent relation between two variables or attributes. Let’s explore the insights from a bivariate perspective based on the provided data.

## Stroke occurrences based on Age high risk group(individual age >55 group as High Risk,else Low):

### 1. Age Risk and Stroke

### High-Risk Age Group:

* Individuals aged greater than 55 are considered high-risk.
* This group includes 206 individuals who had a stroke in the past.
* They account for 82.73% of all stroke cases in the dataset.

### Low-Risk Age Group:

* Individuals aged below 55 fall into the low-risk category.
* Only 43 individuals in this group have had a stroke.
* They represent 17.27% of stroke cases.

### Implications:

* The high-risk age segment faces a significantly higher risk of stroke.
* Organizations and healthcare providers should focus on preventive measures and early detection for this base.
* Lifestyle modifications, regular health check-ups, and awareness campaigns can help mitigate stroke risk.


## Stroke occurrences based on marital status

### 2.Marital Status and Stroke:
The dataset includes individuals categorized by their marital status: unspecified (NA), currently married (Yes), and never married (No).

|  Unspecified  |  Married(Yes)  |  Married(No)  |
|---------------|----------------|---------------|
| 21 Individuals had a stroke | 203 Individuals had a stroke | 25 Individuals had a stroke |


## Stroke occurrences based on Gender

### 3. Gender and Stroke:
The dataset includes individuals categorized by gender: Female, Male, NA (Not Available), and Other.

|  Females total_id's  | Avg_Age | Stroke%   |  Males total id's  |  Avg_Age  |  Stroke%  |
|----------------------|---------|-----------|--------------------|-----------|-----------|
|       2985             |  43.70  |  4.42%    |     2113           |   42.46%  |  5.02%    | 

Not much of a outliers here.


## Stroke occurrences based on different job types

### Job Type and Stroke:
The dataset includes individuals categorized by their job types: children, government jobs, NA (not available), never worked, private jobs, and self-employed and the numbers indicate the following.













