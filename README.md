# Synthetic_data

### We need synthetic data (datasets) for user privacy and testing.

## The datasets provide a comprehensive overview of hypermarket sales, allowing for analysis and exploration of sales performance, customer preferences and behavior, the number of sales and profits.

### We will have two source datasets
The first dataset contains  information about sales on the European market.
The second  dataset contains information about sales on the Asian market.

But both will contain following information:

#### Product Information:
    - ProductID: product unique identifier (will determine NK)
    - ProductName: short product name
    - ProductDescription: Short product name.
    - ProductCategory: determine the main group of product classification 
      (e.g. Food, Electronics, etc)
    - ProductSubcategory: more detailed description (e.g. category Food will 
      contain: Fruits, Cheese, etc)
    - Brand: company which produced a product
    - SupplierID: unique supplier number
    - Supplier: distributor company`s name

#### Sales Information:
    - UnitPrice: The actual selling price of the item.
    - Quantity: The number of units sold.

#### Customer Information:
    - CustomerID: Unique customer identifier.
    - CustomerName
    - CustomerSurname
    - CustomerBirthday
    - CustomerGender: male/female
    - CustomerPhone
    - CustomerEmail
    - Customer income: annual income for a particular customer 
      (will be necessary in analyzing customer`s patterns)
    - CustomerMaritalStatus: single/married/divorced.

#### Payment information:
	- InvoiceNo: Number of the invoice.
	- InvoiceDate: Data of transaction when customer paid.
    - Invoice_line: one line in an invoice which corresponds one product

#### Stores information: 
	- StockID: unique identifier
    - StockCode - unique number of the outlet
    - StoreAddress: district, street, building
    - StoreCountry
    - StoreRegion
    - StoreCity
    - StoreType: online/direct store


#### DiscountPrograms information:
	- DiscountID: unique program identifier
  	- DiscountName: brief description   
    - DiscountDescription: full description  
    - Discount%: discount amount, percentage
    - DiscountType: unlimited, temporal, promocode, 1 month, etc.  
    - DiscountLimit: e.g. discount is available on the particular days, hours, etc.  
    - DiscountAdd: additional privileges

#### Delivery information:
    - DeliveryID  
    - DeliveryType: home standart, home express, pickpoint 
    - DeliveryCompany: name of transport company   
    - CourierID: unique identifier  
    - CourierName: full name 
    - CourierPhone 

#### Metrics (information that appears in the invoice):
	- LineCost: total amount in dollars per one product in one particular 
      line in one invoice
	- TotalQuantity: the total amount of all products in one invoice
	- TotalAmount: the total amount paid in dollars for all products in one invoice 
    - TotalAmountAfterDiscount: the total amount paid in dollars for all products 
      in one invoice after subtracting discount (if it is)
