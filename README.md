# SWYNEX_Data_Cleaning_Preparation
# Car Sales Data

A synthetic dataset of **9,795 car sales transactions** across India, covering vehicle details, pricing, dealer information, customer data, and sale metadata. Useful for practicing data cleaning, exploratory data analysis (EDA), and building sales dashboards.

## Dataset Overview

| | |
|---|---|
| **File** | `Car_Sales_Data.csv` |
| **Rows** | 9,795 |
| **Columns** | 22 |
| **Format** | CSV |

## Column Description

| Column | Type | Description |
|---|---|---|
| `SaleID` | int | Unique identifier for each sale |
| `VIN` | string | Vehicle Identification Number |
| `Company Name` | string | Car manufacturer (e.g., Maruti Suzuki, Toyota, BMW) |
| `Model` | string | Car model name |
| `Year` | int | Manufacturing year of the vehicle |
| `Color` | string | Vehicle color |
| `FuelType` | string | Petrol / Diesel / Electric / CNG / Hybrid |
| `Transmission` | string | Manual / Automatic / CVT |
| `Price` | int | Sale price (in ₹) |
| `Mileage_km` | float | Mileage of the vehicle in km |
| `Mileage_provided` | string | Whether mileage data was provided (Yes/No) |
| `Dealer` | string | Dealership name |
| `State` | string | Indian state where the sale occurred |
| `Day` | float | Day of the sale date |
| `Month` | string | Month of the sale date |
| `Year.1` | float | Year of the sale date (separate from manufacturing year) |
| `Sale_Date_provided` | string | Whether the sale date was provided (Yes/No) |
| `CustomerName` | string | Name of the customer |
| `CustomerEmail` | string | Email address of the customer |
| `Customer_rating` | float | Customer satisfaction rating (1–10) |
| `Notes` | string | Additional remarks about the sale |
| `Finance` | string | Whether the purchase was financed (Yes/No) |

## Key Stats

- **Car manufacturers:** 12 (Audi, BMW, Ford, Honda, Hyundai, Kia, Mahindra & Mahindra, Maruti Suzuki, Mercedes-Benz, Tata Motors, Toyota, Volkswagen)
- **States covered:** 9
- **Manufacturing year range:** 1970 – 2025
- **Price range:** ₹3,53,400 – ₹66,98,700
- **Customer rating range:** 1.0 – 10.0

## Data Quality Notes

This dataset contains **intentional missing/placeholder values**, making it good practice material for data cleaning:

- Several columns use the literal string `"not provided"` instead of blanks (e.g., `FuelType`, `Transmission`, `Color`, `State`, `Finance`, `Notes`).
- `Mileage_km`, `Day`, `Month`, and `Year.1` have genuine blank (NaN) entries when the corresponding `_provided` flag is `"NO"`.
- `Notes` is mostly empty/`"not provided"` (~63% missing).
- Column name `Year.1` duplicates `Year` — the first is manufacturing year, the second is sale year (pandas auto-renamed it due to duplicate headers in the source file).

## Suggested Use Cases

- Data cleaning & preprocessing practice (handling `"not provided"` as missing data)
- Exploratory Data Analysis (sales trends by state, brand, fuel type)
- Building Excel/Power BI/Tableau dashboards
- Regression/price prediction modeling
## 🙋 Contact

Add your name/contact info here if you'd like others to reach out.
