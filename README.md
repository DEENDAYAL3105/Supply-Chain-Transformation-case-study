# Supply Chain Transformation: AeroSports Inc.

> A consulting-style case study diagnosing the root causes of declining margins in a global sportswear supply chain, with short-term and long-term recommendations for the CEO.

---

## Overview

AeroSports Inc. is a global sportswear and athleisure brand headquartered in Amsterdam, with **€15B in revenue** but margins that are shrinking because of supply chain inefficiencies. This project analyses the company's supply chain data across **forecasting, inventory and logistics**, identifies where value is leaking, and proposes a phased transformation plan.

## Client Context

| Item | Details |
|---|---|
| Headquarters | Amsterdam |
| Products | Sports shoes, athleisure apparel, accessories |
| Sales channels | D2C, e-commerce, wholesale |
| Suppliers | 10 across Asia (China: 4, Vietnam: 5, Indonesia: 1) |
| Network | 3 global DCs (US, Europe, Singapore) + 15 regional warehouses |
| Revenue | €15B |

## Objectives

1. Map the current supply chain with key callouts
2. Evaluate forecast performance over the past year
3. Assess inventory management and its impact on working capital
4. Analyse logistics spend by region and shipment mode
5. Recommend improvements across demand, inventory and logistics, split into short-term and long-term horizons

## Approach

- Analysed the provided case dataset covering forecast units, sales units, opening/closing stock, receipts, and logistics costs by lane, region and mode
- Built interactive dashboards to compare forecast vs. sales at total, SKU and regional level
- Broke down inbound (Supplier → DC) and outbound (DC → Warehouse) logistics cost by country, region and air vs. ocean/non-air mode
- Synthesised findings into an executive presentation for the CEO

## Key Findings

### 1. Supply Chain Structure
- Multi-echelon network of 18 distribution facilities (3 DCs + 15 warehouses) adds coordination complexity, carrying cost and obsolescence risk
- Supplier base is concentrated in Asia, giving cost advantage but exposing the company to regional disruption
- One network must serve three very different fulfilment profiles: small-parcel e-commerce, case-level D2C replenishment, and pallet-level wholesale

### 2. Forecasting
- **Aggregate level:** forecast and actual sales are closely aligned and follow the same seasonality (3.05M units forecast vs. 3.05M units sold)
- **SKU level:** noticeable over- and under-forecasting in individual SKUs
- **Impact:** stock imbalances across regions, costly rebalancing shipments, longer fulfilment lead times, and obsolescence risk

### 3. Inventory
| Metric | Value |
|---|---|
| Sum of opening stock | 17.25M units |
| Sum of closing stock | 16.91M units |
| Sum of sales | 3.05M units |
| Sum of forecast | 3.05M units |
| Sum of receipts | 2.72M units |

- Opening and closing stock stay consistently high relative to sales across all regions (Asia, Europe, North America), indicating a push-based model and likely overstocking
- This ties up working capital and raises holding costs and markdown risk

### 4. Logistics
| Lane | Total cost |
|---|---|
| Supplier → DC (inbound) | €23.56M |
| DC → Warehouse (outbound) | €25.90M |

**Inbound (Supplier → DC)**
- About 86% of cost is ocean freight and 13–14% is air
- Vietnam (47%) and China (43%) drive about 90% of inbound spend, so consolidation and container-fill improvements on these lanes offer the biggest savings
- Receipts (2.72M) fell below forecast (3M) while spend stayed high, which points to under-utilised containers or air used for urgent replenishment

**Outbound (DC → Warehouse)**
- Air share of cost: **Asia ~20%, Europe ~22%, North America ~30%**
- Heavy air dependence, especially in North America and for short regional distances in Asia, suggests reactive planning rather than proactive buffers

## Recommendations

### Short term (0–12 months)
- **Enhance SKU-level forecasting:** segment SKUs and focus on those with the highest demand volatility
- **Align inventory to regional demand:** rebalance stock across warehouses using demand-driven allocation
- **Reduce reliance on air freight:** shift urgent shipments to sea/road through better planning buffers and lead-time visibility
- **Real-time operational dashboards:** track forecast variance, aging inventory, warehouse capacity and logistics mode mix

### Long term (1–3 years)
- **Demand sensing and predictive analytics:** use POS data, market signals, promotional calendars and regional trends
- **Digital control tower:** end-to-end visibility across inventory, logistics flows, supplier status and service levels
- **Lifecycle-based portfolio governance:** standardise product onboarding, scaling and phase-out to minimise obsolete inventory

## Tools Used

- Microsoft Excel (data preparation)
- Power BI (dashboards and visual analysis)
- PowerPoint / PDF (executive presentation)

## Repository Structure

```
├── README.md
├── Supply_Chain_Transformation_case_study.pdf   # Executive presentation
├── case_study_PS.pdf                            # Problem statement
└── data/                                        # Case dataset (add if shareable)
```

## Team

- Deendayal Suthar
- Soham Tanaji Raut
- Aditya Singh Shekhawat

## Disclaimer

This is an academic case study. AeroSports Inc. is a fictional company and all data is provided as part of the case brief.
