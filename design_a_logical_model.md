# Bookstore Logical Model

## ERD Description

This is the logical model design for a small bookstore. The key entities include:
- Employee
- Customer
- Book
- Order
- Sales
- Date
- Customer Address
- Shift

Relationships are as follows:
- Customer to Order: 1 to many
- Order to Employee: Many to 1
- Order to Book: Many to Many
- Sales to Employee: Many to 1
- Sales to Date: Many to 1
- Order to Date: Many to 1
- Customer to Customer Address: 1 to 1
- Employee to Shift: 1 to 1

## ERD Diagrams

### Overall Bookstore ERD

![Bookstore ERD: Address Type1]![Type 1 Diagram](https://github.com/user-attachments/assets/633326c5-2b34-49d0-ad60-f1d7d43044e6)

![Bookstore ERD: Address Type2]![Type 2 Diagram](https://github.com/user-attachments/assets/0100058b-2618-42c9-a141-dd3e72802a38)


### Shift Model for Employees

![Shift ERD]![Shift Model Diagram](https://github.com/user-attachments/assets/9227d0a9-bc10-40e1-af4b-20bb08bb16ef)



### Question 3: Customer Addresses
- **Type 1** is best practice and what I would move forward with as the owner of the bookstore. No privacy issues, no history is maintained that isn't current.
- **Type 2** maintains personal history information and (dependant on the province/state/country) has privacy issues.  Breach of privacy is illegal in majority of Canada, again, dependant on the type of infomration.

### Question 4: Comparison with AdventureWorks
In comparison, I would definitely add the following: 
Sales: 
    - Territory/Region
    - Quota
    - Sales Last Year
    - Unit price
    - Discount Price
Production: 
    - Product Review
    - Inventory
    - Product Price History

and likely many more.
