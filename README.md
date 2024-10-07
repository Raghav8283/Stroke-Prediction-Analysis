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

|  Job Type  |  Total ID's  |  % of Total   |  Stroke%  |  Post-stroke patients  |
|------------|--------------|---------------|-----------|------------------------|
|  Private   |    2921      |    57.16%     |   4.96%   |       145              |
|  Self-employed   |    818      |    16.01%     |   7.82%   |      64             |
|  Children   |    687      |    13.44%     |   0.29%   |       2             |
|  Government job   |    656      |    12.84%     |   4.88%   |       32              |
|  Never worked   |    22      |    0.43%     |   0.00%   |       0              |
|  NA  |    6      |    0.12%     |   100%   |       6              |
|  **TOTAL**   |    **5110**      |    **100%**    |   **4.87%**  |       **249**             |

Stroke is more significant with Self-employed and Private job individuals.

## Insights:
1. The high-risk age segment faces a significantly higher risk of stroke.
2. Individuals who are currently married have over 81% higher likelihood of experiencing a stroke compared to those who are never married which is 10%.
3. Females have a marginally higher likelihood of experiencing a stroke compared to males.
4. Job type may play a role in stroke prediction. So individuals in private jobs and self-employed individuals appear to have a slightly higher chances of experiencing a stroke in these categories of workers.

## Category variable Vs Target variable
we use **Stroke** as a target variable which is shown as "0" (never had a stroke) and "1"(Had a Stroke at least once)

#### A. Gender
|  Stroke  |  Female  |  Male  |  NA  |  Other  | Total  |
|---------|-----------|--------|------|---------|--------|
|    0    |  58.69%   |  41.29%|      | 0.02%   |  **100%**  |
|    1    |  53.01%   |  42.57%| 4.42%|         |  **100%**  |
| **Total**   |**58.41%**|**41.35%**|**0.22%**|**0.02%**|**100%**|

**Recommendation:** Focus on preventive measures for both genders, with special attention to Females.

#### B. Marital Status
|  Ever Married?  |  Stroke Count  |
|-----------------|----------------|
|  Yes            |   203          |
|  No             |    25          |
|   NA            |    21          |
|**Total**        |   **249**      |

**Recommendation:** Prioritize preventive strategies for married individuals.

#### C. Residence Type
|  Residence Type  |  Stroke Count  |
|-----------------|----------------|
|  Urban            |   132          |
|  Rural             |   111          |
|   NA            |    6        |
|**Total**        |   **249**      |

**Recommendation:** Address urban lifestyle factors to reduce stroke risk.


#### D. Age Risk
|  Age Related Risk  |  Stroke Count  |
|-----------------|----------------|
|  High Risk Age            |   206         |
|  Low Risk Age             |   43         |
|**Total**        |   **249**      |

**Recommendation:** Individuals with high-risk factors have a significantly higher stroke rate.

#### E. Heart Disease
|  Heart Disease  |  Stroke %  |
|-----------------|----------------|
|   0           |   4.19%         |
|  1             |   17.09%        |
|**Total**        |   **4.87%**      |

**Recommendation:** Manage and prevent heart diseases rigorously.

#### F. Hypertension
|  Heart Disease  |  Stroke %  |
|-----------------|----------------|
|   0           |   3.98%         |
|  1             |   13.28%        |
|**Total**        |   **4.87%**      |

**Recommendation:**  Control blood pressure effectively.

## Continuous vs Target Analysis

## A. Age
|  Stroke  |  Average age  |
|-----------------|----------------|
|   0           |   41.97        |
|  1             |   67.25        |
|**Total**        |   **43.20**      |


## B. Glucose level
|  Stroke  |  Avg of glucose level  |
|-----------------|----------------|
|   0           |   104.59        |
|  1             |   132.54       |
|**Total**        |   **105.96**      |

## C. BMI
|  Stroke  |  Average Age  |
|-----------------|----------------|
|   0           |   23.83        |
|  1             |   30.20        |
|**Total**        |   **28.89**      |

**Recommendation:**  

* Age is certainly a factor for a stroke so focus preventive measures on older adults as they are at higher risk.
* Control blood glucose levels effectively
* BMI doesn't seem to have an impact here. Nevertheless, a proper diet and exercise is imperative.


# Conclusion and Recommendations
The results demonstrated out of our models achieved high recall for stroke cases despite the imbalanced nature of the dataset. Age was found to be a significant predictor, along with other factors such as work type and other health realted condition. The developed model can serve as a valuable tool in identifying individuals at risk of stroke and implementing preventive interventions.

Further analysis and exploration are recommended to delve deeper into genetic factors, long-term effects of lifestyle modifications, advanced predictive models, socioeconomic and cultural factors, novel biomarkers, imaging techniques, and personalized stroke prevention strategies.
























