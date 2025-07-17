# Credit Risk Modeling

## Credit Scoring Business Understanding

### 1. How does the Basel II Accord’s emphasis on risk measurement influence our need for an interpretable and well-documented model?
Basel II requires financial institutions to rigorously measure and manage credit risk, emphasizing transparency, regulatory compliance, and capital adequacy. This means our credit risk models must be interpretable and well-documented so that both internal stakeholders and regulators can understand, validate, and trust the model’s predictions. Interpretability ensures that risk drivers are clear, model decisions can be explained, and compliance with regulatory standards is demonstrable.

### 2. Since we lack a direct "default" label, why is creating a proxy variable necessary, and what are the potential business risks of making predictions based on this proxy?
When a direct "default" label is unavailable, we must create a proxy variable (e.g., 90+ days past due) to approximate default events. This is necessary to train and evaluate the model. However, using a proxy introduces risks: the proxy may not perfectly represent true default behavior, potentially leading to misclassification, biased risk estimates, and suboptimal business decisions. Relying on an imperfect proxy can also expose the institution to regulatory scrutiny and financial losses if the model’s predictions do not align with actual risk.

### 3. What are the key trade-offs between using a simple, interpretable model (like Logistic Regression with WoE) versus a complex, high-performance model (like Gradient Boosting) in a regulated financial context?
Simple models (e.g., Logistic Regression with Weight of Evidence) are highly interpretable, easier to validate, and preferred by regulators for their transparency. They facilitate clear communication of risk factors and decision logic. Complex models (e.g., Gradient Boosting) may offer higher predictive accuracy but are less interpretable, harder to validate, and may face regulatory resistance. In regulated contexts, the trade-off is between maximizing predictive power and ensuring transparency, auditability, and regulatory acceptance. 