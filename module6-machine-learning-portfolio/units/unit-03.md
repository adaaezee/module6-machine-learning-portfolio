# Unit 3 - Correlation and Regression

[← Back to e-portfolio](../README.md) · **LO2, LO3**

**Artefact:** Regression progression and multicollinearity check ([team report](../projects/unit-06-team-project/Team_F_Group_4_Project_Report.pdf), pages 3–5)

The team built regression in three steps: distance alone (R² = 0.15), multiple regression with room type and borough, then degree-2 polynomial regression (R² = 0.51). A variance inflation factor check found borough above 10, showing it overlapped heavily with distance. As a result, their separate effects could not be read independently (Wooldridge, 2020).

**What I learned:** a model with good fit can still have coefficients that cannot be interpreted. Checking for correlation between predictors comes before explaining them.
