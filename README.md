# Ethical-AI-Assignment

Part 1: Theoretical Understanding (30%)

Q1: What is Algorithmic Bias?

Algorithmic bias refers to systematic and repeatable errors in AI systems that result in unfair outcomes. These biases can be introduced through training data, model assumptions, or deployment environments.

Examples:

A hiring algorithm that favors male resumes over female ones because historical training data contained more successful male candidates.

A credit scoring system that assigns lower scores to minorities due to biased historical lending data.

Q2: Transparency vs Explainability

Transparency is the openness about how an AI system operates (e.g., revealing the model architecture or data sources).

Explainability is the ability to interpret and understand an AI system’s outputs.

Importance:
Transparency builds trust and allows auditing. Explainability helps users and developers understand why a model made a specific decision, crucial for accountability and ethical deployment.

Q3: GDPR Impact on AI Development

The GDPR enforces user rights in the EU by:

Requiring explicit user consent for data collection

Granting users the "right to explanation" of AI decisions

Imposing penalties for non-compliance

Impact: AI developers must design systems with privacy, fairness, and accountability from the outset (Privacy by Design).

Ethical Principles Matching

Principle

Definition

A) Justice

Fair distribution of AI benefits and risks

B) Non-maleficence

Ensuring AI does not harm individuals or society

C) Autonomy

Respecting users’ right to control their data and decisions

D) Sustainability

Designing AI to be environmentally friendly

Part 2: Case Study Analysis (40%)

Case 1: Amazon’s Biased Hiring Tool

Source of Bias: The training data was based on resumes from predominantly male applicants, leading to penalization of resumes with the word "women’s" or all-women colleges.

Fixes:

Re-train the model on a balanced and diverse dataset

Remove gender-related features and proxies

Incorporate fairness constraints during model optimization

Fairness Metrics:

Demographic parity

Equal opportunity (equal true positive rate across genders)

False positive/negative rate difference

Case 2: Facial Recognition in Policing

Ethical Risks:

Misidentification of minorities can lead to wrongful arrests and legal consequences

Violates privacy and civil liberties through constant surveillance

Responsible Policies:

Ban use in high-stakes decisions until accuracy is equitable

Require human oversight on final decisions

Independent audits and public transparency reports

Part 3: Practical Audit (25%)

Task: Analyze bias in the COMPAS Recidivism Dataset using IBM AI Fairness 360 Toolkit

Key Steps:

Load COMPAS dataset and define protected attributes (e.g., race)

Evaluate metrics: False Positive Rate (FPR), Disparate Impact, Equal Opportunity Difference

Visualize group-level disparities (e.g., bar charts of FPR for African-American vs Caucasian groups)

Summary (300 words):
The audit reveals higher false positive rates for African-American defendants. This indicates systemic bias, likely stemming from historical criminal justice data. Mitigation could involve reweighing the dataset, applying bias-aware algorithms (e.g., adversarial debiasing), or shifting to interpretable models.

Recommendations:

Implement post-processing correction methods

Include stakeholder review (civil rights experts)

Use multiple fairness metrics, not just accuracy

Part 4: Ethical Reflection (5%)

Reflection:
In a mental health prediction project for university students, I plan to integrate ethics from day one. I'll ensure fairness by using demographically diverse data, respect privacy via anonymization, and include a transparency layer that allows counselors and students to understand risk scores. Open-sourcing the model and encouraging community audits will further enhance trust.

Bonus Task: Ethical AI in Healthcare (Optional)

Policy Proposal: Guidelines for Ethical AI Use in Healthcare

Patient Consent Protocols:

Obtain explicit informed consent before using personal health data

Clearly explain AI’s role in decision-making

Bias Mitigation Strategies:

Train on demographically diverse datasets

Perform regular bias audits with tools like Fairlearn or AIF360

Transparency Requirements:

Provide explanations for AI-generated recommendations

Publish model documentation and performance reports

These guidelines foster trust, reduce harm, and ensure equitable healthcare outcomes for all patients.
