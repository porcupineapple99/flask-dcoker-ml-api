# flask-dcoker-ml-api

Q1:
Estimated Average Treatment Effect (τ̂): -9.106
p-value for τ̂: 0.0004

Interpretation:
→ The treatment effect is statistically significant at the 5% level.

Under the following assumptions, τ̂ can be interpreted causally:
1. Unconfoundedness: No unmeasured confounders; treatment is as good as random given X.
2. Linearity: The relationship between engagement, treatment, and spending is linear.
3. SUTVA: No interference between corporations and only one version of treatment per unit.




Q2:

Explanation of Components
app.py defines a Flask web API that trains a linear regression model using stakeholder engagement data and exposes a /predict endpoint to generate predictions based on user inputs (W and X).

Dockerfile specifies the environment and dependencies needed to run the Flask app, ensuring that the same setup works consistently across different machines or platforms.

Containerization improves reproducibility by packaging the code, libraries, and environment settings into a single Docker image, allowing others to run the exact same application without dealing with version conflicts or local setup issues.

