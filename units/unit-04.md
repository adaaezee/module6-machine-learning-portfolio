# Unit 4 - Linear Regression with Scikit-Learn

[← Back to e-portfolio](../README.md) · **LO3**

**Artefact:** Polynomial regression pipeline ([notebook](../projects/unit-11-individual-presentation/airbnb_ml.ipynb), Section 4)

I built degree-2 polynomial regression as a scikit-learn `Pipeline`, expanding six features into 27 terms. Wrapping the expansion in the pipeline means it is refitted inside each cross-validation fold, which prevents information leaking between training and validation data. Across five folds, RMSE was 0.450 ± 0.005.

**What I learned:** how a model is validated matters as much as which model is chosen. The pipeline structure is what makes the validation trustworthy.
