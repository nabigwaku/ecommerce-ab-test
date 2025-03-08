# E-Commerce A/B Test: Free Shipping Thresholds

This repository contains the design, data, and analysis for an A/B test conducted to evaluate the impact of free shipping thresholds on customer purchase behavior in an e-commerce platform.

## **Overview**
The experiment aimed to determine whether offering free shipping on orders above $50 (Group A) would increase **average order value (AOV)** and **conversion rates** compared to a control group with no free shipping banner or a higher threshold (Group B).

## **Repository Structure**
  * [Data Folder](https://github.com/nabigwaku/ecommerce-ab-test/data): Contains a dataset with fields: user IDs, group assignments, order values, and conversion status
  * [Analysis Folder](https://github.com/nabigwaku/ecommerce-ab-test/analysis): Contains Jupyter Notebook for data analysis and statistical testing
  * [Readme MD File](https://github.com/nabigwaku/ecommerce-ab-test/README.md): Documents an overview of the project
  * [Experiment design MD File](https://github.com/nabigwaku/ecommerce-ab-test/experiment_design.md): Documents the detailed experiment design and methodology

## **Data**
The dataset (`ecommerce_experiment_data.csv`) contains the following columns:
- `user_id`: Unique identifier for each user.
- `group`: Experiment group (A = Free shipping on orders > $50, B = Control group).
- `order_value`: Total value of the order in USD.
- `converted`: Binary indicator (1 = user converted, 0 = user did not convert).

## **Analysis**
The analysis includes:
1. Calculation of **average order value (AOV)** and **conversion rates** for both groups.
2. Statistical testing (such as t-test, chi-square test) to determine if the differences are significant.
3. Visualization of key metrics.

## **Set Instructions**
1. Clone the repository:
   ```bash
   git clone https://github.com/nabigwaku/ecommerce-ab-test.git

2. Install dependencies:
   ```bash
   pip install pandas numpy scipy matplotlib
   
4. Run the Jupyter Notebook (analysis.ipynb) to perform the analysis.
