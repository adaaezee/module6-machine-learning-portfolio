# Unit 7 - Introduction to Artificial Neural Networks

[← Back to e-portfolio](../README.md) · **LO3**

**Artefact:** Feedforward network design ([notebook](../projects/unit-11-individual-presentation/airbnb_ml.ipynb), Section 5)

I designed a network with three hidden layers (6 → 64 → 32 → 16 → 1), using ReLU activations and 20% dropout, and about 3,000 parameters in total. I kept it deliberately small, because evidence suggests deep networks rarely outperform simpler models on tabular data (Shwartz-Ziv and Armon, 2022).

**What I learned:** in neural network design, choosing the size to suit the data is a decision you have to justify. Adding more layers does not automatically improve results.
