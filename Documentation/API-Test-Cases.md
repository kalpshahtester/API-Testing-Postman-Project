# API Test Cases

This document contains the API test cases executed using Postman for the **API Testing Postman Project**.

The APIs tested in this project include:

* User Registration
* User Login
* Admin Login (Token Generation)
* Add Category
* View Category
* Delete Category

---

## Test Case Table

| TC ID | API Name          | Method | Endpoint     | Request Body / Params                   | Expected Result                                | Test Type  | Status |
| ----- | ----------------- | ------ | ------------ | --------------------------------------- | ---------------------------------------------- | ---------- | ------ |
| TC01  | User Registration | POST   | /userreg     | fname, lname, email, phno, pass, gender | User should be registered successfully         | Functional | Pass   |
| TC02  | User Login        | POST   | /userlogin   | email, pass                             | User authentication token should be generated  | Functional | Pass   |
| TC03  | Admin Login       | POST   | /alogin      | email, password                         | Admin authentication token should be generated | Security   | Pass   |
| TC04  | Add Category      | POST   | /addcategory | catname + admin auth token              | Category should be added successfully          | Functional | Pass   |
| TC05  | View Category     | GET    | /category    | admin auth token header                 | Category list should be returned               | Functional | Pass   |
| TC06  | Delete Category   | GET    | /deletecat   | id parameter + admin auth token         | Category should be deleted successfully        | Functional | Pass   |
| TC07  | Invalid Login     | POST   | /userlogin   | wrong email/password                    | System should reject login request             | Negative   | Pass   |

---

## Notes

* API requests were tested using **Postman**.
* Authentication is handled using **admin authentication token**.
* Test execution screenshots are available in the **Screenshots folder**.
