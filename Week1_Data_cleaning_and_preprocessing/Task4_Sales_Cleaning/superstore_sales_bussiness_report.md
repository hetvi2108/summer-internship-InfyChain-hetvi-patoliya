# Superstore Sales Analysis — Business Insights Report

---

## 1. Overview

This report presents a comprehensive analysis of the Superstore dataset
covering sales performance, profit trends, category and regional breakdowns,
and discount impact from 2014 to 2017. The goal is to identify key drivers
of revenue and profitability and highlight areas that require strategic attention.

---

## 2. Sales and Profit Analysis by Category

Based on the analysis we can conclude that higher revenue generated
by a category does not necessarily lead to higher profit.

- **Technology** has the highest revenue generation and also maintains
  the highest profit among all categories, successfully maintaining
  strong profitability.

- **Furniture** is the second highest revenue generating category
  but has the lowest profit generation compared to **Office Supplies**,
  which despite having lower revenue than Furniture, generates
  higher profit than it.

- This indicates potential issues with discount levels, shipping costs
  and marketing and pricing strategy in the Furniture category,
  making it an important category for further analysis.

---

## 3. Sales and Profit Analysis by Sub-Category

Based on the sub-category analysis, the low profit ratio for the
**Furniture** category is primarily driven by **Tables** and **Bookcases**,
both of which are generating negative profit for the category.

- **Tables** are generating the highest negative profit even in
  comparison to Bookcases, which heavily impacts the overall profit
  ratio for the Furniture category. Possible reasons include issues
  with margins, discount levels, shipping costs, pricing strategy
  and marketing strategy.

- The **Technology** category is performing very strongly in profit
  generation with **Phones, Copiers and Accessories** being the top 3
  profit generating sub-categories. However **Machines** are generating
  the lowest profit compared to other sub-categories in this category,
  which requires further analysis before drawing any conclusion.

- For **Office Supplies**, only the **Supplies** sub-category is generating
  a very small portion of negative profit. The majority of profit for
  this category is coming from **Paper, Binders and Storage** sub-categories.

---

## 4. Deep Dive Analysis — Tables and Bookcases

Analysis of loss-making Tables and Bookcases reveals that higher
discounts, larger order quantities and increased sales volume are
all associated with declining profitability.

### Correlation Findings

**Profit vs Sales — (-0.68)**
Strong negative correlation indicating that higher sales do not
guarantee profitability for these sub-categories.

**Profit vs Quantity — (-0.52)**
Quantity negatively impacts profit, suggesting that bulk orders
are contributing to larger losses rather than economies of scale.

**Profit vs Discount — (-0.39)**
Moderate negative correlation confirming that aggressive discounting
is significantly reducing profit margins.

**Tables vs Bookcases**
Tables generate more severe losses compared to Bookcases,
particularly at discount levels between **40% and 50%**.

> Current pricing and discount strategies for Furniture products
> are unsustainable and require immediate optimization to
> prevent continued profit erosion in this category.

### Shipping Method Impact

The shipping method analysis for **Tables and Bookcases** reveals a clear
pattern — as the shipping quality improves, the profit becomes more negative.

This confirms that Tables and Bookcases are likely fragile products that
require premium shipping handling, and the higher cost associated with
better shipping methods is significantly eating into the profit margins,
further contributing to the overall loss in the Furniture category.

> Current pricing and discount strategies for Furniture products
> are unsustainable and require immediate optimization to
> prevent continued profit erosion in this category.

---

## 5. Region Wise Sales and Profit Analysis

**West**
Performs the best in both sales and profit, maintaining the
highest numbers across both metrics.

**East**
Follows closely behind West, maintaining a strong margin of
high profit and high sales generation.

**South**
Has the lowest sales among all regions but its profit margin
is higher compared to the Central region, suggesting that
sales volume alone does not determine profit and business efficiency.

**Central**
The least efficient region business wise, generating the lowest
profit despite having higher sales than the South region,
indicating deeper issues with costs, discounts or pricing strategy.

---

## 6. Yearly and Monthly Revenue Trend Analysis

### Yearly Analysis
Superstore sales generally increased from **2014 to 2017** with only
a slight decline in sales during **2015**. Profit however increased
consistently every year including 2015, indicating positive business
development and improving profitability over time.

### Monthly Trends
Sales consistently reach higher levels toward the end of the year,
particularly from **September to December**, which is likely driven
by seasonal demand and increased shopping activity during
the holiday period.

### Profit Volatility
While profit shows an overall positive trend, monthly profit is
more volatile compared to sales. Some months show sharp increases
while a few periods even record negative profit.

Notable profit peaks in **late 2016** and **March 2017** stand out
and may require further analysis to understand which categories,
regions or discount levels contributed to these unusual spikes.

> Despite occasional volatility, the overall business trajectory
> is positive with both sales and profit showing consistent
> growth from 2014 to 2017.

---

## 7. Key Findings

**Technology** is the most profitable category with highest sales and profit.

**Furniture** has high sales but the lowest profitability among all categories.

**Tables and Bookcases** are the primary loss-making sub-categories
dragging down the entire Furniture category.

**West** is the strongest region by sales, profit and profit margin.

**Central** has the lowest profit margin among all regions despite
having higher sales than South.

**No-discount orders** generate the highest total profit overall.

**20% discount** is the most effective discount level among discounted orders.

**Discounts above 20%** are consistently associated with negative profitability.

**Sales and profit** both increased overall from 2014 to 2017.

---

## 8. Recommendations

**Furniture Category**
Review Tables and Bookcases urgently to understand why these
sub-categories are generating losses despite high sales volume.

**Discount Strategy**
Reconsider all discount levels above 20% as they are consistently
associated with negative profitability. Use the 20% discount level
more strategically as it appears to be the most effective among
discounted orders.

**Central Region**
Investigate whether low profitability is caused by discounts,
product mix or specific loss-making sub-categories being
pushed more in this region.

**Technology Category**
Continue investing in strong sub-categories such as Copiers,
Phones and Accessories. Further analyze the Machines sub-category
for potential improvement opportunities.

**Seasonal Strategy**
Leverage the September to December peak period more aggressively
with targeted campaigns while maintaining healthy profit margins
during high discount periods.

---

## 9. Limitations

This analysis is based solely on the available Superstore dataset.
Important business factors such as marketing costs, inventory levels,
customer acquisition costs, detailed shipping costs and product level
margins are not included. Therefore some recommendations should be
treated as hypotheses for further investigation rather than
definitive conclusions.

---

*Analysis performed using Python, Pandas, Matplotlib and Seaborn*
*Dataset Source: Kaggle Superstore Dataset*