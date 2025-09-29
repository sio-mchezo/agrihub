### Breakdown

*   **Product:** `Avocado`, `Coffee`, `Cashew` - Essential for filtering and sorting.
*   **Order_ID:** A unique identifier for each order (e.g., `AV-2024-001`).
*   **Customer_Name & Country_Destination:** For logistics and customer relationship management.
*   **Container_Type:** Critical for logistics. `Reefer` (refrigerated) for avocados, `Dry` for coffee and cashews.
*   **Quantity_MT:** Volume in Metric Tons, the standard unit for international trade.
*   **Unit_Price_FOB & Total_Value_FOB:** The price per metric ton and total value "Free On Board" at the shipping port. This is a standard Incoterm.
*   **Harvest_Date:** Crucial for perishable goods (avocado) and for establishing the crop year/origin for coffee and cashews.
*   **Origin_Region:** Adds traceability and value (e.g., "Michoacán" for avocado, "Huehuetenango" for coffee).
*   **Quality_Grade:** Product-specific classifications.
    *   **Avocado:** `Hass Extra`, `Hass I`
    *   **Coffee:** `SHB EP` (Strictly Hard Bean European Preparation), `Excelso UGQ` (Usual Good Quality)
    *   **Cashew:** `W320` (White Wholesale 320 pieces per pound)
*   **Specific_Attributes (Customs Column):** This is a flexible column for the detailed specs that define the product's quality and price. It's often the most important column for the buyer.
    *   **Avocado:** `Size` (count), `Dry Matter %`, `Brix` (sugar content).
    *   **Coffee:** `Variety`, `Process` (Washed/Natural), `Screen Size`, `Cupping Score`.
    *   **Cashew:** `Outturn` (bag size), `Count` (kernels per pound), `Moisture %`, `Defect %`.
*   **Shipping_Port, ETD, ETA:** Core logistics information.
*   **Status:** Tracks the order through the pipeline (`Booked`, `Processing`, `Shipped`, `In Transit`, `Delivered`).

### Use

1.  **Sales & Quoting:** The sales team uses the `Specific_Attributes` and `Unit_Price_FOB` from past orders to create accurate quotes for new customers.
2.  **Operations & Logistics:** The ops team filters by `Product` and `Status` to manage the supply chain—arranging `Reefer` containers for avocados and dry storage for the others.
3.  **Quality Control:** The QC team references the `Specific_Attributes` to ensure each shipment meets the contracted specifications before loading.
4.  **Finance & Accounting:** Uses `Total_Value_FOB` for invoicing and revenue tracking.
5.  **Reporting & Analysis:** Management can analyze profitability by product, customer, and region by sorting and pivoting this data.
