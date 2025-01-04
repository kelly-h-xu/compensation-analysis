# Explaining Factors Contributing to Total Compensation for San Francisco City Employees
For a full version of the report, including data cleaning deatils, EDA, variable selection, variable transformation, and more, see [written-report.pdf](https://github.com/kelly-h-xu/compensation-analysis/blob/a186f74c5a27c9a24e071de1fab4169118363ddf/written-report.pdf). 


Written in collaboration with: Mason Wu, Matias Pinto-Chavez, Suhas Kurapati. 

## Introduction
San Francisco is the United States city with the highest median household income. However, some have raised questions on whether San Francisco employees are overcompensated, with claims of excessive benefits and questionable overtime practices. 

With the rising scrutiny over high compensation figures, our analysis aims to provide insight into the impacts of different factors on Total Compensation in San Francisco, to 1) support decisions about budget allocations, overtime policies, and resource management to ensure fair and sustainable compensation practices, and 2) to help job seekers make informed decisions about employment opportunities and better assess their potential earnings.

## Data
<img width="697" alt="image" src="https://github.com/user-attachments/assets/c56b57d2-f0b2-4b45-a7ed-788a9871f316" />

## Methodology
We fit two multiple linear regression models:
### Model 1
| **Response Variable**              | **Predictor Variables**                                                             |
|------------------------------------|------------------------------------------------------------------------------------|
| Total Compensation (log transformed) | Salaries (log transformed), Hours (log transformed), Employment Type, Overtime Status, Retirement |

### Model 2
| **Response Variable**              | **Predictor Variables**                                                |
|------------------------------------|------------------------------------------------------------------------|
| Total Compensation (log transformed) | Hours (log transformed), Employment Type, Overtime Status, Retirement |


## Results
### Model Outputs
#### Model 1
<img width="627" alt="image" src="https://github.com/user-attachments/assets/16566582-8b34-4bd2-8174-20e97a02d7dd" />

#### Model 2
<img width="615" alt="image" src="https://github.com/user-attachments/assets/855c1957-d8d1-45a3-9803-1d6306dce739" />

The most significant factor that is expected to increase an employee's total compensation is retirement benefits. According to both of our models, receiving retirement benefits is expected to significantly increase total compensation by about 40%. Permanent employees are expected to make more than temporary employees, and working more hours is expected to result in a higher total compensation. Model 1 predicts a smaller impact of these factors on total compensation, while Model 2 predicts a much greater impact.

From our models, working overtime is not expected to lead to extreme increases in total compensation, which suggests that employees making hundreds of thousands of dollars in overtime are likely not represenative of the total population. However, more analysis is necessary before we can draw conclusions about the specific impacts of working overtime on total compensation, as our models offer contrasting information: From Model 1, employees who work overtime are expected to earn about 14% more than employees who do not, while from Model 2, employees who work overtime are expected to earn about 17% less than employees who do not.

More analysis is also necessary before we can draw conclusions about the impact of department on total compensation, as again, our models offer contrasting information. From Model 1, it is expected that the Municipal Transportation Agency is the most highly compensated, and the Board of Appeals is the least compensated. This is in direct contrast to the results from Model 2, likely due to the high multicollinearity in Model 1, which causes high variability in model coefficients.
