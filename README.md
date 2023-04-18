# Case-Study - Pizza Runner

![Logo](https://user-images.githubusercontent.com/130475600/232837411-e3e502cc-52e8-4cb5-a857-d5514cad6fb3.PNG)

# Problem Statement:
Did you know that over 115 million kilograms of pizza is consumed daily worldwide??? (Well according to Wikipedia anyway…)

Danny was scrolling through his Instagram feed when something really caught his eye - “80s Retro Styling and Pizza Is The Future!”

Danny was sold on the idea, but he knew that pizza alone was not going to help him get seed funding to expand his new Pizza Empire - so he had one more genius idea to combine with it - he was going to Uberize it - and so Pizza Runner was launched!

Danny started by recruiting “runners” to deliver fresh pizza from Pizza Runner Headquarters (otherwise known as Danny’s house) and also maxed out his credit card to pay freelance developers to build a mobile app to accept orders from customers.

# Entity Relationship Diagram:

![diagram](https://user-images.githubusercontent.com/130475600/232838088-fd53f3fc-b1ae-4720-b689-7f3a9bf8604b.PNG)

# Tables:
Table 1: runners
The runners table shows the registration_date for each new runner

![t1](https://user-images.githubusercontent.com/130475600/232838361-15041eb6-8a0d-4a90-b780-7e905f2ded19.PNG)

Table 2: customer_orders
Customer pizza orders are captured in the customer_orders table with 1 row for each individual pizza that is part of the order.

The pizza_id relates to the type of pizza which was ordered whilst the exclusions are the ingredient_id values which should be removed from the pizza and the extras are the ingredient_id values which need to be added to the pizza.

Note that customers can order multiple pizzas in a single order with varying exclusions and extras values even if the pizza is the same type!
The exclusions and extras columns will need to be cleaned up before using them in

![t2](https://user-images.githubusercontent.com/130475600/232838746-dbbc22a5-ac75-4297-a896-12cb7cdcc237.PNG)

Table 3: runner_orders
After each orders are received through the system - they are assigned to a runner - however not all orders are fully completed and can be cancelled by the restaurant or the customer.

The pickup_time is the timestamp at which the runner arrives at the Pizza Runner headquarters to pick up the freshly cooked pizzas. The distance and duration fields are related to how far and long the runner had to travel to deliver the order to the respective customer.

There are some known data issues with this table so be careful when using this in your queries - make sure to check the data types for each column in the schema SQL!

![t3](https://user-images.githubusercontent.com/130475600/232838949-9fbb8c19-b0a2-4c98-a510-f7a2c8751fc9.PNG)

Table 4: pizza_names
At the moment - Pizza Runner only has 2 pizzas available the Meat Lovers or Vegetarian!

![t4](https://user-images.githubusercontent.com/130475600/232839111-473df729-f6af-4a78-a10f-d6cc4d7af62d.PNG)

Table 5: pizza_recipes
Each pizza_id has a standard set of toppings which are used as part of the pizza recipe.

![t5](https://user-images.githubusercontent.com/130475600/232839256-9e78bdc2-54e7-49d9-9b54-f76424986481.PNG)

Table 6: pizza_toppings
This table contains all of the topping_name values with their corresponding topping_id value

![t6](https://user-images.githubusercontent.com/130475600/232839369-d2022c5b-ab1c-4ccd-9617-f233b5f0b08e.PNG)



