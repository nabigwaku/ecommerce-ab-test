# Experiment Design: Free Shipping Thresholds

## **Objective**
To determine whether offering free shipping on orders above $50 increases **average order value (AOV)** and **conversion rates** compared to a control group with no free shipping banner or a higher threshold.

## **Hypotheses**
- **Null Hypothesis (H₀)**: The free shipping banner has no effect on AOV or conversion rates.
- **Alternative Hypothesis (H₁)**: The free shipping banner increases AOV or conversion rates.

## **Target Population**
- **Active users**: Users who have made at least one purchase in the last 3 months.
- **Geographic region**: United States.
- **Device type**: Both mobile and desktop users.

## **Experiment Groups**
- **Group A (Treatment)**: Users see a banner offering free shipping on orders above $50.
- **Group B (Control)**: Users see no banner or a banner with a higher threshold (e.g., $75).

## **Metrics**
### Primary Metrics
- **Average Order Value (AOV)**: Total revenue divided by the number of orders.
- **Conversion Rate**: Percentage of users who complete a purchase.

### Guardrail Metrics
- **Cart Abandonment Rate**: Percentage of users who add items to the cart but don’t complete the purchase.
- **Revenue per User**: Total revenue divided by the number of users.

## **Sample Size**
- **Total Users**: 1,000+ (randomly split between Group A and Group B).
- **Duration**: 2 weeks to account for weekly shopping patterns.

## **Randomization**
- Users are randomly assigned to Group A or Group B based on their `user_id`.

## **Data Collection**
- Track user behavior (e.g., cart additions, purchases, order values) and log it in a database.
- Example CSV structure:
  | user_id | group | order_value | converted |
  |---------|-------|-------------|-----------|
  | 1       | A     | 55.00       | 1         |
  | 2       | B     | 40.00       | 0         |
  | 3       | A     | 60.00       | 1         |
  | 4       | B     | 75.00       | 1         |

## **Analysis Plan**
1. Calculate AOV and conversion rates for both groups.
2. Perform statistical tests (e.g., t-test for AOV, chi-square test for conversion rates) to determine significance.
3. Visualize results using graphs (e.g., bar charts, box plots).

## **Expected Outcomes**
- If Group A performs significantly better: Roll out the free shipping banner to all users.
- If no significant difference: Test alternative thresholds or other incentives.
- If Group B performs better: Investigate why (e.g., higher threshold may encourage larger orders).

---

### **Next Steps**
1. Run the experiment and collect data.
2. Analyze the results using the provided Jupyter Notebook (`analysis.ipynb`).
3. Document findings and make data-driven recommendations.
