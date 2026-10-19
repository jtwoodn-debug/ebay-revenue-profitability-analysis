# ebay-revenue-profitability-analysis

## 📋 Executive Summary
Standard e-commerce reporting often overstates profitability by excluding seller-absorbed fulfillment costs. This project normalizes 2 years of raw transactional data to quantify true net margins, identify revenue leakage from returns, and uncover operational inefficiencies across Australian markets.

**Key Impact:** Revealed **5.76 percentage point margin erosion** hidden in "Free Postage" orders and delivered actionable recommendations for shipping threshold optimization and inventory staging.

## 🎯 Business Objectives
- Quantify the impact of out-of-pocket shipping costs on "Free Postage" orders
- Measure annual refund rates and gross revenue leakage from returns
- Identify regional profitability concentration and fulfillment density opportunities
- Evaluate seasonal revenue patterns against operational listing cadence

## 🛠️ Technical Approach
| Component | Technology | Purpose |
|-----------|------------|---------|
| Data Warehouse | Google BigQuery | Scalable SQL processing & storage |
| Transformation | SQL (CTEs, Window Functions) | Cost normalization & metric derivation |
| Data Modeling | Star Schema (fct/dim) | Optimized query performance |
| Visualization | Power BI | Interactive stakeholder dashboards |
| Version Control | GitHub | Reproducibility & documentation |

## 📊 Key Findings & Recommendations

### 1. True Margin Visibility
> **Finding:** 43.5% of orders absorbed $4,080 AUD in unrecorded shipping costs, eroding reported net profit by 5.76pp.
>
> **Recommendation:** Implement a $60 AUD free-postage threshold or migrate low-margin SKUs to buyer-paid flat-rate shipping.

### 2. Return Rate Benchmarking
> **Finding:** 3.97% return frequency ($2,385 AUD leakage) confirms strong listing accuracy but identifies item-level QA opportunities.
>
> **Recommendation:** Institute quarterly defect reviews on returned SKUs; update imagery and condition descriptions to sustain <3.5% return rate.

### 3. Regional Fulfillment Density
> **Finding:** VIC/NSW/QLD account for 74.78% of volume and 71.97% of revenue, indicating East Coast fulfillment concentration.
>
> **Recommendation:** Stage high-velocity inventory near Melbourne/Sydney hubs to reduce transit time and postage costs.

### 4. Operational Cadence Context
> **Note:** Revenue fluctuations correlate with listing velocity rather than pure seasonality. eBay's algorithm rewards consistent daily uploads. Future iterations should incorporate listing logs to isolate platform-driven vs. market-driven variance.

## 🔗 Project Assets
- [📂 SQL Queries](./queries/)
- [📸 Dashboard Screenshots](./visuals/)
- [📄 Raw Data Sample](./data/)
- [📊 Power BI File](./dashboard.pbix)

---
*Built as an independent analytical project demonstrating end-to-end data modeling, cost normalization, and business recommendation delivery.*
