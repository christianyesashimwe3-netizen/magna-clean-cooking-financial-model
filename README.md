# magna-clean-cooking-financial-model
Financial feasibility model for the Magna Phase II clean cooking pilot.
# Magna Clean Cooking Project
## Phase II Financial Feasibility Model

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/christianyesashimwe3-netizen/magna-clean-cooking-financial-model/blob/main/Clean_Cooking_Financial_Model.ipynb)

This repository contains a Python-based financial feasibility model developed to assess the financial sustainability and scale-up potential of the **Magna Clean Cooking Project**.

The model supports Phase II of the project by translating key operational and financial assumptions into projected unit economics, break-even requirements, investment recovery, cash flow, and sensitivity analyses.

**Prepared by:** Christian Yesashimwe  
**Project:** Magna Clean Cooking Project  
**Model status:** Working / Preliminary Model  
**Last updated:** July 2026

---

## 1. Project Overview

The Magna Clean Cooking Project is piloting a battery-powered electric cooking service designed to provide households with access to modern electric cooking without requiring them to purchase the full cooking and energy system upfront.

The service combines:

- Electric cookstoves
- Rechargeable battery storage
- Battery charging and swapping operations
- An Energy-as-a-Service delivery model

Following the initial technology and operational pilot, **Phase II** focuses on testing the service at a larger household scale and generating evidence on its operational and financial feasibility.

---

## 2. Purpose of the Model

The model is an internal decision-support and financial planning tool built around the following foundational question:

> **Can Magna deliver reliable battery-powered electric cooking at a price households are willing and able to pay, while generating sufficient cash flow to recover investment, sustain operations, and scale the service?**

The model is designed to help answer:

1. What is the cost and revenue associated with serving each household?
2. At what household scale can the project cover its operating costs?
3. How much upfront investment is required at different deployment scales?
4. How long does it take to recover the initial investment?
5. How do alternative battery strategies affect financial viability?
6. Which assumptions have the greatest influence on financial performance?
7. What operational and financial variables need to be validated during Phase II?

---

## 3. Scenarios Evaluated

### Scenario A — Battery-as-a-Service (BaaS)

Under this scenario, battery technology is outsourced to a local battery provider.

The project pays for battery capacity based on the amount of available storage provided to households.

Key working assumption:

- Battery service cost: **USD 2/kWh/month of available storage**
- Indicative allocated storage: **5 kWh per enrolled household**

The model evaluates the recurring battery-service cost alongside electricity, maintenance, field operations, payment-processing costs, fixed operating expenses, and customer revenues.

### Scenario B — Battery Ownership

Under this scenario, the project purchases and owns the battery assets and cookstoves.

Current working assumptions include:

- Battery purchase cost: **USD 300 per household**
- Cookstove purchase cost: **USD 60 per household**
- Equipment CAPEX: **USD 360 per household**
- Customer payment assumption: **USD 11 per household/month**
- Preliminary project operating-cost assumption: **USD 1,300/month**
- Investment analysis horizon: **60 months / 5 years**

This scenario evaluates upfront capital requirements, monthly cash generation, operating break-even, investment recovery, and payback at different household scales.

---

## 4. Model Structure

The model includes:

### Inputs and Assumptions
Centralized operational and financial assumptions that can be modified as new project data become available.

### Deployment Modeling
Household enrollment, activity rates, churn, and deployment growth over time.

### Revenue Modeling
Revenue generated from household usage and service payments.

### Energy Economics
Electricity consumption, charging losses, energy tariffs, and related charging costs.

### Battery Economics
Comparison of recurring Battery-as-a-Service costs with direct battery ownership.

### Operating Costs
Fixed and variable operating expenses, including staffing, transport, maintenance, monitoring, administration, and field operations.

### Carbon Revenue
Optional carbon-finance assumptions are modeled separately so that the underlying business can be assessed both with and without carbon revenue.

### Financial Analysis
The model evaluates metrics including:

- Revenue
- Operating costs
- Contribution margin
- Operating profit
- Break-even household scale
- Capital requirements
- Investment recovery
- Payback period
- Net Present Value (NPV)
- Sensitivity to key assumptions

---

## 5. Sensitivity Analysis

The model tests how financial outcomes change when key assumptions vary.

Variables evaluated include or may include:

- Number of households served
- Customer pricing
- Household activity/utilization
- Charging frequency
- Battery cost
- Battery ownership versus BaaS
- Electricity consumption
- Electricity tariff
- Operating costs
- Exchange rate
- Carbon revenue assumptions

Sensitivity analysis is intended to identify the variables that have the greatest influence on financial viability and therefore require the strongest validation during Phase II.

---

## 6. Preliminary Outputs

Under the current simplified battery-ownership assumptions, the model estimates:

| Metric | Preliminary Result |
|---|---:|
| Equipment CAPEX | USD 360/household |
| Monthly operating break-even | ~119 households |
| 5-year investment-recovery break-even | ~260 households |
| Investment horizon | 60 months |

These figures are **illustrative outputs based on current assumptions and should not be interpreted as final commercial break-even thresholds**.

In particular, the simplified ownership scenario currently assumes a project-level monthly operating cost of USD 1,300. Phase II will help determine how operating costs actually change with household scale, energy consumption, charging requirements, staffing, logistics, maintenance, and service infrastructure.

---

## 7. Key Phase II Questions to Validate

Phase II will be used to replace assumptions with observed project data, particularly around:

- Actual household electricity consumption
- Energy consumed per meal
- Cooking frequency and usage patterns
- Household willingness and ability to pay
- Payment consistency and customer retention
- Battery utilization and required storage capacity
- Battery-to-household ratio
- Charging frequency and charging-station capacity
- Electricity and charging costs
- Battery degradation, failures, replacement, and useful life
- Cookstove maintenance and replacement costs
- Fixed versus variable operating costs
- Staffing and logistics requirements at larger scale
- Potential carbon-credit revenues and associated MRV costs

These data will progressively improve the reliability of the financial model.

---

## 8. How to Use This Model

1. Open the notebook in **Google Colab**.
2. Review the assumptions in the **Inputs / Configuration** section.
3. Update assumptions where necessary using the latest project or Phase II data.
4. Select:

   `Runtime → Run all`

5. Review the generated:
   - Monthly financial projections
   - Unit economics
   - Break-even analysis
   - Investment-recovery analysis
   - Sensitivity tables
   - Financial charts and visualizations

The model should be updated progressively as actual Phase II operational and financial data become available.

---

## 9. Open in Google Colab

The model can be viewed and run directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_OR_GITHUB_COLAB_LINK_HERE)

Replace `YOUR_COLAB_OR_GITHUB_COLAB_LINK_HERE` with the direct Colab link to the notebook.

For a notebook hosted in this GitHub repository, the link normally follows this structure:

`https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPOSITORY/blob/main/YOUR_NOTEBOOK.ipynb`

---

## 10. Model Development Approach

This is a **driver-based financial model with scenario and sensitivity analysis**.

Rather than relying primarily on historical financial statements, the model links physical and operational project drivers — such as households served, energy consumption, battery capacity, customer payments, charging frequency, and operating costs — to financial outcomes.

The model is intended to evolve through the following process:

**Initial assumptions → Phase II pilot data → validated unit economics → break-even analysis → scale-up financial model**

---

## 11. Important Limitations

This model is currently a **working financial feasibility model**, not an audited financial forecast or investment recommendation.

Current outputs depend on assumptions that are still being tested.

In addition:

- The BaaS and ownership scenarios should ultimately be evaluated using a common analysis horizon, deployment trajectory, customer base, revenue assumptions, and operating-cost structure before making a definitive comparison.
- Some operating costs may increase non-linearly as the project scales.
- Equipment replacement, battery degradation, infrastructure expansion, financing costs, taxes, and working-capital requirements may require further modeling.
- Carbon revenues remain uncertain and should not be treated as essential to core business viability until eligibility, methodology, verification costs, issuance timelines, and realized revenues are validated.

Results should therefore be interpreted as **scenario-based estimates for decision support**.

---

## 12. Repository Contents

The repository may include:

```text
magna-clean-cooking-financial-model/
│
├── README.md
│
├── Magna_Phase_II_Financial_Feasibility_Model.ipynb
│
├── outputs/
│   ├── Financial_Feasibility_Preliminary_Results.pdf
│   └── sensitivity_results.csv
│
└── docs/
    └── methodology_notes.md
