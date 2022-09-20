1. Customer Accounts API.zip (RAML File)
2. apdev-accounts-diy-ws.jar (Export in AnypointStudio & deploy on cloudhub)
3. apdev-customer-accounts-diy-ws.jar (Export in AnypointStudio)
4. payroll-customer-accounts.jar(Export in AnypointStudio)

# apdev-accounts-diy-ws.jar

### **GET:**

`http://localhost:8080/api/accounts`

Headers:

    user_id (Mandatory)
    client_id (Mandatory)
    client_secret (Mandatory)

Query Parameters: 

    account_type
        enum : business
                personal
    account_name

### **GET:**

`http://localhost:8080/api/accounts/{ID}`

Headers:

    user_id (Mandatory)
    client_id (Mandatory)
    client_secret (Mandatory)

Uri Parameters: 

    id  (Mandatory)

### **POST:**

`http://localhost:8080/api/accounts`

Headers:

    user_id (Mandatory)
    client_id (Mandatory)
    client_secret (Mandatory)

Parameters: 

    account_type
        enum : business
                personal
    account_name


# apdev-customer-accounts-diy-ws.jar

### **GET:**

`http://localhost:8080/accounts`

Headers:

    user_id (Mandatory)


Query Parameters: 

    account_type    (Mandatory)
        enum : business
                personal
    account_name    (Mandatory)
    condition       (Mandatory)
        enum : AND
                OR

### **GET:**

`http://localhost:8080/transactions/{id}`

Uri Parameters: 

    id  (Mandatory)