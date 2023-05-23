
**Business Intelligence Analysis for Plato Pizza**


Role: BI Consultant.


**Consultancy Overview:**

For this project, I played the role of a BI Consultant hired by Plato's Pizza, a Greek-inspired pizza place in New Jersey. You've been hired to help the restaurant use data to improve operations, and just received the following note:



**Client Request:**
Welcome aboard, we're glad you're here to help!



Things are going OK here at Plato's, but there's room for improvement. We've been collecting transactional data for the past year, but really haven't been able to put it to good use. Hoping you can analyze the data and put together a report to help us find opportunities to drive more sales and work more efficiently.



1. Here are some questions that we'd like to be able to answer:

2. What days and times do we tend to be busiest?

3. How many pizzas are we making during peak periods?

4. What are our best and worst-selling pizzas?

5. What's our average order value?

6. How well are we utilizing our seating capacity? (we have 15 tables and 60 seats)



That's all I can think of for now, but if you have any other ideas I'd love to hear them – you're the expert!

Thanks in advance,


Mario Maven (Manager, Plato's Pizza)



For this challenge, your task is to build a single-page dashboard based on Mario's email to help him improve the restaurant's operations.







**Work Steps:**



**About the dataset:**

This dataset contains 4 tables in CSV format;

The "Orders" table contains the date & time that all table orders were placed

The "Order Details" table contains the different pizzas served with each order in the Orders table, and their quantities

The "Pizzas" table contains the size and price for each distinct pizza in the Order Details table, as well as its broader pizza type

The "Pizza Types" table contains details on the pizza types in the Pizzas table, including their name as it appears on the menu, the category it falls under, and its list of ingredients.






**B.I Tool used: Microsoft Excel, MS Power Query and PowerBi**





**Data transformation:**

Upon loading the data csv files into Power Query Editor;

1. I created two new columns (Unit Price and Sales) in the Order Details table to ascertain the total sales for each Pizza type and order quantity.

 2. I created new columns in the Order table by extracting the Month, Day, and Time to be able to get specific information about the month, day, and time of each order. 

3. To identify and explore the trend of order time in hours, I grouped them into hour-based time bins. 

4. In order to sort the months in the right order(Jan-Dec) I navigated to the database tab, selected month name column from the calendar table. 5. Select the modeling tab and then "Sort by Column" and select your month number column. Month name should now appear in the correct order.







**Data Modelling**

To establish relationships between the different tables and aid easy visualization, I created connections in the Modelling Tab between specific tables:

1. A connection was made between the "Orders id column in the Orders Details table" and the "Orders id column in the Orders table"

2. A connection was made between the "Pizza id column in the Orders Details table" and the "Pizza id column in the Pizzas table"

3. A connection was made between the "Pizza type column in the Pizza Type table" and the "Pizza type column in the Pizzas table"





**Business Intelligence Report:**



**Insights**



**1. What days and times do we tend to be busiest?**

Plato Pizza tends to be busiest on Fridays, Saturdays, and Thursdays, with peak periods between 12 to 1 pm and 5 to 6 pm.



**2. How many pizzas are we making during peak periods?**

A total of 23,817 pizzas are made during peak periods with 13,189 pizzas around 12 to 1 pm and 10,628 pizzas around 5 to 6 pm.



**3. What are our best and worst selling pizzas?**

Best selling pizzas

The best selling pizza is The Classic Deluxe Pizza (14,888 orders)



Worst selling pizzas

The worst selling pizza is The Brie Carre Pizza (490 orders)



**4. What's our average order value?**

Average order value (AOV) is a metric that showing the average amount spent whenever a customer places an order for pizza.

The average order value is $16.49



**5.How well are we utilizing our seating capacity? **

In a restaurant setting, capacity is the number of customers they may serve or the seats a venue may accommodate for good dining seating — capacity utilization rate measures how this potential space or outcome maximizes its full potential. Capacity Utilization rate= actual output/optimal output x100%.






**Other Key Insights**

**Key Performance Indicators**

1. A total of 49,574 orders were received during this period, generating $817,446 in Revenue.

2. The most ordered pizza category is The Classic Pizza, with 14,888 orders made, generating $219,754 in revenue.

3. The Pizza type that generated the highest revenue is The Thai Chicken Pizza ($43,434); the least revenue was generated from The Brie Carre Pizza ($11,588).

4. The month when the highest order of pizza was received is July (4392 orders, generating $72,519 in revenue) ; the least order of pizza was received in October (3883 orders, generating $63,997 in revenue).

5. In the first quarter, a total of 12K orders was made, generating $205K in revenue.

6. In the second quarter, a total of 13K orders was made, generating $208K in revenue.

7. In the third quarter, a total of 12K orders was made, generating $205K in revenue.

8. In the fourth quarter, a total of 12K orders was made, generating $199K in revenue.

9. The most ordered pizza size is the Large Pizza (18,956 orders, generating $375,254 in revenue); the least ordered pizza size is the XXL Pizza (28 orders, generating $1006 in revenue).



