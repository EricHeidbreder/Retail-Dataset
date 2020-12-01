# Data description

This is a transnational data set which contains all the transactions occurring between 12/01/2010 and 12/09/2011 for a UK-based and registered non-store online retail. For the purposes of presentation, we'll call this store 'iShop'

## Data Dictionary

| **Column Name** | **Data Type** | **Description**                                                                                                                        |
|-----------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------|
| `InvoiceNo`     | string        | A 6-digit integral number uniquely assigned to each transaction. If this code starts with the letter ‘c’, it indicates a cancellation. |
| `StockCode`     | string        | Product (item) code.  A 5-digit integral number uniquely assigned to each distinct product.                                            |
| `Description`   | string        | Product (item) name.                                                                                                                   |
| `Quantity`      | int64         | The quantities of each product (item) per transaction                                                                                  |
| `InvoiceDate`   | datetime64    | The day and time when each transaction was generated.                                                                                  |
| `UnitPrice`     | float64       | Product price per unit in sterling.                                                                                                    |
| `CustomerID`    | int64         | A 5-digit integral number uniquely assigned to each customer.                                                                          |
| `Country`       | string        | The name of the country where each customer resides.                                                                                   |

## Problems / Questions

* What are the best months for sales, and what products are selling best during those months?

* What is the customer breakdown? What's the distribution of high-value/mid-value/low-value customers?

* What is the average order per customer?

* What is the month-to-month churn rate?

* How can iShop implement changes that will lead to positive growth in sales in the coming year given that the retailer only has one year of data?

## Cleaning process



## Recommendations

* Unify the way lost/damaged items are codified to better track how many items are being returned or lost. This could be a problem if the rate of returns/lost items gets too high.

* Monthly churn will not be a good indicator since our customers seem to buy a lot of party supplies. Recommend changing the metric to yearly to see if returning customers are buying more supplies every year.

* To boost sales, client could implement a recommender system or secure more items related to event/party planning so customers can stay on the platform for all event/party planning needs

* For better sales analysis, we should have subcategories available. Recommend using natural language processing to identify subcategory clusters.