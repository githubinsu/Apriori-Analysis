# Customer Product Recommendation using Apriori Analysis

## Apriori Analysis
Apriori analysis involves analyzing transaction data to find sets of products that are frequently purchased together. This information is used to generate association rules, which can then be used to make product recommendations. For example, if there is an association rule that states “apples and bananas are frequently purchased together,” then a customer who purchases apples could be recommended bananas.

## Background
It is important to understand the purchasing behavior of customers in order to provide personalized product recommendations. By analyzing the transaction data, we can discover patterns and relationships between different products, and use this information to recommend products that are likely to be purchased together.

## Objective
The goal of this project is to use Apriori analysis to generate personalized product recommendations for customers. I have a dataset containing transaction data, where each row represents an individual order and the columns include information such as Order Date, Customer ID, Product Number, Price, Sector, Category, and Subcategory.

## Method
I used the `mlxtend` library to perform Apriori analysis on the transaction data. First, I preprocessed the data by grouping the orders by Order Date and Customer ID, and transforming the data into a format suitable for Apriori analysis using the `TransactionEncoder` class. Then, I used the `apriori` function to generate frequent itemsets and the `association_rules` function to generate association rules.

## Results
The resulting association rules represent relationships between different products. For example, if an association rule has antecedents `(A)` and consequents `(B)`, it means that customers who purchased product A are also likely to purchase product B. We can use these rules to generate personalized product recommendations for each customer.

## Future Applications
The results of this analysis can be used to increase basket size by recommending additional products to customers. By providing personalized product recommendations, we can improve customer satisfaction and increase sales. In addition, this analysis can be extended to other areas such as market basket analysis and customer segmentation.
