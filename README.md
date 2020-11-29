# Abstract

This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.

## Attribute Information

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

## Problem / Questions

* What are the best months for sales, and what products are selling best during those months?

* What is the customer breakdown? What's the distribution of high-value/mid-value/low-value customers?

* What is the average order per customer?

* What is the month-to-month churn rate

## Next Steps

Unify the way lost/damaged items are codified to better track how many items are being returned or lost. This could be a problem if the rate of returns/lost items gets too high.