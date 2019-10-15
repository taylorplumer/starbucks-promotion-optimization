## Project Background

This project is part of the Udacity Data Scientist Nanodegree program and uses a synthetic dataset from Starbucks. The dataset consists of about 120,000 data points split in a 2:1 ratio among training and test files.

As per project background information:

>>In the experiment simulated by the data, an advertising promotion was tested to see if it would bring more customers to purchase a specific product priced at $10. Since it costs the company 0.15 to send out each promotion, it would be best to limit that promotion only to those that are most receptive to the promotion. Each data point includes one column indicating whether or not an individual was sent a promotion for the product, and one column indicating whether or not that individual eventually purchased that product. Each individual also has seven additional features associated with them, which are provided abstractly as V1-V7.

## Objective

The project prompt was to maximize Incremental Response Rate and Net Incremental Revenue. The optimization strategy is then evaluated against test data and a benchmark model.

## My Approach

I went ahead and used the training data to build a model to classify users as either "Yes" or "No" to whether the user should receive the promotion. Due to imbalanced classes, I upsampled the minority class and utilized a Gradient Boosting Classifier.

## Important Files

| File | Description |
| --- | ----------- |
| Starbucks_PromotionStrategy_Classifier.ipynb | Notebook containing analysis and evaluation |
| training.csv | training data  |
| Test.csv | test data that is utilized by the test_results module  |
| test_results.py | module used to evaluate optimization strategy against benchmark  |
| yellowbrick_visualizer.ipynb  | notebook that uses yellowbrick's [Classification Visualizers](https://www.scikit-yb.org/en/latest/api/classifier/index.html)  |


