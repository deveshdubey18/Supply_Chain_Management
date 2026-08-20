# 🚚 Supply Chain Management Dashboard (Power BI)

An interactive Power BI dashboard that analyzes warehouse-level supply chain data — covering warehouse capacity, staffing, distribution networks, refill requests, storage issues, and government certification — to help operations teams spot bottlenecks and monitor network health at a glance.

## 📊 Overview

The report is built on a dataset of **22,150 warehouses** and combines KPI summary cards, breakdown charts, and a decomposition tree with two supporting strategic-analysis pages (SWOT and Fishbone/root-cause diagrams) to frame the operational findings.

## 📁 Repository Structure

```
Supply_Chain_Management/
├── Dashboard/
│   └── SCM_dashboard.pbix     # Power BI Desktop report file
├── data/
│   └── SCM.csv                # Source dataset (22,150 warehouse records)
├── LICENSE                    # Apache-2.0
└── README.md
```

## 🗂️ Dataset

`data/SCM.csv` contains one row per warehouse with the following fields:

| Column | Description |
|---|---|
| `Ware_house_ID`, `WH_Manager_ID` | Unique warehouse and manager identifiers |
| `Location_type` | Urban / Rural |
| `WH_capacity_size` | Small / Mid / Large |
| `zone`, `WH_regional_zone` | Geographic zone (North, South, East, West) and regional sub-zone |
| `wh_owner_type` | Company Owned / Rented |
| `retail_shop_num`, `distributor_num` | Retail shops and distributors served |
| `num_refill_req_l3m` | Refill requests in the last 3 months |
| `transport_issue_l1y` | Transport issues in the last year |
| `Competitor_in_mkt` | Number of competitors in the market |
| `flood_impacted`, `flood_proof` | Flood risk and flood-proofing status |
| `electric_supply` | Whether the warehouse has electric supply |
| `dist_from_hub` | Distance from the distribution hub |
| `workers_num` | Number of workers |
| `wh_est_year` | Year the warehouse was established |
| `storage_issue_reported_l3m` | Storage issues reported in the last 3 months |
| `temp_reg_mach` | Temperature regulation machines on-site |
| `approved_wh_govt_certificate` | Government certification grade |
| `wh_breakdown_l3m` | Warehouse breakdowns in the last 3 months |
| `govt_check_l3m` | Government inspections in the last 3 months |
| `product_wg_ton` | Total product weight (tons) |

## 📈 Dashboard Pages

**1. Overview**

<img width="1100" height="620" alt="image" src="https://github.com/user-attachments/assets/b4f0edae-49b6-45cb-8fe2-5a263ad75314" />

##

**2. Methods**

<img width="1100" height="620" alt="image" src="https://github.com/user-attachments/assets/a26afbae-d7fb-4c14-aad5-257cc09de8bd" />

##

**3. SWOT** — Strengths, Weaknesses, Opportunities, and Threats summary for the supply chain network.

<img width="1100" height="620" alt="image" src="https://github.com/user-attachments/assets/9757c07f-fd2f-4da3-9724-1ba7746e70c5" />

##

**4. Fishbone** — Root-cause (Ishikawa) diagram breaking down the key drivers behind warehouse and supply chain issues.

<img width="1100" height="620" alt="image" src="https://github.com/user-attachments/assets/a9c9c0a4-f935-46ed-8414-fda7e3a0cdb5" />

##

## 🛠️ Tools & Technologies

- **Power BI Desktop** — data modeling, DAX measures, and report design
- **Power Query** — data cleaning and transformation
- Source data supplied as CSV

## 🚀 Getting Started

1. Install [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/desktop) (Windows only).
2. Clone or download this repository.
3. Open `Dashboard/SCM_dashboard.pbix` in Power BI Desktop.
4. If prompted, point the data source to `data/SCM.csv` in your local copy of the repo, then refresh.

## 📄 License

This project is licensed under the [Apache-2.0 License](LICENSE).
