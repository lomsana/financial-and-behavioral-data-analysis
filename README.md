# financial-and-behavioral-data-analysis
Exploratory data analysis examining financial and behavioral interaction data to identify early indicators of financial distress using indicator-based classification and visualization.

## Research Question
Can customers showing early signs of financial distress be identified using daily customer interaction data?

## Data Source & Structure
- **Data:** Daily customer interaction records (descriptive text fields)
- **Key fields:** Des1, Des2, Des3 (interaction descriptions)
- **Reference tables:** Financial Stress Indicators; Behavioral Stress Indicators
- **Note on privacy:** This repository does not include sensitive/raw customer data.

## Methods
1. Separated descriptive fields into three working tables (Des1, Des2, Des3).
2. Built/used indicator lists for **financial** and **behavioral** stress categories.
3. Used **Power Query merges (joins)** to match descriptions to indicator keys.
4. Created binary match variables (1 = matched indicator; 0 = no match).
5. Appended results across Des1–Des3 and removed duplicates.
6. Produced frequency visualizations and a heatmap of category intersections.

## Key Findings
- Liquidity risk was the most frequent financial stress category.
- Anxiety and card-related behaviors were the most common behavioral stress indicators.
- High-frequency intersections (e.g., liquidity risk + anxiety) suggest behavioral cues can function as early warning signals when paired with financial stress indicators.

## Value to the Organization
This approach demonstrates how interaction data can support early risk detection and proactive outreach (e.g., targeted alerts, financial education, or support) to reduce escalation and improve customer experience.

## Figures
### Financial Stress Frequency
![Financial stress frequency](docs/figures/financial_stress_frequency.png)

### Behavioral Stress Frequency
![Behavioral stress frequency](docs/figures/behavior_stress_frequency.png)

### Financial × Behavioral Stress Heatmap
![Heatmap](docs/figures/stress_heatmap.png)

## Tools & Skills

**Tools:** Microsoft Excel, Power Query  
**Methods & Skills:** Data cleaning and preprocessing, indicator-based classification, exploratory data analysis, data deduplication and validation, frequency and intersection analysis, research documentation

**Research Practices:** Reproducible workflows, data integrity, ethical handling of sensitive data

