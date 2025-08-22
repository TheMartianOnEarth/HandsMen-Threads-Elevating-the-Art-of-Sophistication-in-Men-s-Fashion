# HandsMen-Threads-Elevating-the-Art-of-Sophistication-in-Men-s-Fashion
A hands-on project for Smartbridge's 2025 Salesforce Developer Virtual Internship Program.

My Demo Link: https://drive.google.com/file/d/1xNAJYAXx8Ldyn7wZImxmhg176xzwFztM/view?usp=sharing

HandsMen Threads, a premium men's fashion brand, aims to leverage Salesforce to streamline operations, enhance customer experience, and optimize inventory management. This project focuses on implementing Salesforce CRM to manage customer orders, track inventory, automate marketing campaigns, and provide seamless customer service.

1. Salesforce CRM Implementation
2. Process Automation & Workflows
3. Apex & Trigger Implementations
4. Batch Jobs & Scheduled Processes
5. Data Security & Access Control

**DATA MANAGEMENT**
**A. Custom objects**
- HandsMen Customer
- HandsMen Product
- HandsMen Order
- Inventory
- Marketing Campaign

**B. Custom fields**
- HandsMen Customer
    1. Email
    2. First name
    3. Full name
    4. Last name
    5. Loyalty points
    6. Loyalty status
    7. Phone
    8. Total Purchases
- HandsMen Product
    1. Order (Lookup relationship to HandsMen Order)
    2. Price
    3. SKU
    4. Stock quantity
- HandsMen Order
    1. Customer (Lookup relationship to HandsMen customer)
    2. Product
    3. Quantity
    4. Status
    5. Total Amount
- Inventory
    1. Product (Master-Detail with HandsMen Product)
    2. Stock quantity
    3. Stock status
    4. Warehouse
- Marketing Campaign
    1. End date
    2. HandsMen Customer (Lookup to HandsMen customer)
    3. Start date
 
**DATA CONFIGURATION**
Validation Rules:
1. Total Amount in HandsMen Order - prevents saving a record if Total_Amount__c is zero or negative
2. Stock Quantity in Inventory - prevents saving a record if Stock_Quantity__c is zero or negative
3. Email in HandsMen Customer - prevents saving a record if the Email field does not contain “@gmail.com”

