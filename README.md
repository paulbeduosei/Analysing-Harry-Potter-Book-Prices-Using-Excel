## Optimizing Product Pricing: Harry Potter Sequel

**SCM 651: Business Analytics, Homework 2 (Group 2)**

## Overview
The Book Emporium wants to set a profit-maximizing price for a new Harry Potter sequel. This project uses weekly pricing-test data from Harry Potter Book 7 to build a demand curve. It then finds the best selling price under three different publisher-cost scenarios.

## Assumptions
- Demand for the sequel will be similar to Harry Potter Book 7
- 100,000 customers will consider buying the book
- A power regression model gives a reasonable prediction of demand
- Base publisher cost is $5.00 per book

## Methodology
1. **Regression analysis:** Plotted percent purchased against price and fit a power regression.
   - Model: `y = 14.098x^(-1.872)`
   - R² = 0.9919 (explains about 99.19% of the variation in the log-transformed purchase percentages)
2. **Profit modeling:** Calculated predicted %, predicted sales, revenue, and profit at each price point, with conditional formatting on profit.
3. **Optimization:** Used Excel Solver to find the profit-maximizing price under three constraints:
   - Scenario 1: $5.00/book, no minimum order
   - Scenario 2: $4.50/book if at least 30,000 are sold
   - Scenario 3: $4.00/book if at least 50,000 are sold

## Results
| Scenario | Publisher Cost | Max Profit |
|---|---|---|
| 1 | $5.00 | $95,066.94 |
| **2** | **$4.50** | **$99,586.51** |
| 3 | $4.00 | $97,606.79 |

**Recommendation:** Scenario 2. Price the sequel at about **$7.82** and buy from the publisher at $4.50 per book. This gives the highest projected profit while still meeting the 30,000-unit minimum.

## Limitations
- Consumer preferences and buying habits may have changed since Book 7
- Competition from e-books, audiobooks, and other retailers may lower demand
- If actual sales fall below 30,000, the Scenario 2 discount and its profit are lost

## Future Improvements
- Recent sales data from comparable book releases
- Customer surveys on interest and willingness to pay
- Competitor pricing (e.g., Amazon, Barnes & Noble)
- Customer demographics
- Shipping, marketing, and operating costs for a more complete profit estimate
 
# Tools
Microsoft Excel (Regression, Solver, Conditional Formatting), Microsoft Word
