---
# e-Commerce-Churn-Customer-Prediction
---

## Introduction

Customer churn or attrition is one of the most crucial problems for any business that directly sells or serves customers be it Telecom service providers, eCommerce, insurance and many more. It is important to track and analyse how many customers are leaving the platform and how many are sticking and the reasons behind them. Knowing customer behaviour can greatly enhance decision-making processes and can further help reduce churn to improve profitability.

In this project, we are going to analyse an eCommerce dataset and find the best model to predict customer churn.

### Data Source:
[X e-Commerce Dataset](https://drive.google.com/drive/folders/1Ffl_KwbH2oIRVOYToGy56-p5RBKfZwsi?usp=sharing) 

## Business Context

E-Commerce is one form of technological development in the economic field which includes the process of promotion, purchasing and marketing of products through electronic media or the internet. In the midst of the development of increasingly sophisticated digital information and technology flows. E-Commerce activity is an implementation of E-Business or electronic business that is quite effective, so that there are more eCommerce platforms and the competition is getting tougher. An eCommerce company called "X E-Commerce" runs an online retail business with a B2C (Business to Consumer) model with products offered such as Laptops & Accessories, Mobile Phones, Fashion, Groceries, and others. Today's eCommerce companies are competing to innovate in offering attractive products to customers. In fact, companies are acquiring customers from each other's eCommerce companies. So that customers stop transacting using the company's eCommerce platform and switching to other eCommerce platforms is very possible. This customer behavior is known as Churn. Customers are one of the most important assets of the company and have a very important role in improving market competitiveness and company performance. Launching from the European Business Review webpage, Research shows that the cost of acquiring a new customer is often higher (5 times more expensive) than the cost of retaining an existing customer. The company will experience a significant loss if there are customers who churn.

## Problem Statement

Churn prediction is identifying customers that are most likely to live a service. This is important for most companies as acquiring new customers is more costlier than retaining old ones, So the results of Churn prediction help companies focus on customers that are likely to churn and develop strategies for retaining those customers.

Churned customer is one of the problems which should be faced in any of eCommerce business because generally the customers will always come and go. But if the Churn keeps happening, that could be the profound impact on the long term income. Since the eCommerce market increasing in more competitive way, for some years running the business, the customers acquisition's costs increasing because of the needs of more digital commercial and of that marketing still remain seen. If the company cannot maintain the customers after the initial invest, thus the profits will significantlly decrease. In addition, if the churned customers on the grounds of disappointment, it is most likely they will tell the others so that affecting others to not using the eCommerce platform of company X.

## Goals

Based on these problems, reducing customer churn is the company's main business goal. This company wants to have the ability to predict the probability that customers will churn/not, and know what factors/variables can influence customers to churn/not. So that companies can plan more suitable offers to customers who have the potential to retain customers.

## Analytic Approach

So, what we need to do is analyze the data to be able to find the pattern of features that exist, which differentiate customers who are likely to churn and those who are not.

Next, we will build a classification model that will help companies to be able to provide a tool to predict customers who are likely to churn or not.

## Metric Evaluation

`Positive Class : Churn`

`Negative Class : Not Churn (Retain Customer)`

| Type I error (False Positive) refers to a customer who is predicted to Churn but plans to remain loyal. |
| --- |

Consequences: If we assume e-Commerce X invests in retaining customers who are at risk for churn but in fact these customers will not churn such as offering new products at special prices, increasing the amount of cashback, etc. This type I error is due to the investment costs being passed on to customers who are not planning to Churn.

| Type II error (False Negative) refers to customers who will Churn but are predicted to remain loyal / not churn. |
| --- |

Consequences: Assuming e-Commerce X only focuses its investment in retaining risky customers so as not to Churn and continues to provide the same offers to other loyal customers, so this Type II Error is losing customers. The company will be at a great loss because the cost of acquiring new customers is estimated to be higher than that of retaining current customers.

| Actual | `P` | `N` |
| --- | --- | --- |
**Predicted** 
| `P` | TP | $FP$ |
| `N` | $FN$ | TN |

Based on the consequences, then as much as possible what we will do is create a model that can reduce the number of customer losses from the company and reduce the cost of wasted investment in retaining customers who are predicted to Churn but in reality customers will not Churn.

For this reasons, we will minimize *False Postive* and *False Negative* to optimize the profit for company X. So the metric we will use is *F1-Score*.
