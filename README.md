# Customer Rewards Calculator based on customer transaction
The rest API to get customer rewards based on customer Id

A retailer offers a rewards program to its customers, awarding points based on each recorded purchase.

A customer receives 2 points for every dollar spent over $100 in each transaction, plus 1 point for every
dollar spent between $50 and $100 in each transaction.
(e.g., a $120 purchase = 2x$20 + 1x$50 = 90 points).  

To start the application navigate to `src/main/java/com/retail/customer/rewards/CustomerRewards/CustomerRewardsApplication.java` and start the application.
The application loads `classpath: script.sql` file to h2 database when the application starts. You can add data as desired by running sql scripts on the databse.

Exposed Endpoints are:
1. `v1/customers` for getting all customer and their ids
2. `v1/customers/{customerId}/rewards` to view the rewards for the last 3  months

Swagger Docs:
   ``http://localhost:8080/swagger-ui/index.htm``
