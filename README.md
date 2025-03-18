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
![Final Diagram](https://github.com/user-attachments/assets/9bb0f0cf-25b3-4b7b-8a48-768f40eea49a)


## Data Dictionary
<img width="636" alt="image" src="https://github.com/user-attachments/assets/ad8d29c4-1d06-4edd-929a-5f4e128ccc72" />
<img width="638" alt="image" src="https://github.com/user-attachments/assets/5c7fff9e-fd8d-442e-a425-72773937dec5" />
<img width="639" alt="image" src="https://github.com/user-attachments/assets/bfe8487c-280c-498c-81b1-88d642cbab47" />
<img width="641" alt="image" src="https://github.com/user-attachments/assets/62e700b7-4c90-4fd7-b37f-1824fd630220" />  

![Customer Service Employee Table](https://github.com/user-attachments/assets/f65a870d-8197-45d1-9cd2-cc70393cff8e)
![Membership Table](https://github.com/user-attachments/assets/fb7ee9c4-def2-427d-91df-231b1524e6c0)



## Ten Queries


1. Query 1 lists the products, their restaurants, and the total number of times customers have ordered said products. This query lists those products whose total number of quantity ordered is greater than the average quantity ordered among all products.

![Query 1 gp1](https://github.com/user-attachments/assets/0c4e0d2f-1022-4fd4-9f85-4ae0d41b7186)

Query 1 allows managers to see what products are popular and which restaurants they come from. This is important so they can decide what type of products and restaurants to pursue if they want to expand. Additionally, they can use this information to give coupons or freebies of certain products to get more customers to purchase them.


2. Query 2 lists the drivers with the highest number of orders delivered. It lists the driver’s name and the number of orders delivered.

![Query 2 gp1](https://github.com/user-attachments/assets/25ebdf49-e7b4-4d47-8435-6f37d35d5afa)

Query 2 will allow managers to determine which drivers dedicate a lot of time to the app and who is the most productive. Through this, they can give a bonus to those drivers who are doing exceptionally well, thus boosting morale and incentivizing the drivers to keep driving for them. 

3. Query 3 organizes Srini's Eats' lowest rated restaurants with a rating out of 5.

5. Query 5 counts the number of John Smith's customer support tickets that were "Quality Issues".

7. Query 7 lists the top three cities and their total revenue that are the highest profits across all cities.
   
![image](https://github.com/user-attachments/assets/8376b9c9-6b27-49dc-8aa8-3bb9a780ca57)

As a manager of Srini Street Eats, one needs to be aware of their success in relation to their clients’ geographic locations to determine future resource allocation. Based on the profit, one can strategize on how to allocate resources like drivers, vehicles, and customer service employees in accordance with their future goals. Since Miami produced the highest total revenue of $356, one can first analyze its geographical and demographic advantages through customers, their reviews, and order products. A restaurant’s location can influence order products because of the different population, culture, and climate. Then, one can observe how drivers and customer service employees were dispatched to maximise customer satisfaction and hence restaurant success in Miami. Finally, one can implement a similar strategy towards cities near Miami and/or cities with similar geographical and demographic structures. The same is to be applied for Chicago and New York. 

8. Query 8 lists the percentage of orders in each city that are associated with restaurants that have at least one review below 3 stars.

![image](https://github.com/user-attachments/assets/dc0573ff-8475-4372-9339-6475342edb0f)

As a manager of Srini Street Eats, one needs to be aware of their clients’ success to determine whether the current resource allocation provides maximum benefit for the company’s goals. Since 42.5% of the orders have review ratings below 3, there needs to be slight improvements. Firstly, one has to determine the restaurant cities and the restaurant names that contribute to the 42.5%. Secondly, their review descriptions need to be sourced out to determine the percentage of problems that were caused by Srini Street Eats. If it is high, the contract between Srini Street Eats and the restaurant may be continued. If it is low, the contract needs to be analyzed and re-considered as the problems lie with the restaurant, and Srini Street Eats have little to no managerial control over the restaurant. 



## Database Information
Our group database is under ns_Sp25_21482_Group6
We have used the bookarking storage method. Each query can be called under TP_Qx (x is to be replaced with the query number).
