# Business Questions, KPIs & Data Requirements

## Purpose

The purpose of this phase is to translate the identified business problems into measurable business questions, define relevant KPIs, and determine the data required for the analysis.

## Business Questions

1. Which suppliers have the highest and lowest on-time delivery performance?
2. How many deliveries arrive late?
3. How many deliveries arrive without defects or damage?
4. Which suppliers provide the best overall performance in terms of delivery time, quality, and cost?
5. At which stage of the supply chain do delivery delays occur – supplier preparation or logistics/transport?
6. How long does each stage of the order-to-delivery process take?

## Key Performance Indicators (KPIs)

- On-Time Delivery Rate (%)
- Late Delivery Rate (%)
- Average Delivery Delay
- Defect-Free Delivery Rate (%)
- Average Cost per Order / Unit
- Supplier Processing Time
- Transit Time
- Total Lead Time

## Data Requirements

| Category | Required Data |
|---|---|
| Order | Order ID, Order Date, Product ID / Product Name, Ordered Quantity |
| Supplier | Supplier ID, Supplier Name |
| Delivery | Promised Delivery Date, Supplier Dispatch Date, Actual Delivery Date |
| Quality | Quality Status, Damaged / Defective Quantity |
| Cost | Delivery Cost |

## Derived Measures

Some measures do not need to exist directly in the raw dataset because they can be calculated during the analysis.

**Delivery Status**
- Actual Delivery Date <= Promised Delivery Date → On Time
- Actual Delivery Date > Promised Delivery Date → Late

**Delivery Delay**
- Actual Delivery Date - Promised Delivery Date

**Supplier Processing Time**
- Supplier Dispatch Date - Order Date

**Transit Time**
- Actual Delivery Date - Supplier Dispatch Date

**Total Lead Time**
- Actual Delivery Date - Order Date

## Analysis Approach

The required data will be assessed for availability and quality before analysis begins. The available fields will determine which business questions and KPIs can be reliably evaluated.

No conclusions about supplier or logistics performance will be made until the data has been analysed.

## Project Status

**Phase 4 – Business Questions, KPIs & Data Requirements**

Business questions, KPIs, and required data fields have been defined.

Next step: Data Acquisition & Exploratory Data Analysis (EDA).
