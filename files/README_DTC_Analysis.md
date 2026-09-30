# 📊 DTC Campaign Overview Dashboard

> An Excel dashboard that tracks manning, volume, value and cash reconciliation for a multi-region Direct-to-Consumer (DTC) sales campaign across Nigeria, covering **11 August to 4 September 2026**.

---

## 🎯 Project Overview

A consumer brand ran a DTC campaign in which brand ambassadors (BAs) sold a 120g evaporated milk product directly to shoppers. Teams worked across **14 locations in 3 regions (East 1, East 2, West 2)**, with 12 BAs per location.

I built an overview dashboard that condenses the whole campaign into one page:

- **Headline KPI cards** for active teams, volume and value
- **A location-by-location performance table** (manning, reach, conversion, volume, cash and value)
- **A regional roll-up** of the same metrics
- **A team performance chart** comparing target and actual volume for each location

## 🖼️ Dashboard Preview

**Headline KPIs**

![Dashboard KPIs](images/kpi_summary.png)

**Team performance: target vs. actual volume by location**

![Team performance chart](images/team_performance.png)

## ❓ Business Questions Answered

1. Are all planned teams active and fully manned?
2. How much of the volume and value target has been achieved to date?
3. Which locations and regions are ahead, and which are lagging?
4. Is the cash collected in line with what was expected?
5. How does actual conversion compare with the conversion target?

## 🧮 Dashboard Assumptions

| Parameter | Value |
|---|---|
| Daily sales target per BA | 21 cases |
| Consumer reach target per BA per day | 70 shoppers |
| Implied conversion target | 30% (21 of 70) |
| BAs per location | 12 |
| Price per case (value ÷ volume) | ₦2,000 |

## 🗂️ Dashboard Structure

| Section | What it shows |
|---|---|
| **Headline KPIs** | Active teams, volume (cases) and value (₦), each as target, actual and % achieved |
| **Location table** | Region, location, commencement date, promoter manning, man-days, work-days, reach, conversion, strike rate, volume, cash reconciliation and value |
| **Regional summary** | The same metrics rolled up to East 1, East 2 and West 2, with a grand total |
| **Team performance chart** | Clustered columns of target vs. actual volume and % achieved per location |

## 🔍 Key Findings

### Headline results

| KPI | Target | Actual | % Achieved |
|---|---|---|---|
| Active teams | 168 | 168 | **100%** |
| Volume (cases) | 37,548 | 23,115 | **61.6%** |
| Value | ₦75,096,000 | ₦43,923,814 | **58.5%** |

All 168 planned promoters were in the field, yet the campaign delivered about **three-fifths of its volume target**.

### Regional performance

| Region | Promoters | Volume target | Volume actual | % Volume | % Value |
|---|---|---|---|---|---|
| East 1 | 48 | 10,584 | 5,997 | 56.7% | 53.8% |
| East 2 | 60 | 12,852 | 7,712 | 60.0% | 56.9% |
| West 2 | 60 | 14,112 | 9,406 | **66.7%** | **63.4%** |

West 2 leads on both volume and value, and East 1 trails.

### Location performance (ranked by % of volume target)

| Location | Region | Target | Actual | % Achieved |
|---|---|---|---|---|
| Bayelsa | East 2 | 2,520 | 2,240 | 88.9% |
| Auchi | West 2 | 4,284 | 3,804 | 88.8% |
| Owerri | East 1 | 4,032 | 3,399 | 84.3% |
| Warri | West 2 | 3,276 | 2,550 | 77.8% |
| PHC 1 | East 2 | 3,528 | 2,337 | 66.2% |
| Onitsha | East 1 | 2,520 | 1,477 | 58.6% |
| Ado-Ekiti | West 2 | 3,024 | 1,686 | 55.8% |
| Uyo | East 2 | 3,528 | 1,756 | 49.8% |
| Calabar | East 2 | 3,024 | 1,326 | 43.8% |
| Akure | West 2 | 1,008 | 391 | 38.8% |
| Benin | West 2 | 2,520 | 975 | 38.7% |
| Asaba | East 1 | 2,268 | 674 | 29.7% |
| Enugu / Abakaliki | East 1 | 1,764 | 447 | 25.3% |
| Aba | East 2 | 252 | 53 | 21.0% |

### What the numbers say

- **Manning is not the problem.** Every location reports 100% manning, so the shortfall comes from productivity per BA, not headcount.
- **Average productivity is about 13 cases per BA per day against a target of 21** (23,115 cases ÷ 1,788 man-days).
- **Conversion is well below plan.** Actual sales equal roughly **18.5% of shoppers reached**, against a 30% conversion target.
- **Sales are concentrated.** The top three locations (Auchi, Owerri, Warri) delivered about **42% of total volume**.
- **A clear top tier exists.** Bayelsa, Auchi and Owerri each run at 84-89% of target, roughly 17.7-18.7 cases per BA per day, which shows the target is achievable.
- **A long tail underperforms.** Six locations sit below 40% of target, and Aba, Enugu/Abakaliki and Asaba are below 30%.
- **Cash collected is about 5% below expected** (₦43.92M paid vs. ₦46.23M expected, a ₦2.31M variance). The gap is similar at every location (roughly 4.5-5.6%), which points to a consistent deduction or margin and not isolated shortfalls.

## 💡 Insights and Recommendations

- **Focus on conversion, not headcount.** Coach BAs in the weakest locations on approach, product demonstration and market choice.
- **Replicate the best performers.** Compare Bayelsa, Auchi and Owerri against Asaba and Enugu/Abakaliki on market selection, timing and supervision.
- **Review very low performers.** Aba shows just one work day, and Akure four, so their percentages partly reflect a late start. Confirm before judging them against full-campaign targets.
- **Prioritise East 1.** It is the lowest-performing region and holds three of the four weakest locations.
- **Confirm the cash variance.** Document what the ~5% gap represents so that it can be reported separately from genuine shortfalls.

## ⚠️ Data Quality Notes

Auditing the dashboard turned up several items worth fixing before it is shared widely:

- The **regional "Reach %Ach" and "Strike Rate" columns show values of 4-5 and 198-300%**, which look like formula errors. The grand total row (61.6%) is correct.
- **"Reached Achieved" equals "Reached Target"** for every location, which suggests reach is calculated from man-days and not captured in the field. Actual reach counts would make the conversion analysis more reliable.
- **Chart data and table disagree slightly** for Enugu/Abakaliki (450 vs. 447 cases), giving a chart total of 23,118 against 23,115 in the table.
- **Akure's commencement date reads 13 June 2026**, which is before the campaign window and is likely a typo for August.

## 🛠️ Skills Demonstrated

- Executive KPI dashboard design in Excel (headline cards, tables and charts)
- Multi-level roll-ups: location → region → campaign total
- Target-vs-actual analysis for volume, value and cash
- Productivity and conversion analysis (cases per BA per day, strike rate)
- Data-quality auditing and critical reading of metrics
- Turning operational data into recommendations

## 🚀 Possible Next Steps

- [ ] Rebuild in **Power BI / Tableau** with date and region filters
- [ ] Add a daily trend line of volume vs. target across the campaign
- [ ] Capture real reach counts to measure true conversion
- [ ] Add cost-per-case and BA-level productivity analysis

## 📁 Repository Contents

```
├── CHI_DTC_Analysis_Report.xlsx   # Workbook (Overview Dashboard sheet)
├── README.md                      # This document
└── /images
    ├── kpi_summary.png            # Headline KPI cards
    └── team_performance.png       # Target vs. actual volume chart
```

> **Note:** Figures are shown as recorded in the dashboard. Individual names are not included.

---

*Built by [Your Name] · [LinkedIn](#) · [Email](#)*
