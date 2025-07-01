# Bitcoin Sentiment — Analysis Report

## Objective
The goal of this assignment was to explore the relationship between **Bitcoin market sentiment** and **trader performance**, leveraging historical trade data and the Fear & Greed Index.

---

## Datasets Used

1. **Fear & Greed Index**
   - Columns: `date`, `value`, `classification`
   - Represents daily market sentiment

2. **Historical Trader Data (Hyperliquid)**
   - Includes: `Account`, `Coin`, `Execution Price`, `Size`, `Side`, `Closed PnL`, `Timestamp`, etc.
   - Captures individual trade performance

---

## Methodology

1. **Preprocessing:**
   - Parsed and formatted date columns
   - Cleaned and checked for nulls

2. **Merging:**
   - Merged both datasets on the `date` column

3. **Exploratory Analysis:**
   - Grouped data by `classification` and calculated **average Closed PnL**
   - Created bar charts to visualize average performance under different sentiment states

4. **Correlation Analysis:**
   - Converted `value` column to numeric
   - Created scatter plots to visualize correlation between sentiment score and PnL

---

## Key Findings

- **Extreme Greed** sentiment days had the highest average trader profits
- **Extreme Fear** was associated with low or negative PnL
- Moderate correlation observed between higher sentiment scores and trader profitability
- Some volatility even during "Greed" phases — further filtering by position side/coin could help

---

## ⚠Challenges

- Date alignment between both datasets (some dates missing in one of them)
- Sparse data during certain sentiment classifications (e.g., Extreme Fear)
- No labels or ground truth for trader strategy types

---

## Possible Extensions (Given More Time)

- Analyze impact by **trade direction** (Long vs Short)
- Include **coin symbol** to track performance by asset
- Build simple strategy simulator based on sentiment conditions

---

## Conclusion

The Fear & Greed Index can serve as a valuable **contextual indicator** for anticipating average trader performance. This exploratory analysis demonstrates a pattern where traders tend to perform better in high-sentiment (greed) environments.

---
