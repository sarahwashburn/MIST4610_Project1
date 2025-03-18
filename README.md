# MIST4610_Project1
Srini Street Eats  
Sp25_21482_Group6

## Team Members
Sarah Washburn [@sarahwashburn](https://github.com/sarahwashburn)  
Dylan Kiperman [@dylankiperman](https://github.com/dylankiperman)  
Nimay Patel [@nimaypatel](https://github.com/nimaypatel)  
Aay Bel Pa Pa Minn [@aaybelpapaminn](https://github.com/aaybelpapaminn)  
Marshall Massey [@MMassey25](https://github.com/MMassey25)

## Scenario Description
The task at hand is to create a data model and build a relational database to represent the basis of an online food delivery service in the United States! Our data model consists of 10 separate entities, with the orders entity being the central focus of our model. The orders that customers place allow us to connect with the restaurants our drivers pick up from, where the destination of our orders are, and the customers we deliver to, along with any complaints or problems they have with our service. Our main goal is to accurately describe our day-to-day activities and the relationships that happens within our business. To fully show the detail of these relationships, there are a multitude of attributes within each entity filled with general, sample data. Through the use of functional queries, we are able to see where our company flourishes and where it lacks perfection. These queries will show us where we need to improve and how we can be the best possible service for Srini's Steets Eats' customers!


## Data Model
Our online food delivery data model is made up of 10 unique entities that show the processes of our company. Each entity has unique information that allows our company to know who we are delivering to, how we are delivering to them, what we are delivering to them, or even the complaints that our customers have with our services. The ten entities that make up our data model include: Products, OrderProducts, Orders, Restaurants, Reviews, Customers, Memberships, Drivers, SupportTickets, and finally CustomerServiceEmployees.

Products- Products consist of certain details like productID, productName, and menuCategory. The Products entity gives multiple examples of products that people order and what type of food it is. Products have a one-to-many identifying relationship from Products to OrderProducts. Another relationship that exists is a one-to-many non-identifying relationship from Restaurants to Products. Basically restaurants have many products, but these unique products only belong to one, specific restaurant. 

OrderProducts- OrderProducts is an associative entity between Products and Orders. OrderProducts is useful for showing sales management and inventory between the products we deliver and the orders that include those items. Product quantity and product price are examples of data that is collected within this entity. This helps with keeping up with the food that is ordered online and the price of the food that is being ordered.

Orders- The center of our data model begins with the Orders entity. This consists of all the details associated with the delivery of the food. Whether it be a PK of orderID, or 2 FK of customerID and driverID, we can know which customer the food is being delivered to and which driver is dropping the food off. Branching off of the Order entity is OrderProducts, Drivers, SupportTickets, and Customers. There is a one-to-many identifying relationship from Orders to OrderDetails, a one-to-many non-identifying relationship from Drivers and Customers to Orders, and finally a one-to-one non-identifying relationship between Orders and SupportTickets. 

Basically these relationships mean that an order can have many order details but order details can only belong to one order. A customer can have many orders, but an order can only belong to one customer. A driver can deliver many orders, but a singular order can only belong to one driver. Finally, Orders can only have one support ticket and a unique support ticket can only belong to one order.

Restaurants- Restaurants consist of all the data that our company needs to pick up food from the restaurants and what food is ordered. The data collected includes the restaurant name, phone number, city and the unique ID associated with each restaurant. For example if we get a certain product/food, we will be able to see which restaurant it belongs to and how to contact the restaurant to order the customer’s food. The Restaurant entity has a one-to-many non-identifying relationship from Restaurant to both Products and Reviews. This means that a restaurant can have a plethora of reviews about them, but each unique review only belongs to one restaurant. 

Reviews- Reviews are essential to keeping up with the restaurants we deliver to and the customers that submit them. We are able to see data including the review, a description of the review, and the date of when the review was submitted. Using this data we can see which Customers seem upset with our service and/or the restaurants they are complaining about. There is a one-to-many non-identifying relationship from both Restaurants and Customers to reviews. In simplistic terms, Customers can submit multiple reviews, but a unique review can only belong to one customer. 

Customers- Customers are also considered one of the backbones of our data model and our company as a whole. The Customers entity gives us all the information we need to know where to deliver the food, who is ordering the food, and how the customer is paying for our service. Each customer is also given a unique customerID to ensure that we don’t confuse two customers with similar names. The Customers entity has a one-to-many non-identifying relationship from Customers to Reviews and Orders, while also having a one-to-many non-identifying relationship from Memberships to Customers. This means that a membership type can belong to many customers, but a customer can only have one membership. 

Memberships- The Memberships entity shows our company’s types of memberships, the cost of the membership, and the benefits that are associated with each membership. Memberships range from a variety of costs and provide unique benefits associated with each type. Memberships are essential to understanding our customers and provide us with a way to benefit customers who have been loyal to us. The Memberships entity has a one-to-many non-identifying relationship from Memberships to Customers.  

Drivers- The Drivers entity shows the data associated with our employees who provide the services for our customers. They are one of the two entities associated with our company and the workers that help make us successful. Some information stored about our drivers may be the car they drive, the name of our driver, and other unique details about their car. Without the driver's entity, we would not be able to execute our online delivery service, so it is truly essential to the basis of our business. The Drivers entity has a one-to-many non-identifying relationship from Drivers to Orders. 

SupportTickets- The SupportTickets interview is a way for our customers to reach out to our company about the service we are providing. This feedback could include an issue that the customer had with their order, when the feedback was submitted, a description of the feedback, the order associated with the ticket, and even the employee that helped resolve this complaint. The SupportTickets entity has a one-to-one non-identifying relationship between Orders and SupportTickets. There is also a one-to-many non-identifying relationship from CustomerServiceEmployees to SupportTickets. This means that an employee can help with multiple support tickets, but a specific support ticket is only resolved by one employee.

CustomerServiceEmployees- Finally the CustomerServiceEmployees entity shows who helps with the support tickets submitted by customers. The data included within this entity includes the first and last name of our employee, the title of the employee as well as where our employee is located. This makes up the second entity that provides information about the employees that work for our company. This entity has a one-to-many non-identifying relationship from CustomerServiceEmployees to SupportTickets. 

![Final Diagram](https://github.com/user-attachments/assets/9bb0f0cf-25b3-4b7b-8a48-768f40eea49a)


## Data Dictionary
<img width="636" alt="image" src="https://github.com/user-attachments/assets/ad8d29c4-1d06-4edd-929a-5f4e128ccc72" />
<img width="638" alt="image" src="https://github.com/user-attachments/assets/5c7fff9e-fd8d-442e-a425-72773937dec5" />
<img width="639" alt="image" src="https://github.com/user-attachments/assets/bfe8487c-280c-498c-81b1-88d642cbab47" />
<img width="641" alt="image" src="https://github.com/user-attachments/assets/62e700b7-4c90-4fd7-b37f-1824fd630220" />  
<img width="721" alt="Screenshot 2025-03-18 at 2 19 52 PM" src="https://github.com/user-attachments/assets/0fa6c3a3-842d-4d9d-bb7c-4ef57bcf25a1" />

![Membership Table](https://github.com/user-attachments/assets/fb7ee9c4-def2-427d-91df-231b1524e6c0)
<img width="716" alt="Screenshot 2025-03-18 at 1 53 50 PM" src="https://github.com/user-attachments/assets/017bf23c-e742-4db1-b6d9-ebb275933a70" />
<img width="648" alt="Screenshot 2025-03-18 at 1 54 20 PM" src="https://github.com/user-attachments/assets/5ee1e15d-aea1-4caa-91fb-ce54b44412c1" />
<img width="688" alt="Screenshot 2025-03-18 at 1 55 37 PM" src="https://github.com/user-attachments/assets/c7d4f044-dfc1-492e-a8d6-7079d9b859ac" />
<img width="701" alt="Screenshot 2025-03-18 at 1 56 26 PM" src="https://github.com/user-attachments/assets/75bcd677-6085-4a00-a86d-fe45fb09fc61" />



## Ten Queries


1. Query 1 lists the products, their restaurants, and the total number of times customers have ordered said products. This query lists those products whose total number of quantity ordered is greater than the average quantity ordered among all products.

![Query 1 gp1](https://github.com/user-attachments/assets/0c4e0d2f-1022-4fd4-9f85-4ae0d41b7186)

Query 1 allows managers to see what products are popular and which restaurants they come from. This is important so they can decide what type of products and restaurants to pursue if they want to expand. Additionally, they can use this information to give coupons or freebies of certain products to get more customers to purchase them.


2. Query 2 lists the drivers with the highest number of orders delivered. It lists the driver’s name and the number of orders delivered.

![Query 2 gp1](https://github.com/user-attachments/assets/25ebdf49-e7b4-4d47-8435-6f37d35d5afa)

Query 2 will allow managers to determine which drivers dedicate a lot of time to the app and who is the most productive. Through this, they can give a bonus to those drivers who are doing exceptionally well, thus boosting morale and incentivizing the drivers to keep driving for them. 

3.Query 3 lists John Smith's customer support tickets that were "Quality Issues" and which restaurant they corresponded to.

<img width="810" alt="Screenshot 2025-03-18 at 2 23 20 PM" src="https://github.com/user-attachments/assets/e7115156-163b-4314-a2d6-d4638ba67d53" />

Query 3 focuses in on the work that the customer support employee, John Smith does, pertaining specific support tickets that he dealt with. This query emits the employee first and last name, which will always be John Smith in this case, as well as the name of the restaurant, the ID of the support ticket to easily refer back to the specific instance, and the description of the issue. These are all "Quality Issues" and REGEXP was used to narrow the query down to this unique issue. These unique insights will allow Srini's Eats to pinpoint specific situations where the restaurants did not provide adequate quality in their food. In this case, Srini's Eats can further investigate the details of the quality issue, like why it happened and ways the restaurant can improve to please their customers. 

4. Query 4 organizes Srini's Eats' lowest rated restaurants with a rating out of 5.

<img width="945" alt="Screenshot 2025-03-18 at 2 24 13 PM" src="https://github.com/user-attachments/assets/4b18908c-401d-4170-a7d2-0459347c40c8" />

Query 4 will help the Srini's Eats service analyze which restaurants are the worst performing. This will help us, as administrators, decide which restaurants we want to retain as a client and which one's we should abandon. Displaying restaurantID, the name of the restaurant, and an average of the reviewRating in ascending order, Query 4 was succesfully able to identify the restaurans that are receiving the worst reviews, hence performing the worst. Windy City Eats and Bayou Bites each have an average rating of 3.00/5.00, while Gourmet Heaven and Sunset Bistro both have ratings of 4.5/5.00. From a managerial perspective, Srini's Eats can further investigate the poor performance of the lower rated restaurants and see why they are receiving bad reviews. From there, Srini's Eats can choose to advise the restaurant on better practices, or eliminate them from providing their services.

5. Query 5 shows which driver has the worst reviews associated with a support ticket under the category of "delivery issue"

<img width="445" alt="image" src="https://github.com/user-attachments/assets/bbdaba6d-c042-4588-9e89-b5d78d306520" />

This query shows which driver has the worst reviews associated with a support ticket under the category of "delivery issue". The actual query lists the driver name, as well as their review rating only if they were listed on a support ticket relating to a delivery issue. This allows my company to see which drivers are struggling and are receiving complaints from our customers. This can let us know if we need to resolve an issue with this driver and if they might not be the best fit for our company. As shown in the results, David Brown received the lowest rating, so our company will need to talk with him about these complaints.

6. Query 6 allows our company to see what is the most frequently ordered product from every restaurant by customers not having a premium subscription

<img width="653" alt="image" src="https://github.com/user-attachments/assets/ab8d4056-996c-4094-8b0e-4e1021de9cec" />

Through the use of this query, our company is able to see what is the most frequently ordered product from every restaurant by customers not having a premium subscription. In the query we are actually able to see the list of products that are being ordered by people without a premium subscription, and the amount of times it has been ordered. As seen in the results the most frequently ordered item is Pineapple Sorbet, with an amount of 5 times. Using this information we can see which products we need to promote and do not need to promote to our basic customers. I only chose items ordered over 2 times because an item being ordered twice is not considered statistically significant when looking at how many times other items were ordered. Maybe if we promote the highest ordered products more, then we can get more customers to upgrade their membership in order to receive more benefits associated with these items. For example: if a customer upgrades their subscription then they will get a pineapple sorbet bogo deal on their next purchase.

7. Query 7 lists the top three cities and their total revenue that are the highest profits across all cities.
   
![image](https://github.com/user-attachments/assets/8376b9c9-6b27-49dc-8aa8-3bb9a780ca57)

As a manager of Srini Street Eats, one needs to be aware of their success in relation to their clients’ geographic locations to determine future resource allocation. Based on the profit, one can strategize on how to allocate resources like drivers, vehicles, and customer service employees in accordance with their future goals. Since Miami produced the highest total revenue of $356, one can first analyze its geographical and demographic advantages through customers, their reviews, and order products. A restaurant’s location can influence order products because of the different population, culture, and climate. Then, one can observe how drivers and customer service employees were dispatched to maximise customer satisfaction and hence restaurant success in Miami. Finally, one can implement a similar strategy towards cities near Miami and/or cities with similar geographical and demographic structures. The same is to be applied for Chicago and New York. 

8. Query 8 lists the percentage of orders in each city that are associated with restaurants that have at least one review below 3 stars.

![image](https://github.com/user-attachments/assets/dc0573ff-8475-4372-9339-6475342edb0f)

As a manager of Srini Street Eats, one needs to be aware of their clients’ success to determine whether the current resource allocation provides maximum benefit for the company’s goals. Since 42.5% of the orders have review ratings below 3, there needs to be slight improvements. Firstly, one has to determine the restaurant cities and the restaurant names that contribute to the 42.5%. Secondly, their review descriptions need to be sourced out to determine the percentage of problems that were caused by Srini Street Eats. If it is high, the contract between Srini Street Eats and the restaurant may be continued. If it is low, the contract needs to be analyzed and re-considered as the problems lie with the restaurant, and Srini Street Eats have little to no managerial control over the restaurant. 

9. Query 9 tells us which customer gave the highest rating to any select restaurant. This customer will be rewarded with a $5 off coupon on their next order from that restaurant

![image](https://github.com/user-attachments/assets/b379e75b-ce00-4813-af14-c9cd7df37d04)

Identifying the customer who gave the highest review to a specific restaurant helps in rewarding loyal customers and encouraging positive feedback. This query finds the top reviewer and offers them a $5 off coupon for their next order. By recognizing high ratings, the platform boosts customer satisfaction and strengthens restaurant relationships.

10. Query 10 tells us which customer has spent the highest average amount of money compared to the rest of the customers who have ordered from all restaurants

<img width="981" alt="image" src="https://github.com/user-attachments/assets/da70aa8a-f1bf-4dc6-aa93-526a3880623d" />

This query identifies the customer who spends the most on average per order by calculating the total cost, including both delivery and product prices, grouping by customer, and finding the highest spender. Understanding top spenders helps businesses reward loyal customers, build stronger relationships, and boost long-term sales by encouraging repeat orders and brand loyalty.


## Database Information
Our group database is under ns_Sp25_21482_Group6
We have used the bookarking storage method. Each query can be called under TP_Qx (x is to be replaced with the query number).
