# API Test Cases

| TC ID | API Name          | Method | Endpoint     | Request Body / Params                   | Expected Result               | Status |
| ----- | ----------------- | ------ | ------------ | --------------------------------------- | ----------------------------- | ------ |
| TC01  | User Registration | POST   | /userreg     | fname, lname, email, phno, pass, gender | User registered successfully  | Pass   |
| TC02  | User Login        | POST   | /userlogin   | email, pass                             | User auth token generated     | Pass   |
| TC03  | Admin Login       | POST   | /alogin      | email, password                         | Admin token generated         | Pass   |
| TC04  | Add Category      | POST   | /addcategory | catname                                 | Category added successfully   | Pass   |
| TC05  | View Category     | GET    | /category    | Admin token header                      | Category list displayed       | Pass   |
| TC06  | Delete Category   | GET    | /deletecat   | id parameter                            | Category deleted successfully | Pass   |
| TC07  | Invalid Login     | POST   | /userlogin   | wrong email/password                    | Login should fail             | Pass   |
