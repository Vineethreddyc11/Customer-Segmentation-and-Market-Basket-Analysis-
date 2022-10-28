
![1_DHfQvlMVBaJCHpYmj1kmCw](https://user-images.githubusercontent.com/68578215/198731722-d806271a-af9b-4ca7-b879-88ab390ffdab.png)

# Customer-Segmentation-and-Market-Basket-Analysis-

Analyzed 3M+ grocery orders data from more 200k+ users to increase profitability by leveraging customer transaction behavior and purchasing history and discovered hidden association rules between products for better cross-selling and upselling.

## Introduction
- Instacart is an American company that operates a grocery delivery and pick-up service in the United States and Canada. The company offers its services via a website and mobile app. The service allows customers to order groceries from participating retailers with the shopping being done by a personal shopper.

- With the large customer base, the company collects data of the users’ transactions behaviour and purchasing history.

- The objective of this study is to increase profitability by tailoring suitable marketing approach and find key driver to used as a lever to improve profit.

- The dataset contains a sample of over 3 million grocery orders from more than 200,000 Instacart users.

- Dataset: https://www.kaggle.com/c/instacart-market-basket-analysis



![Screen Shot 2022-10-28 at 1 26 09 PM](https://user-images.githubusercontent.com/68578215/198726446-777d43b0-c1fb-4f5a-adeb-12acce4ec239.png)

## Business Model

- Customers access Instacart’s platform via website or app. Whenever an order is placed on the platform, the so-called personal shoppers in proximity will receive a notification of the request. These shoppers are independent contractors, and they receive by delivery made. Once a shopper accepts the request, they drive to the grocery store chosen, pick up the groceries and deliver them to the customer’s address.
#### Revenue Stream
- Commissions
  - Every time an item is sold through Instacart’s platform, the company receives a percentage of the price, according to the agreement made with the retailer. In some cases, Instacart even sells some products at a higher price to increase markup.
- Delivery and Service Fees (Price Discrimination)
  - Delivery fees vary from USD 3.99 - 9.99. Because Instacart, just like other platforms, such as Uber or Lyft, charges according to the demand and external conditions (such as the weather), the so-called surge pricing. And also due to shipment scheduling. These fees are distributed between the store and Instacart. The service fees (mark-up prices) get around 5% to 10% of the purchase. Sometimes, there are additional fees, for example, when an order surpasses a certain weight threshold or when there is a bag fee.
- Subscription
  - The company has the Instacart Express. It is a subscription service that ensures unlimited deliveries (or orders above USD 35), cheaper service fees, and no surge pricing for an annual (USD 99) or monthly fee (USD 9.99).
- Advertising
  - Sellers and brands can advertise on the platform, for additional visibility. The price will depend on the categories and search terms. Usually, advertisers set a budget previously, to avoid overspending.
#### Cost Structure
- Technological maintenance
- Salaries
- Shoppers payment
- Payment processing fees
- Administration and operations
- Marketing
#### Key Customer
**Users:** People who don’t like shopping, elderly people, people who have a tight schedule; Users can schedule orders for a specific day and time.

**Shopper:** People with a smartphone and a vehicle (car or bicycle), people who love shopping, people who need an additional income.

**Partner Stores:** The ones that want to increase their sales, and those that want to reach out to more customers.
#### Value Proposition
**Users:** A convenient way to shop for groceries, quick delivery, vast inventory;
**Shoppers:** Flexible working schedule, additional income, part-time work;
**Stores:** Additional sales, increase in the number of customers.

## Tableau Dahboard


![Screen Shot 2022-10-28 at 1 53 14 PM](https://user-images.githubusercontent.com/68578215/198730713-5797faf3-a12d-4df6-a925-0084d700d7d9.png)

![Screen Shot 2022-10-28 at 1 53 40 PM](https://user-images.githubusercontent.com/68578215/198730706-dae3885c-bbbd-4970-8060-31b17db54fd0.png)

## Exploratory Data Analysis using Python

#### Number of Products by Department

<img width="961" alt="Screen Shot 2022-10-28 at 11 49 01 AM" src="https://user-images.githubusercontent.com/68578215/198719152-1224edea-0b72-4595-9db6-1464cf56d321.png">

- Personal Care and Snacks category offered the most various type of products.

#### Number of Products by Aisle 

<img width="1017" alt="Screen Shot 2022-10-28 at 11 49 16 AM" src="https://user-images.githubusercontent.com/68578215/198719149-6ea37194-4dde-49b6-90d5-a94258c74e58.png">

- Candy Chocolate aisle offered most variety types of products.

#### Consumer Buying Behaviour

<img width="979" alt="Screen Shot 2022-10-28 at 11 49 29 AM" src="https://user-images.githubusercontent.com/68578215/198719148-50554d1f-6f0b-427b-bc1d-c3e84e9a2f25.png">

- Most orders are placed in Day 0 & 1 (Saturday and Sunday). Most people usually shopping in the weekend. Tuesday and Wednesday have the least activity.

<img width="963" alt="Screen Shot 2022-10-28 at 11 49 37 AM" src="https://user-images.githubusercontent.com/68578215/198719147-fcfb7f83-bae1-452f-8b3f-e30b28f73442.png">

#### Freqency of Orders by hours of the day

<img width="881" alt="Screen Shot 2022-10-28 at 11 49 43 AM" src="https://user-images.githubusercontent.com/68578215/198719145-346ea39b-a9e6-4403-a397-2f3dd8a0cb3c.png">

- Order starts getting busy after 8 AM.
- The number of order almost constant between 9 AM till 4 PM. This is a range of busy hour.
- Order start decreasing after 4 PM.

#### Consumer Buying Pattern


<img width="914" alt="Screen Shot 2022-10-28 at 11 49 50 AM" src="https://user-images.githubusercontent.com/68578215/198719143-fab402c3-ddae-4236-8403-54e64c892cd6.png">

- Most Customer shop on the weekend, from 9 AM to 4 PM.
- On the weekdays, most order are placed on Friday. Afternoon has less traffic because of working hours.
- On Tuesday & Wednesday, there is not much activity.

#### Number of orders since last order

<img width="987" alt="Screen Shot 2022-10-28 at 11 49 57 AM" src="https://user-images.githubusercontent.com/68578215/198719140-31049c92-8204-4468-ad52-5996131e376d.png">

- Most people doing recurring shopping weekly or monthly.

#### Items per transaction

<img width="967" alt="Screen Shot 2022-10-28 at 11 50 07 AM" src="https://user-images.githubusercontent.com/68578215/198719136-e38946a4-1f80-49e3-884d-ea05a9b994f8.png">

- Most people buy 1 -10 items in 1 transactions. Most frequent transaction is 5 items per order.


#### Number of transaction per customer

<img width="986" alt="Screen Shot 2022-10-28 at 11 50 22 AM" src="https://user-images.githubusercontent.com/68578215/198719135-67d4249b-ea50-4620-8569-3ad431e22bad.png">

- Most user made a transaction between 3-6 transactions. It is indicated that Instacart has a problem in retaining new customer.

### Orders vs Hour of day

![Screen Shot 2022-10-28 at 12 32 05 PM](https://user-images.githubusercontent.com/68578215/198719134-106104b0-404d-48dc-8758-2c151fecb35c.png)

- Most orders are placed from Early morning to midnight, and very few orders placed from midnight to early morning.


#### Frequently reordered product by weekly buyers


![Screen Shot 2022-10-28 at 1 08 35 PM](https://user-images.githubusercontent.com/68578215/198724154-3194956a-c4b1-4b65-b632-74c187c10f73.png)


#### Frequently reordered product by monthly buyes

![Screen Shot 2022-10-28 at 1 08 40 PM](https://user-images.githubusercontent.com/68578215/198724151-ec6563d6-d887-4b35-92e9-3a4ce707b229.png)

#### users with orders containing only reordered products

![Screen Shot 2022-10-28 at 1 17 20 PM](https://user-images.githubusercontent.com/68578215/198724715-d064fe26-2bec-41af-8a2d-f2ac176b366b.png)

- User_id 99753 have 99 orders which contains only reordered items
- Followed by User 26489 and 100935
