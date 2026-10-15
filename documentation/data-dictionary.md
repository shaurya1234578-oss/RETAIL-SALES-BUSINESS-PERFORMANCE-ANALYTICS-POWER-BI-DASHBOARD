# Data dictionary

This dictionary records the column names and apparent meaning of fields in the supplied CSV headers. It does not assert data types, model relationships, or business definitions beyond what the source names support. The raw CSVs are not included because provenance and sharing rights are undocumented and one table links customer IDs to demographic and spending attributes.

| File / table | Columns | Notes |
|---|---|---|
| `Sales_Data.csv` | `Date`, `Site ID`, `Product ID`, `Units Sold`, `Revenue`, `Discounts`, `Returns`, `Customer ID` | Sales fact-like rows. Dates are recorded as day-month-year in the sample. Currency and the business meaning of `Returns` are unspecified. |
| `Product_Information.csv` | `Product ID`, `Product Name`, `Category`, `Subcategory`, `Unit Cost`, `Unit Price`, `Supplier`, `Shelf Life` | Product attributes. Shelf-life unit is not specified in the header. |
| `Site_Details.csv` | `Site ID`, `Site Name`, `Site Format`, `Region`, `City`, `State`, `Store Size`, `Open Date`, `Status` | Site/location attributes. The meaning/unit for `Store Size` is unspecified. |
| `Customer_Demographics.csv` | `Customer ID`, `Age`, `Gender`, `Income Bracket`, `Purchase Frequency`, `Average Spend` | Customer-level demographic and spend attributes. Age units, income period/currency, purchase-frequency period, and average-spend calculation are unspecified. |
| `Inventory_Data.csv` | `Site ID`, `Product ID`, `Beginning Inventory`, `Ending Inventory`, `Replenishment`, `Stockout Flag` | Inventory snapshots or movements; period/grain and quantity units are unspecified. |
| `Logistics_Data.csv` | `Shipment ID`, `Site ID`, `Product ID`, `Shipment Date`, `Quantity`, `Delivery Status`, `Transportation Type` | Shipment records; quantity unit and status definitions are unspecified. |
| `Promotions_and_Discounts.csv` | `Promotion ID`, `Product ID`, `Site ID`, `Start Date`, `End Date`, `Discount Type`, `Discount Amount` | Promotion attributes; amount units and percentage-vs-value conventions are unspecified. |
| `Monthly_Seasonal_Planning.csv` | `Month`, `Site ID`, `Product Category`, `Forecasted Sales`, `Actual Sales`, `Seasonal Adjustments` | Planning values; currency, adjustment convention, and exact month grain are unspecified. |

## Report fields observed

The report definition references `Date_Table` fields `Year` and `Year Month`, as well as fields from `Sales_Data`, `Product_Information`, `Site_Details`, and `Customer_Demographics`. A standalone `Date_Table` CSV is not present. The available report definition does not provide enough evidence to document the complete relationship cardinalities or filter directions.
