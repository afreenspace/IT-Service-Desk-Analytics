# IT Service Desk Project Roadmap

## Objective

Build an analytics solution in Excel to evaluate SLA compliance, ticket triage quality, and agent performance for a service desk handling 97,498 tickets from 2016–2020.

## Project Steps

### 1. Data Ingestion and Cleaning

- Import the raw ticket dataset into Excel.
- Standardize category labels and fix typos.
- Identify and flag missing values, especially missing priority assignments.

### 2. SLA Logic and Target Definition

- Determine priority tiers from ticket data.
- Calculate median resolution time by priority tier.
- Define SLA thresholds using median resolution times plus a buffer.
- Apply SLA compliance logic to each ticket.

### 3. Statistical Validation

- Use Interquartile Range (IQR) to detect and understand outliers.
- Use Pearson correlation to test assumptions about workload, resolution time, and satisfaction.
- Validate that findings are supported by data rather than anecdote.

### 4. Dashboard Building

- Create Pivot Tables for key metrics such as breach rate, triage gap, and ticket volume.
- Add slicers for Year, Agent, and Priority to enable interactive analysis.
- Build a Master Dashboard sheet to summarize the most important insights.

### 5. Findings and Recommendations

- Document the main insights into an findings summary.
- Translate analytical results into business recommendations for process improvement.
- Focus on actionable outcomes such as mandatory triage, category-specific remediation, and agent quality metrics.

## Tools Used

- Microsoft Excel
- Pivot Tables
- Slicers
- Nested `IF`
- `COUNTIFS`, `AVERAGEIFS`
- `VLOOKUP`
- `MEDIAN` with conditional logic
- `QUARTILE` / IQR outlier detection
- `CORREL`
- Conditional formatting

## Outcome

A self-service Excel analytics workbook with an interactive dashboard and documented findings that allows stakeholders to explore SLA compliance and ticketing process quality over time.
