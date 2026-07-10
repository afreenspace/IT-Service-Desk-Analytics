# IT Service Desk Findings

## Executive Summary

This analysis examined 97,498 IT support tickets from 2016–2020 to identify SLA compliance gaps, triage failures, and agent performance patterns.

Key conclusions:
- 29.76% of tickets never received a priority assignment, indicating a systemic intake or ticket creation process failure.
- 40.29% of tickets breached the SLA, with breach rates varying widely by category: 1% for Login Access, 41% for Software, and 66% for Hardware.
- Ticket volume doubled from 2016 to 2020, yet breach rates and triage gaps remained essentially unchanged, showing the process did not scale.
- Correlation between ticket volume and breach rate was only 0.14, suggesting workload volume was not the primary driver of breaches.
- Correlation between resolution time and satisfaction was -0.02, indicating that faster resolution alone did not translate to higher satisfaction.

## Detailed Findings

### 1. Triage and Priority Assignment

- Nearly 30% of tickets had no priority assigned.
- This gap was consistent across categories, suggesting the issue was not isolated to a single team or ticket type.
- Recommendation: enforce mandatory priority assignment at ticket intake or through automation rules.

### 2. SLA Breach Performance

- Overall breach rate: 40.29%.
- Category breakouts:
  - Login Access: 1%
  - Hardware: 66%
  - Software: 41%
  - System: 60%
- Recommendation: focus remediation on Hardware and System ticket workflows first, where breaches are highest.

### 3. Time Trends

- Ticket volume doubled from 2016 to 2020.
- SLA breach rate and triage gap stayed roughly flat.
- Recommendation: review process capacity and intake procedures, since growth was not matched by reliability improvements.

### 4. Agent Performance vs Workload

- Correlation between ticket count and breach rate: 0.14.
- This is effectively negligible and suggests that agent consistency matters more than sheer volume.
- Recommendation: measure and support individual quality, not just load balancing.

### 5. Resolution Speed vs Satisfaction

- Correlation between resolution time and satisfaction: -0.02.
- This indicates speed alone does not explain perceived service quality.
- Recommendation: investigate other factors such as communication quality, ticket ownership clarity, and outcome relevance.

## Business Recommendations

1. Implement mandatory triage and priority controls at ticket creation.
2. Use historical median resolution times plus buffer to define realistic SLA targets by priority tier.
3. Monitor high-breach categories separately and assign process improvement resources there.
4. Track agent consistency metrics, not only ticket volume.
5. Conduct a qualitative review of customer experience beyond resolution speed.

## Notes

- The workbook includes the full data model, formulas, and interactive dashboard used to produce these findings.
- The analysis was built in Microsoft Excel with Pivot Tables, slicers, and statistical formulas.
