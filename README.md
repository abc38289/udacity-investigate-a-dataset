# Udacity-Data-Analyst-Nanodegree
# Project: Investigate a Dataset - Medical Appointment No shows¶

### Date created

Jerry Liu created this project on January 2, 

## Project Overview

In this project, I will analyze a dataset and then communicate my findings about it. I will use the Python libraries NumPy and pandas to make my analysis easier.

## Dataset Description
**Selected dataset**: [No-show appointments](https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd2e9a_noshowappointments-kagglev2-may-2016/noshowappointments-kagglev2-may-2016.csv)

This dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row.

- **`PatientId`**: indicates the patient ID; duplication is possible due to cases where the same patient booked more than one appointment.

- **`AppointmentID`**: indicates appoint ID, this field should be unique
- **`Gender`**: indicates the patient's gender (M/F)
- **`ScheduledDay`**: indicates the Date/Time the patient set up their appointment.
- **`AppointmentDay`**:  indicates the date/time the patient called to book their appointment.
- **`Age`**: indicates the patient's age.
- **`Neighborhood`**: indicates the location of the hospital.
- **`Scholarship`**: indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.
- **`Hipertension`**: indicates whether or not the patient is experiencing Hypertension.
- **`Diabetes`**: indicates whether or not the patient is experiencing Diabetes.
- **`Alcoholism`**: indicates whether or not the patient is experiencing Alcoholism.
- **`Handcap`**: indicates whether or not the patient is with special needs.
- **`SMS_received`**: indicates whether or not the patient has received a reminder text message.
- **`Show-up`**: ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.


## Why this Dataset?

What interests me about this dataset is that it is more close to everyone. Once people have to reserve something, there will be a no-show. So, it aroused my curiosity to find out what factors are more important in affecting the no-show rate.

## Question(s) for Analysis

The major problem that we want to know is:
>What factors are important for us to know in order to predict if a patient will show up for their scheduled appointment?

So we ask some questions below in order to find the answer:
1. What is the overall percentage of no-show appointments?
2. Is there a difference in the no-show rates between male and female patients?
3. Is there a relationship between the time gap from scheduling an appointment to the actual appointment and the likelihood of a no-show?
4. How does the age of the patient correlate with the likelihood of a no-show?
5. Are there specific neighborhoods where the no-show rate is higher?(Top 5)
6. Does having a scholarship (Bolsa Família) influence the likelihood of a no-show?
7. Is there a relationship between each health conditions (e.g., hypertension, diabetes) and no-show appointments?
8. Which health condition combinations affect no-show appointments the most?¶
9. Does receiving one or more SMS messages affect the no-show rate?


## Summary of Main Findings:

According to the research above, we found that `Appointment scheduling interval`, `age`, `neighborhoods`, `health condition combinations` and `SMS` will affect the no-show rate.

Some situations will decrease the no-show rate beyond our thought. For instance, the no-show rate will increase when a patient receives an SMS message.

It shows that there are some factors we do not know to study further. 


Our findings:


**1. What is the overall percentage of no-show appointments?¶**

The overall no-show rate is 20.19%.

**2. Is there a difference in the no-show rates between male and female patients?**

There is no significant difference between males and females in terms of no-show rates.

**3. Is there a relationship between the time gap from scheduling an appointment to the actual appointment and the likelihood of a no-show?**

The no-show rate will increase once the interval is over 30 days.

**4. How does the age of the patient correlate with the likelihood of a no-show?**

Once a patient is over 40 years old, the no-show rate starts to decrease.

**5. Are there specific neighborhoods where the no-show rate is higher?(Top 5)**

The neighborhoods with the top five no-show rates are 'SANTOS DUMONT', 'SANTA CECÍLIA', 'SANTA CLARA', 'ITARARÉ', and 'JESUS DE NAZARETH'.

**6: Does having a scholarship (Bolsa Família) influence the likelihood of a no-show?**

Although there is no significant difference between having a scholarship and the no-show rates, it shows that having a scholarship does increase the no-show rate.

**7. Is there a relationship between each health conditions (e.g., hypertension, diabetes) and no-show appointments?**

There is no significant difference between having each health condition will affect the no-show rates. But it is interest that having a health condition decreases the no-show rate a bit.

**8: Which health condition combinations affect no-show appointments the most?**

When a patient has all the health conditions, we can find that it affects the no-show rate the most, over 30%. However, the no-show rate decreases when other combinations of health conditions are involved.

**9. Does receiving one or more SMS messages affect the no-show rate?**

Surprisingly, patients who received SMS messages were more likely to miss their appointments than those who did not receive messages.

These findings provide valuable insights into factors influencing no-show rates, allowing for more targeted strategies to reduce appointment non-attendance.