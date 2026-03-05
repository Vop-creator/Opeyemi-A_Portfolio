# Electronic Sales Performance

I analyzed an electronic sales dataset in Power BI by cleaning and modelling the data, creating a custom Date table and DAX time-intelligence measures to reveal sales trends, channel performance, and profitability insights that support better business decisions.


## ⚙️ Project Type 

- [x] Exploratory Data Analysis (EDA)
- [x] Dashboard / Data Visualization
- [x]  ETL
- [x] Data Cleaning/ Modelling
- [x] End-to-End (multiple of the above)


## Table of Contents
1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Repository Structure](#4-repository-structure)
5. [Data Workflow](#5-data-workflow)
7. [Analysis & Metrics](#8-analysis--metrics)
8. [Key Insights](#9-key-insights)
9. [Recommendations](#10-recommendations)
10. [Assumptions & Limitations](#11-assumptions--limitations)
11. [Future Enhancements](#12-future-enhancements)
12. [Deliverables](#13-deliverables)
13. [Author](#14-author)



## 1. Project Overview

An electronic retail company was generating large amounts of sales data across different channels, product categories, and regions, but did not have a clear way to analyze overall performance. The goal of this project was to understand sales trends over time, identify the most profitable sales channels and product categories, and determine which regions were driving business growth. To address this, the dataset was cleaned and transformed in Power BI using Power Query, and a data model with a custom Date table and time-intelligence measures was created using DAX. The results were presented in an interactive Power BI dashboard that highlighted key insights such as strong year-on-year sales growth, the dominance of the reseller channel, high-margin product categories, and regional performance differences that could guide future expansion.


## 2. Objectives

- Determine overall sales performance across channels, product categories, and regions using an interactive Power BI dashboard.
- Identify the top three product categories contributing the highest revenue and profit margins.
- Quantify sales growth trends over time using time-intelligence measures such as Year-over-Year and Month-over-Month comparisons.
- Evaluate regional sales performance to determine which regions contribute most to overall revenue.


## 3. Project Scope & Tools

### Scope

 - **In Scope**: "Sales transaction data including revenue, product categories, sales channels, and                   regional performance. Analysis focuses on identifying sales trends, top-                            performing categories, and regional contributions using Power BI visualizations"
 - **Out of Scope**: "Customer demographic information and marketing campaign data were excluded                         because the dataset only contains sales transactions, product categories,                           channels, and regions."
 - **Time Period**: Dec 2012 - Dec 2015
 - **Granularity**: Transaction-level sales records aggregated into monthly, category-level, and                         regional summaries for analysis.

### Tools & Technologies

 - Data Storage: [CSV files]
 - Data Processing: [Power Query]
 - Analysis | [Power BI]
 - Visualization: [Power BI]
 - Version Control: [ Git / GitHub]
 - Documentation: [Markdown]

## 4. Repository Structure

```
[project-root]/
│
├── data/
│   ├── raw/                  # Original, unmodified source data - never edited
│   ├── processed/            # Cleaned and transformed data
│   └── external/             # Reference data, lookup tables, third-party file
│
├── reports/                  # Final outputs: PDFs, slide decks, Word docs
│
├── visuals/                  # Exported charts, dashboard screenshots, ERD diagrams
│
├── project_metadata.yml      # Machine-readable metadata (optional)
└── README.md                 # You are here
```

## 5. Data Workflow

  1. Source: "Monthly CSV sales exports from the company."
  2. Extraction: "Imported CSV file into Power BI."
  3. Cleaning/Transformation: "Removed Duplicates.
                Fixed missing values.
                Standardized data types and date formats in the datasets.
                Created Date table, Time intelligence measures."
  5. Modelling: Created a star-scheme realtionship beween the data
  6. Analysis: "Built dashboards to see trends, top channels, and profit margins."
  7. Output: "Summary report (PDF)

```
[Data Source(s)]
      ↓
[Extraction]
      ↓
[Cleaning & Transformation]
      ↓
[Analysis / Modelling / Querying]
      ↓
[Output / Visualisation / Reporting]
```


## 8. Analysis & Metrics

<!--
  Explain what you measured and how - before you share what you found.

  WHAT GOOD LOOKS LIKE:
  Metric: "Customer Return Rate"
  Definition: "Number of transactions flagged as returns divided by total
               transactions, calculated at product-category and regional grain."
  Why It Matters: "Return rate - not sales volume - was hypothesised to
                  explain regional revenue gaps. This metric tests that hypothesis."

  WHAT TO AVOID:
  ❌ Defining a metric only in code: SUM(returns) / COUNT(transaction_id)
     That's an implementation. Write the plain-language definition here.
     Both belong in your project - the definition in the README,
     the implementation in the code.
-->

### Analytical Approach

[Describe how you approached the analysis. Were you exploring patterns? Testing a hypothesis? Building and validating a pipeline? Be honest about your method - exploratory work is valid, just call it that.]

### Key Metrics Defined

| Metric | Plain-Language Definition | Why It Matters |
|--------|--------------------------|----------------|
| `[Metric 1]` | [What it measures, in one sentence] | [What decision or question it answers] |
| `[Metric 2]` | [What it measures, in one sentence] | [What decision or question it answers] |
| `[Metric 3]` | [What it measures, in one sentence] | [What decision or question it answers] |

### Methods Used

- [e.g., Descriptive statistics - distribution, central tendency, outlier detection]
- [e.g., Trend analysis across [time period]]
- [e.g., Segmentation / group comparison by [dimension]]
- [e.g., Correlation analysis between [variable A] and [variable B]]
- [e.g., SQL window functions for [specific aggregation]]
- [e.g., Custom aggregation or transformation logic in [tool]]

---

## 9. Key Insights

<!--
  Findings + implications. Not just what happened - what it means.

  WHAT GOOD LOOKS LIKE:
  ✅ "Return rates, not sales volume, explain Region A's underperformance.
      Region A's return rate on home goods was 34% - more than double the
      company average. Revenue was not lost at the point of sale; it was
      lost post-sale through refunds. This points to a fulfilment or
      product quality issue specific to that region, not a demand problem."

  WHAT TO AVOID:
  ❌ "Region A had lower revenue than other regions in Q4."
     (That's an observation. It describes what happened.
      An insight says what it means and where to look next.)

  Aim for 3–6 insights. Quality over quantity.
-->

**Insight 1: [Short descriptive headline]**
[What you found + what it suggests. One short paragraph.]

**Insight 2: [Short descriptive headline]**
[What you found + what it suggests.]

**Insight 3: [Short descriptive headline]**
[What you found + what it suggests.]

**Insight 4 (if applicable): [Short descriptive headline]**
[What you found + what it suggests.]

---

## 10. Recommendations

<!--
  Action-oriented. Addressed to a real audience.
  Tied explicitly to the insight that supports each one.

  WHAT GOOD LOOKS LIKE:
  Priority: High
  Recommendation: "Conduct a fulfilment audit for home goods deliveries
                   in Region A - specifically investigating whether returns
                   correlate with a particular warehouse, carrier, or SKU batch."
  Based On: Insight 1 - return rate anomaly in Region A
  Owner: Operations / Supply Chain team

  WHAT TO AVOID:
  ❌ "Improve the return rate."
     (Not actionable. Doesn't say who, how, or where to start.)
  ❌ "Further analysis is needed."
     (This is a placeholder, not a recommendation.)
-->

| Priority | Recommendation | Based On | Suggested Owner |
|----------|---------------|----------|-----------------|
| High | [Specific, actionable step] | [Insight it comes from] | [Who should act] |
| Medium | [Specific, actionable step] | [Insight it comes from] | [Who should act] |
| Low | [Exploratory or longer-term suggestion] | [Insight it comes from] | [Who should act] |

---

## 11. Assumptions & Limitations

<!--
  WHAT GOOD LOOKS LIKE:
  Assumption: "Transaction records were assumed to be complete for all five regions.
               No validation was performed against source system record counts."
  Limitation: "The analysis cannot distinguish between returns initiated by
               the customer vs. returns initiated by the business (e.g., recalls).
               If business-initiated returns are concentrated in Region A, the
               return rate finding may reflect a policy decision, not a quality issue."

  WHAT TO AVOID:
  ❌ Leaving this section blank or writing "None known."
     Every project has limitations. Documenting them is a sign of
     analytical maturity - not a confession of failure.
-->

### Assumptions
- [What did you treat as true without being able to verify?]
- [What simplifications did you make for scope or feasibility?]
- [What domain rules or definitions did you accept as given?]

### Limitations
- [What gaps exist in the data?]
- [What analysis was out of scope but could affect interpretation?]
- [What would a more rigorous version of this project include?]
- [Are there known biases in the data source or collection method?]

> *The goal here is pre-emptive Q&A. What would a thoughtful skeptic push back on? Document the answer here, before they ask.*

---

## 12. Future Enhancements

<!--
  WHAT GOOD LOOKS LIKE:
  ✅ "Automate the monthly data pull from the POS export folder using
      a scheduled Python script, replacing the current manual process."
  ✅ "Expand the return rate analysis to include carrier-level data,
      which was unavailable in this dataset but exists in the logistics system."

  WHAT TO AVOID:
  ❌ "Add a machine learning model."
     (Vague, and disconnected from the actual findings of this project.)
  ❌ Listing aspirational features that don't follow logically from the work.
-->

- [ ] [Enhancement 1 - specific and traceable to a real gap in this project]
- [ ] [Enhancement 2]
- [ ] [Enhancement 3]
- [ ] [Enhancement 4]

---

## 13. Deliverables

| Deliverable | Description | Location |
|-------------|-------------|----------|
| [Name] | [What it contains] | [`/path/to/file`] |
| [Name] | [What it contains] | [`/path/to/file`] |
| [Name] | [What it contains] | [`/path/to/file`] |

---

## 14. Author

**[Your Name]**
[Your role or title - current or target]

- 🔗 [LinkedIn URL]
- 💼 [Portfolio or GitHub profile URL]
- 📧 [Email - optional]

---

*Last updated: [Month YYYY]*
*If this template helped you, consider starring the repository.*
