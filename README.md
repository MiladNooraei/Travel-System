
# Travel System

Created a Travel System using simple python GUI(tkinter) and DataBase(MySQL)

## Description

### Travels
The platform contains four types of travels based on the vehicle:
Train, Bus, Ship and Airplane where air travel can be domestic or abroad.
Each travel has some info:
- Date and time
- Type of vehicle
- Price
- Number of available seats

### User Roles

This project contains three types of users with different roles: 
- passenger
- travel agency manager 
- super admin
Any user should register with one-time password (OTP). 
OTP should have expiration time and it shouldn’t be accepted after the
expiration time which is 30 seconds. User's account verification only occur after the
successful completion of the OTP process. Until the OTP is validated within
the specified expiration time, the user's account remains unverified
and inaccessible. While the account is verified, user can log in using its
passwords.
Users are provided with the flexibility to log in to their accounts using
either their registered phone number or email address. The system
supports both login methods, allowing users to choose their preferred option
during the authentication process.
Database security is very important and many famous databases
get leaked every day, so we keep users’ passwords
safe by saving hash of password in DataBase!

### Passenger

- Each passenger have their own panel with personal information.
- They are able to reserve tickets, order them and pay for them and eventually track orders’ status.
- They are able to apply discounts to their orders with discount codes. Discount codes have a maximum limit of price.
- Passengers can search for tickets with different search parameters and filters such as rating, price and etc.
- Passengers who have bought tickets, are be able to rate the previous travels.

### Travel Agency Manager

- Managers are able to add new travels.
- Managers can filter travels that their agency involved using different filtering parameters such as rating, price, time and etc.
- They can receive needed stats at once, like: Bestselling travels, highest income through the year based on time, highest rating, most popular destination and etc.
- Managers are able to retrieve information on the top 5 customers with the highest total paid price for travels in a specific month. Include their full name, contact information (email or phone number), total paid price, number of destinations they traveled to in that month, and the name of the city they visited the most.

    -> They also can see plots of above information.

### Support System

To enhance customer and travel agency manager interaction, an online support system will be implemented on the website. Super admins have the ability to engage in chat conversations with customers and travel agency managers.
Key features of the support system include:
- Ticket Creation: Customers and travel agency managers should have the ability to create support tickets. These tickets serve as a means of communication with the support team. Users can submit their queries, concerns, or requests through the ticket creation process.
- Messaging: Users are able to send and receive messages within the support system. Each message is associated with a date and time and seen status, ensuring a clear timeline of the conversation. 

## Implementation

This project is implemented using Python and its simple GUI(tkinter). To connect the code to DataBase(MySQL), mysql.connector is used.

## Installation

To run this project you need to install : 
- [Python](https://www.python.org/)
- [MySQL](https://www.mysql.com/)

And also you need to install folowing packages in python
(for Windows users, copy command in CMD) :
1. hashlib
```bash
pip install hashlib
```
2. pandas
```bash
pip install pandas
```
3. tkinter
```bash
pip install tkinter
```
4. seaborn
```bash
pip install seaborn
```
5. mysql.connector
```bash
pip install mysql-connector-python
```
6. pandastable
```bash
pip install pandastable
```
7. matplotlib
```bash
pip install matplotlib
```
