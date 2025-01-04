# Data

If using an external dataset (that doesn't come in an R package), place data file(s) in this folder.

Then, include metadata about your dataset including information on provenance, data dictionary, etc.

The data dictionary for your data file(s) using the following format.

## Employee_Compensation.csv

| Variable            | Description                                                                                               | Datatype           |
|---------------------|-----------------------------------------------------------------------------------------------------------|--------------------|
| data_as_of          | Timestamp at which the data was last updated.                                                             | Floating Timestamp |
| data_loaded_at      | Timestamp at which the data was loaded to the open data portal.                                             | Floating Timestamp |
| Department          | The City department at which the employee was employed.                                                    | Text               |
| Department Code     | A three-digit identifier indicating the City department in which the employee was employed.                | Text               |
| Employee Name       | Name of the employee compensated by the City.                                                             | Text               |
| Employment Type     | The type of employment. Possible values: Permanent Civil Service, Permanent Exempt, Temporary Provisional, Temporary Exempt, Other                                  | Text               |
| Health and Dental   | Averaged health and dental benefits to protect employee privacy as legally required.                        | Number             |
| Hours               | The number of hours worked by the employee.                                                               | Number             |
| Job                 | Jobs are defined by the Human Resources classification unit. Examples include gardeners, police officers.  | Text               |
| Job Code            | Jobs are defined by the Human Resources classification unit. Examples include gardeners, police officers.  | Text               |
| Job Family          | Job Family combines similar Jobs into meaningful groups.                                                   | Text               |
| Overtime            | Amounts paid to the employee working in excess of 40 hours per week.                                       | Number             |
| Other Benefits      | Mandatory benefits such as Social Security contributions and minor discretionary benefits.                 | Number             |
| Other Salaries      | Various irregular payments including premium pay, incentive pay, or one-time payments.                    | Number             |
| Retirement          | City contributions to employee retirement plan.                                                           | Number             |
| Salaries            | Normal salaries paid to the employee.                                                                     | Number             |
| Total Benefits      | The sum of all benefits paid to the employee.                                                             | Number             |
| Total Compensation  | The sum of all salaries and benefits paid to the employee.                                                  | Number             |
| Total Salary        | The sum of all salaries paid to City employees. (Salaries + Overtime + Other Salaries)                                                          | Number             |
| Union               | Unions represent employees in collective bargaining agreements.                                            | Text               |
| Union Code          | Unions represent employees in collective bargaining agreements. A job belongs to one union.                | Text               |
| Year                | An accounting period of 12 months. The Fiscal Year ending June 30, 2012 is represented as FY2011-2012.     | Text               |
| Year Type           | Fiscal (July through June) or Calendar (January through December).                                         | Text               |


