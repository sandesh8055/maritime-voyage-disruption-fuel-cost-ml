# Vessel Voyage Disruption & Fuel Cost Impact Prediction

## Overview
Maritime voyages operate under uncertain conditions such as changing sea states,
varying vessel loads, port congestion, and crew readiness.
Disruptions during a voyage can lead to delays, increased fuel consumption,
and significant cost overruns.

This project demonstrates how machine learning can be used as a
**decision-support tool** to:
- Predict the likelihood of voyage disruptions
- Estimate the additional fuel cost impact caused by such disruptions

The emphasis is on **interpretability, operational relevance, and responsible use**
of machine learning rather than complex black-box models.

---

## Problem Statement
Before a vessel departs, operators must assess risk under uncertainty.

This project addresses two key planning questions:
1. *Is a given voyage at risk of disruption?*
2. *If a disruption occurs, what could be the additional fuel cost impact?*

By separating disruption risk from cost impact estimation,
the project mirrors real-world maritime operational workflows.

---

## Data Strategy
Due to the proprietary and sensitive nature of real maritime operational data,
a **synthetic dataset** is generated to simulate realistic voyage conditions.

The dataset includes:
- Sea state conditions
- Vessel load levels
- Port congestion levels
- Engine efficiency
- Crew experience
- Route distance (nautical miles)
- Voyage disruption indicator
- Additional fuel cost impact (USD)

Synthetic data generation allows explicit modeling of cause–effect relationships
while avoiding the use of confidential or restricted information.

---

## Exploratory Data Analysis (EDA)
EDA focuses on identifying key drivers of voyage disruption and fuel cost escalation,
including:
- Environmental risk from rough sea states
- Operational bottlenecks caused by port congestion
- Human and mechanical factors such as crew experience and vessel load
- Cost amplification effects on long-distance voyages

The analysis prioritizes **decision-oriented insights** over exhaustive visualization.

---

## Modeling Approach
Two simple and interpretable models are used:

- **Logistic Regression** for voyage disruption risk prediction
- **Linear Regression** for additional fuel cost impact estimation

These models are intentionally selected to:
- Ensure transparency and explainability
- Support trust in maritime operational environments
- Avoid black-box decision-making in safety- and cost-critical systems

---

## Evaluation
Model evaluation focuses on practical usefulness rather than maximum accuracy:
- Classification metrics and confusion matrix for disruption prediction
- MAE and RMSE for fuel cost impact estimation

In maritime operations, failing to identify a high-risk voyage
is often more costly than exercising caution on a low-risk one.

---

## Limitations & Ethical Considerations
- The dataset is synthetic and based on assumed relationships.
- Real-world maritime operations involve additional factors such as
  regulatory constraints, geopolitical risks, and unexpected mechanical failures.
- Model outputs should not be used as the sole basis for operational decisions.

Machine learning is positioned as a **planning aid for human decision-makers**,
not as an autonomous navigation or control system.

---

## Conclusion
This project illustrates a responsible application of machine learning
to maritime voyage disruption and fuel cost impact analysis.

By emphasizing operational context, interpretability, and limitations,
the project highlights how ML can support proactive and cost-aware
maritime planning without replacing human expertise.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
  
## Author
Sandesh Duduskar
