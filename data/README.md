# Dataset notes

The source folder contains eight CSV files used alongside the retail dashboard project. Their provenance, license, and whether the records are synthetic or operational are not documented. The files are therefore described here but are not redistributed in this repository.

`Customer_Demographics.csv` contains customer IDs linked to age, gender, income bracket, purchase frequency, and average spend. Because that is customer-level demographic and spending information and its provenance is unknown, the raw files are withheld from the public repository. The customer-detail table is also obscured in the published screenshot preview; aggregate visuals remain visible.

## Source files and observed row counts

Counts below are from the supplied CSV files. They describe the source files as inspected, not a claim about a live or complete retail operation.

| Source file | Rows | Purpose based on columns |
|---|---:|---|
| `Sales_Data.csv` | 219 | Dated sales rows with site, product, units, revenue, discounts, returns, and customer IDs. |
| `Product_Information.csv` | 100 | Product names, category, subcategory, unit cost/price, supplier, and shelf life. |
| `Site_Details.csv` | 50 | Site names, format, region, city, state, size, open date, and status. |
| `Customer_Demographics.csv` | 50 | Customer age, gender, income bracket, purchase frequency, and average spend. |
| `Inventory_Data.csv` | 100 | Beginning/ending inventory, replenishment, and stockout flag by site/product. |
| `Logistics_Data.csv` | 150 | Shipment dates, quantities, delivery status, and transport type by site/product. |
| `Promotions_and_Discounts.csv` | 50 | Promotion dates, discount type/amount, product, and site. |
| `Monthly_Seasonal_Planning.csv` | 120 | Forecast and actual sales with seasonal adjustment by month, site, and category. |

The sales rows span 2 April 2024 through 14 May 2025. They include 50 customer IDs, 78 product IDs, and 49 site IDs; all IDs observed in sales match an ID in the corresponding supplied dimension file. The 50-site dimension therefore has one site with no matching sales row in this sales extract.

The source uses example-like labels such as `Yogurt Item 45` and `Supplier 1`, and patterned IDs. Those labels suggest sample data but do not establish the dataset's provenance or sharing rights. No currency is specified in the files.

See [the data dictionary](../documentation/data-dictionary.md) for the observed columns. The original CSVs remain in the user's source folder and were not modified.
