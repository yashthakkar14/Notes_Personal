#### Dealshare KT
- 10% of people at Dealshare see our prices.
- Every 4 hours, we need to update those prices based on competition and other factors.
- For this, we have a list of requirements from them.
- Color and size both different - master id (Amazon)
- color different size same - parent id (AMAZON)
- 4 level of hierarchies
- attribute : size
- active status are the products for which we need to do pricing.
- Do pricing for 100 products and they will compare with their other products.
- Products will change when they want the products to change.
- every 4 hours they will send the prices.
- 29 location - Delhi
- Inventory - stock, current stock
- timeID e.g. 16, that is 12:00:01-16
- product catalogue master data

#### Product Level Sales 
- Level : sku, location, orderdate, time, pricegroup
- Internal group means the 10% of the people.
- Data we show on the level : sellingPrice is the total number of units sold * listing price for a single unit.
- visits is for all the products
- impression is for a single product where they viewed the product.
- conversion is the customer who purchased the product.
- All the three are unique where each person is considered as 1, irrespective of how many times they visir or purchase.

#### Category Level Sales
- Level : categoryid, locationid, orderdate, timeId, pricegroup
- profit formula : revenue-cost/revenue (Markdow)

#### Task
- Download the CSV files from S3.
- Then deal those files in pandas
- dtypes