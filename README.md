# Domain-Driven Design Example C#

## Api

To keep things simple I have created in memory repository with few saved items. To start using simply download, open solution and run.

### Customer

Customer already exists (John Smith, ID: 5D5020DA-47DF-4C82-A722-C8DEAF06AE23).

But if you would like to add my customers here are urls that you can call:

```
api/customer/add?FirstName=john2&LastName=smith2&Email=john2.smith2@microsoft.com

api/customer/Getbyid/5D5020DA-47DF-4C82-A722-C8DEAF06AE23

api/customer/IsEmailAvailable?email=smith.john@microsoft.com

api/customer/RemoveById/5D5020DA-47DF-4C82-A722-C8DEAF06AE23

api/customer/update?id=5D5020DA-47DF-4C82-A722-C8DEAF06AE23&Email=smith.john@microsoft.com
```

### Product

Product already exists (iPhone, ID: 65D03D7E-E41A-49BC-8680-DC942BABD10A).

But if you would like to add more products here are urls that you can call:

```
api/product/add?name=iPhone5&quantity=6&cost=422&productcodeid=B2773EBF-CD0C-4F31-83E2-691973E32531

api/product/get/65D03D7E-E41A-49BC-8680-DC942BABD10A
```

### Cart
Customer and product already exists, so feel free just to call these urls:
```
/api/cart/add?customerid=5D5020DA-47DF-4C82-A722-C8DEAF06AE23&productid=65D03D7E-E41A-49BC-8680-DC942BABD10A&quantity=1

/api/cart/getbyid?customerid=5D5020DA-47DF-4C82-A722-C8DEAF06AE23

/api/cart/remove?customerid=5D5020DA-47DF-4C82-A722-C8DEAF06AE23&productid=65d03d7e-e41a-49bc-8680-dc942babd10a&Quantity=1

/api/cart/checkout?customerid=5D5020DA-47DF-4C82-A722-C8DEAF06AE23
```