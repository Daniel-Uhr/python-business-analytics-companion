## Data dictionary

Oakridge Retail Group is a fictional multiregional retailer and distributor with five U.S. business regions and different product lines. These author-created data are synthetic and educational. The period is January 2024 through December 2025; some branches may have opened during the window. Monetary values are in U.S. dollars, with no implicit thousands scaling. Regions are fictional company groupings, not official Census regions. The U.S. localization preserves the teaching magnitudes without exchange-rate conversion.

### sales.csv

Each row represents an order/transaction recorded by a branch.

| Field | Meaning |
|---|---|
| `order_id` | Order identifier |
| `date` | Transaction date, YYYY-MM-DD |
| `branch_id` | Branch code |
| `product_id` | Product code |
| `customer_segment` | Customer segment recorded in the sale |
| `quantity` | Units sold |
| `unit_price` | Gross price per unit, in U.S. dollars |
| `discount_rate` | Discount as a proportion between 0 and 1 |

Valid discounts range from 0% to 40%, inclusive. There are no returns or negative quantities. Reference segments: Retail, Small Business, and Corporate.

### operating_registry.xlsx — sheet branches

Each row represents a branch. It should have no activity before its opening date.

| Field | Meaning |
|---|---|
| `branch_id` | Branch code |
| `branch` | Branch name |
| `region` | Company business region |
| `city` | Branch city and state |
| `opening_date` | Opening date, YYYY-MM-DD |

### operating_registry.xlsx — sheet products

Each row represents a product. The registry price need not equal the price observed in each sale.

| Field | Meaning |
|---|---|
| `product_id` | Product code |
| `product` | Product name |
| `category` | Business category |
| `reference_price` | Registry reference price, in U.S. dollars |

### costs.csv

Each row represents product × month. UTF-8, semicolon separator, decimal comma: this legacy export format is intentionally retained. Costs can vary over time.

| Field | Meaning |
|---|---|
| `product_id` | Product code |
| `month` | Reference month, YYYY-MM-01 |
| `unit_cost` | Unit cost for the month, in U.S. dollars |

### targets.csv

Each row represents branch × month. Missing values before opening represent legitimate nonoperation and should not be automatically imputed.

| Field | Meaning |
|---|---|
| `branch_id` | Branch code |
| `month` | Reference month, YYYY-MM-01 |
| `revenue_target` | Monthly revenue target, in U.S. dollars |
| `margin_target_rate` | Margin target as a proportion between 0 and 1 |

### Relationships and possible indicators

- Sales and branches: `branch_id`.
- Sales and products: `product_id`.
- Sales and costs: `product_id` and sale month.
- Monthly actuals and targets: `branch_id` and month.

Before joining, confirm the unit of observation and uniqueness of registry keys. No inference, forecasting, or outside information is needed. The tables support gross revenue, net revenue, total cost, margin, average order value, quantity, and actual-versus-target measures. These derived metrics are not supplied ready-made. Discount and margin-target rates are fractions: 0.10 represents 10%, not 0.10%.
