# CS3SY26_ProjectProposal by Rb13, Rb14, Rb19

### Project Title or Name of the Application	: BonChon Order Management System
### Section			   	      : Rubidium
### Group Members			    : Amalia Lapira, Michaela Laqui, Andrey Obial
### Date (Proposal Date)  : Nov 5, 2026
### Project Description:

The BonChon Order Management System designed to streamline the delivery of orders from BonChon. The application will allow customers to browse the restaurant’s menu, modify their orders, and confirm their purchases. Once an order is confirmed, the application calculates the total cost, records the order, and assigns it a delivery rider. Restaurant staff may then provide real-time updates on food preparation. This reduces long lines in the restaurant and brings convenience to those who are unable to order in person. Through this digital platform, customers can easily access BonChon’s delicious dishes in just a few clicks.

**Classes**

**1) Food**

_Attributes:_

name - name of food item

price - price of food item

quantity - quantity of item selected

status - availability (available/unavailable)

_Methods:_

display() - displays the item's information

upd_qty() - updates the quantity of selected item

upd_status() - changes item's availability

**2) Cart**

_Attributes:_

items - list of food items added to the cart

quantity - total quantity of items in the cart

total_price - total cost of all items in the cart

_Methods:_

add_item() - adds a food item to the cart

remove_item() - removes a food item from the cart

upd_qty() - updates the quantity of a selected item

calc_total() - calculates the total price of all items in the cart

display_cart() - displays all items added to the cart

**3) Customer**

_Attributes:_

name - name of the customer

address - customer's delivery address

cart - cart containing the customer's selected food items

_Methods:_

browse_menu() - displays the available food items

add_to_cart() - adds a selected food item to the cart

place_order() - places an order using the items in the cart

confirm_order() - confirms the customer's purchase

**4) DeliveryRider**

_Attributes:_

name - name of the delivery rider

address - delivery address assigned to the rider

food - food items assigned for delivery

status - availability of the rider (available/unavailable)

_Methods:_

receive_order() - receives an order assigned by the restaurant

receive_address() - receives the customer's delivery address

deliver_order() - delivers the food to the customer

upd_status() - updates the rider's availability or delivery status

**5) RestaurantStaff**

_Attributes:_

name - name of the restaurant staff member

assigned_orders - list of orders assigned to the staff member

status - current status of the food preparation

_Methods:_

receive_order() - receives confirmed customer orders

cook_order() - prepares the customer's food order

package_order() - packages the prepared food

upd_status() - updates the preparation status of an order

### Class Diagram:

<img width="189" height="323" alt="image" src="https://github.com/user-attachments/assets/6426b3cd-0c0a-450d-9efb-8c098b8b1828" />

### Goals:

Our project aims to improve the overall efficiency and convenience of food ordering and delivery. By providing a more organized system for handling transactions, we hope to minimize human errors, reduce unnecessary delays, and improve coordination among the individuals involved. In the long run, we expect this project to contribute to a smoother and more reliable customer experience while helping restaurant operations become more systematic and manageable.

**Objective 1:**
Develop an interactive system that allows users to browse available food items on the menu, including their descriptions, prices, and possible combinations for orders.

**Objective 2:** 
Implement a cart management system that will be able to record, track, and calculate customers’ orders. Users may still be able to add, remove, and modify items before confirming their purchases.

**Objective 3:** 
Integrate an order monitoring feature that allows restaurant staff to update the preparation status of confirmed orders to keep customers informed.

**Objective 4:** 
Develop a delivery management system that assigns available riders to confirmed orders and allows delivery statuses to be updated as well.
