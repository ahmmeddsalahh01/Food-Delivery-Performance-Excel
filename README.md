# Food Delivery Business Performance Analysis

## Small overview

An Excel dashboard project exploring a generated food-delivery dataset across customer behavior, order outcomes, delivery operations, restaurant performance, and revenue. The dataset is fictional practice data and does not represent a real delivery business.


## Business questions

- How much order value is delivered, cancelled, or refunded?
- Which cities, cuisines, restaurants, and payment methods contribute to delivered sales?
- How often are orders delivered within the stated target, and how long do deliveries take?
- Which restaurants have higher cancellation and refund rates?
- How do customer order activity and loyalty tiers relate to revenue?
- Where can the delivery business improve customer experience and operating performance?

## Data

The project includes `food_delivery_analytics.xlsx`, with four tables:

- `fact_orders` — 6,000 orders with order date, customer, restaurant, rider, item count, order value, delivery fee, delivery time, customer rating, order status, and payment method
- `dim_customer` — 500 customers, including city, signup date, and loyalty tier
- `dim_restaurant` — 15 restaurants, including cuisine, city, and average cost for two
- `dim_rider` — 80 riders, including vehicle type, join date, and rider rating

The reporting workbook, `DELIVERY & BUSINESS PERFORMANCE.xlsx`, contains the Excel Data Model, supporting analysis, and five interactive dashboard pages. All data is generated for practice and demonstration.

## Dashboard pages

1. **Revenue & Growth** — total orders, delivered-order sales, average order value, monthly sales, sales by city and cuisine, and revenue by payment method.
2. **Order Funnel** — delivered, cancelled, and refunded order totals and shares; total refunds; refund rate; cancellation rates by city and restaurant.
3. **Delivery Performance** — average delivery time, share delivered within target, delivered orders, delivery time by vehicle type, and average time by rider.
4. **Customer Insights** — customer count, orders per customer, total order value, and revenue by loyalty tier.
5. **Restaurant & Rider Performance** — average delivery time and rider rating, restaurant average order value, and cancellation rate by restaurant.

## Detailed key findings

- The dataset contains **6,000 orders**: **5,270 delivered (87.83%)**, **477 cancelled (7.95%)**, and **253 refunded (4.22%)**.
- The Revenue & Growth page reports **2,132,701 EGP** in sales from delivered orders. The Customer Insights page reports **2,420,695 EGP** in total sales across the order data. These are different scopes; delivered-order sales are the more relevant figure for realized sales.
- The dashboard displays an **average order value of 355.45 EGP**. This equals delivered-order sales divided by all 6,000 orders. Dividing delivered-order sales by the 5,270 delivered orders gives about **404.69 EGP per delivered order**. State which definition is intended and use it consistently.
- Average delivery time is about **34.68 minutes**, and **55.53%** of orders are shown as delivered within the target time. The workbook does not state the target threshold.
- Total refunds are about **102,424 EGP** across 253 refunded orders. The displayed refund rate is **4.22%** of all orders.
- Delivered-order sales are highest in **October (about 187,943 EGP)** and lowest in **February (about 157,870 EGP)** in the monthly chart.
- **Aswan** has the highest displayed sales by city at about **431,271 EGP**. Cairo is lowest at about **142,058 EGP**; sales alone do not show whether this reflects order volume, delivery capacity, or average order value.
- **Italian cuisine** contributes the largest displayed cuisine share (**20.56%**) and **Healthy** the smallest (**7.09%**). The payment method shares are close: Credit Card **714,192 EGP**, Cash on Delivery **709,983 EGP**, and Mobile Wallet **708,526 EGP** in delivered-order sales.
- **Green Bowl** has the highest displayed restaurant cancellation rate (**9.86%**); **Wok This Way** has the lowest (**5.84%**). Order counts and cancellation reasons should be reviewed before comparing or acting on these rates.
- The rider rating average is about **4.52**. Average delivery times by vehicle type are close to **35 minutes**, with little separation in the displayed chart.
- Bronze-tier guests account for about **48%** of the revenue shown by loyalty tier, compared with Silver **28%**, Gold **19%**, and Platinum **5%**.

## Advanced recommendations

1. **Improve on-time delivery through a targeted operations pilot.** Only 55.53% of orders are marked within the target time, while average delivery time is about 34.68 minutes. First define the customer-facing SLA, then pilot changes to restaurant preparation handoffs, rider dispatch timing, or delivery-zone coverage in a small set of locations. Compare on-time rate, median and 90th-percentile delivery time, customer rating, and cost per completed order before expanding.
2. **Reduce cancellations and recover at-risk orders.** Cancellation rates are highest at Green Bowl and lowest at Wok This Way in the displayed restaurant comparison. Have the higher-rate restaurants review order acceptance, item availability, and preparation capacity; offer customers substitutions when an item is unavailable. Track cancellations by reason and compare rates using order counts, then keep changes that reduce cancellations without increasing refunds or delays.
3. **Control refund losses and improve service recovery.** The report shows 253 refunded orders and about 102,424 EGP in refunds. Record a consistent refund reason, identify recurring restaurant or delivery issues, and give support staff a clear recovery process such as replacement or credit when appropriate. Monitor refund rate and amount alongside complaint resolution time and repeat orders.
4. **Plan promotions and capacity around demand.** February is the lowest-sales month in the displayed chart and October the highest. Test a targeted February promotion with selected restaurants, and schedule sufficient restaurant and rider capacity for October. Compare incremental delivered sales, contribution after discounts, on-time delivery, and cancellations against comparable periods; do not assume a single year's pattern will repeat.
5. **Build repeat business among Bronze-tier customers.** Bronze accounts for the largest shown share of loyalty-tier revenue. Test a simple next-order reward or personalized offer for Bronze customers, with clear expiry and minimum-spend rules. Measure repeat-order rate, average contribution per customer, and reward cost to ensure the campaign creates incremental value.
6. **Strengthen restaurant and city planning.** Aswan leads the displayed city sales, while Green Bowl has the highest restaurant cancellation rate. Review order volume, staffing, menu availability, delivery radius, and contribution by location before adding capacity or changing service areas. Use a limited operational pilot and compare completed orders, on-time delivery, cancellations, and contribution per order.
7. **Use rider coaching and recognition fairly.** The overall rider rating is about 4.52, and vehicle-type averages appear similar. Recognize consistently strong service and coach riders with recurring low ratings or delivery delays only after checking their order counts, routes, and conditions. Track delivery time and customer rating together so speed improvements do not reduce service quality.
8. **Maintain convenient payment choice.** Delivered sales are nearly evenly distributed across Credit Card, Cash on Delivery, and Mobile Wallet. Keep all three payment options available and use a controlled test before offering a payment-specific incentive. Compare completed orders, payment failure or refund rates, and transaction costs before changing payment strategy.

## Tools

- Microsoft Excel
- Excel Data Model and PivotTables
- Generated practice dataset in `.xlsx` format
