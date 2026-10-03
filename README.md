# Sales Performance Dashboard 2024–2025 | Andes Retail Group

Interactive Power BI dashboard that analyzes the commercial performance of **Andes Retail Group** (Peru, Chile and Colombia) across 2024 and 2025, explains why revenue declined, and turns the findings into actionable recommendations using the **SCQA** storytelling framework.

## Business Question

How did total revenue evolve between 2024 and 2025, and **why did it change**? Is the decline widespread or concentrated in specific areas of the business?

## Dashboard Structure

### View 1: Executive Overview
Answers: *How has total revenue evolved between 2024 and 2025?*

- **KPIs:** Revenue 2024, Revenue 2025, Revenue Variation %, Profit Margin %
- **Line chart:** monthly revenue, 2024 vs 2025
- **Horizontal bar chart:** revenue by country
- **Column chart:** revenue by product category
- **Donut chart:** cost vs. profit
- **Slicers:** Year, Country

### View 2: Detailed Analysis
Answers: *Why did revenue fall, rise, or stay flat?*

- **Column chart:** revenue by season, 2024 vs 2025
- **Bar chart:** revenue by customer segment, 2024 vs 2025
- **Clustered column chart:** revenue by region, 2024 vs 2025
- **Table:** product category and sales level, sorted by revenue variation %
- **Slicers:** Year, Region

## Data Preparation

- Converted `Fecha_Pedido` to Latin American Spanish date format
- Fixed data types of numeric columns
- Created a conditional column `Nivel_Venta`: **High Sale** if `Ingresos` ≥ 1,000, otherwise **Low Sale**
- Validated data quality with Column Profile view

> Column names and category values are in Spanish, as in the original dataset.

## Key Findings

| Metric | Result |
|---|---|
| Revenue 2024 | $2.86M |
| Revenue 2025 | $2.67M (**-6.8%**) |
| Profit margin | 35.1% |
| Top markets | Peru ($2.2M), Chile ($2.0M), Colombia ($1.3M) |

**The decline is not widespread. It is concentrated in specific areas:**

- **Seasonality:** Summer generated $1.22M in 2024 (down to $1.02M in 2025) versus only $0.33M in Winter.
- **Region:** South had the biggest drop ($0.95M → $0.83M), while North stayed nearly flat ($0.94M → $0.95M).
- **Customer segment:** Premium fell the most ($1.40M → $1.20M), Standard held steady, and Economy slightly grew ($0.24M → $0.26M).
- **Product category:** High-sale Electronics had the worst decline (-15.5%), followed by high-sale Clothing (-12.2%).

## Recommendations

1. Run commercial campaigns during the low season (Winter) to smooth out seasonality.
2. Investigate the drop in the South region and the Premium segment (possible customer loss to competitors or a change in buying habits).
3. Review the product mix and pricing in Electronics and Clothing, the categories with the largest deterioration.

## Data Storytelling (SCQA)

- **Situation:** Andes Retail Group generated $2.86M in 2024 with a healthy 35.1% profit margin.
- **Complication:** Revenue fell 6.8% in 2025, with 2025 below 2024 in most months.
- **Question:** Is the decline widespread, or concentrated in specific areas?
- **Answer:** It is concentrated in the South region, the Premium segment, high-sale Electronics and Clothing, and the low season.

## Tools

Power BI Desktop · DAX · Data modeling · Data storytelling (SCQA)

## Files

- `<your-file-name>.pbix`: Power BI dashboard file.
- `sprint_10_-_cuaderno_de_jupyter_-_S10_Proyecto_VersionEstudiante_Desempeno_Comercial.ipynb`: project notebook with the dashboard planning, SCQA narrative and Slack executive message.
- `images/`: screenshots of both dashboard views.

- [Download the Power BI dashboard (.pbix) from Google Drive](https://drive.google.com/file/d/1Njc6DYqpcMevuBx9iYa5599R6ccFPdPl/view?usp=drive_link)

- [Download the dashboard from Google Drive](https://drive.google.com/file/d/1fWGqsy11tkoJsZmFEVJFcm0AugrWJcDz/view?usp=sharing)

## Author

**Dante Mota**: [GitHub](https://github.com/dantemota12)
