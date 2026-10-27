## Project roadmap

This roadmap organizes the investigation without choosing your tools. Record your decisions and preserve a sequence that another person can reproduce. Submit `final_project_firstname_lastname.ipynb`, preferably as one notebook, keeping relative paths to `data/ch16`. In a class, the instructor sets the deadline. For independent study, attempt the project before consulting the solution. Run **Restart Kernel and Run All** before finishing.

### 1. Understanding the data

**Guidance.** Understand each table before analyzing results.

**Hint.** What does a row represent? What period is covered? Which variables identify records? Which tables complement one another? Which units of observation differ?

**Caution.** Two tables having a column with the same name does not automatically justify joining them in that way.

### 2. Quality

**Guidance.** Investigate problems that could change the results.

**Hint.** Are there repeated records, missing values, semantically identical categories with different spellings, violations of documented rules, or unusual observations?

**Caution.** Do not change the data before understanding the problem. An extreme observation is not necessarily an error.

### 3. Cleaning

**Guidance.** Document each important decision: problem, decision, justification, and possible information loss or change.

**Hint.** Is the decision necessary for every measure or only part of the analysis? Is there a defensible alternative?

**Caution.** There is no universal rule for treating missing values.

### 4. Integration

**Guidance.** Construct coherent analytical data and validate every join.

**Hint.** What is the correct key? What is the cardinality? Should the number of rows change? Do costs vary only by product, or also over time? Do targets belong to transactions or branch × month?

**Caution.** A merge can run without errors and still produce substantively incorrect data.

### 5. Indicators

**Guidance.** Construct measures that answer the business questions.

**Hint.** Consider activity, revenue, costs, margin, volume, average order value, targets, and change over time. Identify the numerator, denominator, and unit of every ratio.

**Caution.** A larger absolute value does not necessarily mean better performance.

### 6. Branches and regions

**Guidance.** Compare units and state the question each measure answers.

**Hint.** Do regions contain the same number of branches? Were all branches active for the same period? Do cumulative totals and average performance answer the same question?

**Caution.** Total comparisons may reflect scale and time exposure.

### 7. Products and categories

**Guidance.** Investigate the portfolio along more than one dimension.

**Hint.** Does the quantity leader also lead in revenue? Does higher revenue necessarily imply a higher margin? Does sales composition matter?

**Caution.** The “best product” depends on the indicator.

### 8. Time

**Guidance.** Analyze activity over the observed period.

**Hint.** Are some months more active? Does activity change between 2024 and 2025? Is a recurring pattern visible?

**Caution.** Describing a trend does not predict the future.

### 9. Targets

**Guidance.** Assess performance against targets and state the denominator.

**Hint.** Meeting a target in one month differs from doing so consistently. Attainment frequency and the actual-to-target ratio answer different questions. How should pre-opening periods be treated?

**Caution.** Structural missingness is not necessarily an error.

### 10. Observations that warrant investigation

**Guidance.** Identify unusual observations before deciding to retain or remove them.

**Hint.** Do they violate rules? Are their keys valid? Could they represent legitimate business events? What is their impact?

**Caution.** Extreme does not mean erroneous.

### 11. Visualizations

**Guidance.** Produce three to five nonredundant visualizations.

**Hint.** For each chart, record the question, visual choice, evidence, interpretation, and limitation. Choose the chart based on the question.

**Caution.** A technically correct chart can be inappropriate for the question or encourage an exaggerated interpretation.

### 12. Conclusions, recommendations, and limitations

**Guidance.** Present five executive conclusions and two to four recommendations. Each conclusion should follow evidence → interpretation → managerial implication.

**Hint.** Separate what the data show from the action proposed. Include a limitations section addressing synthetic data, descriptive scope, cleaning decisions, coverage, absence of causal identification, and absence of forecasting.

**Caution.** Descriptive association does not demonstrate causality, and an unsupported recommendation is not an analytical conclusion.

### Pre-submission checklist

- [ ] Units of observation have been identified.
- [ ] Cleaning decisions have been justified.
- [ ] Cardinalities have been checked.
- [ ] Numerators, denominators, and units have been stated.
- [ ] Coverage differences have been considered.
- [ ] Unusual observations have been investigated.
- [ ] Charts answer explicit questions.
- [ ] There are five conclusions and two to four recommendations.
- [ ] Limitations are recorded.
- [ ] The notebook runs from beginning to end in a clean kernel.
