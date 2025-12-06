# Understanding Secondary School Student Performance with Bayesian Modelling

This project uses Bayesian regression and hierarchical models to understand which factors influence
final Portuguese language grades for students in two Portuguese secondary schools.

It was originally completed as part of the ST308 *Bayesian Inference* course.

---

## Research question

> Which study habits, socio-economic variables and school-related factors are most strongly associated with
> students’ final Portuguese language grade?

The outcome variable is:

- **`G3`** – final Portuguese language grade (integer from 1 to 20). 

---

## Data

- **Dataset:** “Student Performance” (Portuguese course) from the **UCI Machine Learning Repository**.
- **Original variables:** 33 variables including grades (`G1`, `G2`, `G3`), demographics, family background, and school-related factors.
- **Outcome:** `G3` (final grade in Portuguese).
- **Predictors used in the final analysis (all categorical):**

  - `school` – school (GP = Gabriel Pereira, MS = Mousinho da Silveira)
  - `studytime` – weekly study time (4 ordered categories)
  - `failures` – number of past class failures
  - `schoolsup` – extra educational support (yes/no)
  - `higher` – wants to pursue higher education (yes/no)
  - `Dalc` – weekday alcohol consumption (1–5)
  - `goout` – going out with friends (1–5)
  - `health` – current health status (1–5)
  - `Fjob` – mother’s job (teacher, healthcare, civil services, at home, other) Reference[oaicite:3]{index=3}  

The dataset contains no missing values. For modelling, the data are split into **training (90%)** and **test (10%)** sets. 
