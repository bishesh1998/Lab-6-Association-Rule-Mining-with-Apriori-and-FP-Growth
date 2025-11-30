# Lab-6-Association-Rule-Mining-with-Apriori-and-FP-Growth


Lab 6: Association Rule Mining
Overview

This lab applies Apriori and FP-Growth to a retail dataset from UCI Online Retail to identify frequent itemsets and generate association rules.

Key Steps

Data Cleaning: Removed canceled transactions, missing values, and negative quantities.

Exploration: Top items include PAPER CRAFT, LITTLE BIRDIE, MEDIUM CERAMIC TOP STORAGE JAR, and WORLD WAR 2 GLIDERS. Most invoices had few distinct items. Co-occurrence is strong within related product families (e.g., Jumbo Bags, Popcorn Holders).

Frequent Itemsets: Using top 50 items and min_support=0.02, Apriori and FP-Growth found 180 frequent itemsets. Apriori was faster (0.38s vs 7.92s).

Association Rules: With min_confidence=0.1, weak rules were found; strong rules were limited due to low co-occurrence.

Insights

Customers tend to buy popular items individually or in small related groups. Multi-item frequent sets are rare. Apriori performed faster than FP-Growth on this subset, and dataset size matters for memory management in Colab.
