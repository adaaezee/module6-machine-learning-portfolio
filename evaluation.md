# Evaluation: Final Project (Unit 11) vs Initial Project (Unit 6)

[← Back to e-portfolio](README.md)

Both projects used the same Airbnb dataset, so the comparison shows how my approach developed rather than how two different problems differed.

| | Unit 6 team project | Unit 11 individual project |
|---|---|---|
| Question | How is distance from Times Square associated with price, and what segments exist? | Which model type is better suited to recommending prices, and at what cost? |
| Methods | Linear, multiple and polynomial regression; k-means clustering | Polynomial regression vs a PyTorch neural network |
| Validation | Single train/test split; learning curve | 5-fold cross-validation plus a hold-out test set |
| Polynomial model | RMSE 0.488, R² 0.512 | RMSE 0.442, R² 0.553 |
| Explainability | None | SHAP for both models |
| Ethics and bias | Not addressed | Subgroup error analysis; privacy, fairness and harm |
| Business use | Described findings; limited recommendations | Framed as a host pricing tool, with a deployment design |

The polynomial results are not directly comparable. Unit 11 added more features and removed prices above $1,000, so the improvement reflects data preparation as much as modelling.

## What improved

The tutor's feedback on Unit 6 asked for more critical discussion of method choices, more on limitations, and clearer business value. Unit 11 responded to each. Cross-validation exposed something a single split would have hidden: the neural network failed on one fold, and that changed my recommendation. SHAP showed *why* the models predicted as they did, and the subgroup analysis showed *who* they served least well. Framing the work as a pricing tool for hosts gave every result a practical consequence.

## What did not improve

Unit 11 dropped clustering altogether, so the Unit 6 weakness of not interpreting the segments for business use was never fully resolved. Some limitations also carried over, such as label-encoding categorical variables. The biggest change was in my process rather than my results: I moved from describing what a model found to questioning whether it could be trusted.
