# Test Cases – SauceDemo 

## 1.Login Functionality

| Test ID | Test Scenario | Preconditions  | Test Steps | Expected Results | Actual Result | Status |
|-|-|-|-|-|-|-|
| T_001 | Login with valid credentials | User is on the login page | 1. Enter valid username (standard_user) 2. Enter valid password (secret_sauce) 3.Click login | User should be  redirected to inventory page |  User was successfully redirected to the inventory page | Pass |
| T_002 | Login with invalid password | User is on the login page | 1.Enter valid username (standard_user) 2. Enter invalid password (sauce)3.Click login | Error message should be displayed |  Error message was displayed stating that the password does not match any user in this service | Pass |
| T_003 | Login with empty fields | User is on the login page | 1. Leave username blank () 2.Leave password blank ()  3. Click Login | Error message for required fields should be shown | Error message was displayed stating that the username is required | Pass |
| T_004 | Login with username only | User is on the login page | 1 Enter valid username 2. Leave password empty 3. Click login | Error message indicating password required should be displayed | Error message requiring password was displayed | Pass |
| T_005 | Login with locked out user | User is on the login page | 1. Enter username (locked_out_user) 2. Enter valid password(secret_sauce) 3.Click login | Error message indicating that the user is locked out shoud be displayed | Error message was displayed that the user has been locked out | Pass |




## 2. Cart Functionality
| Test ID | Test Scenario | Preconditions  | Test Steps | Expected Results | Actual Reslt | Status |
|-|-|-|-|-|-|-|
| T_006 | Add a single item to the cart | User is logged in as standard_user | 1. Click "Add to cart" button for a the item to be added in the cart 2. Click the cart icon | The item should be visible inside the cart page |The item was visible in the cart | Pass |
| T_007 |  Remove the item from cart | User has one item in the cart | 1. Navigate to cart 2. Click the "Remove" button | The item should be removed from the cart | The item was successfully removed from the cart| Pass |
| T_008 | Add multiple items to the cart | User has two items in the cart | 1. Click add two different items to the cart 2. Click the cart icon | Both items should be displayed in the cart and the cart should show the correct number, representing number of items in the cart | Both items were visible in the cart, and the correct number of items was showing on the cart icon| Pass |

## 3. Checkout Functionality


| Test ID | Test Scenario | Preconditions  | Test Steps | Expected Results | Actual Reslt | Status |
|-|-|-|-|-|-|-|
| T_009 | Complete checkout with valid information | User has at least one item in  the cart | 1.Click cart icon 2. Click checkout 3. Enter valid First Name 4.Enter valid Last name  5.Enter valid postal code 6.Click Continue 7. Click Finish | An order confirmation page should be displayed, thanking the customer | "Thak you for your order" message was displayed| Pass |
| T_010 | Attempt checkout without First Name | User has an item in the cart | 1.Click Checkout 2.Leave First Name empty 3.Enter Last Name 4.Enter PostalCode 5.Click continue | Error message saying: "First Name is required" should be displayed | Error: First Name required was displayed| Pass |
| T_011 | Attempt checkout without Last Name | User has an item in the cart | 1. Click Checkout 2. Enter First Name 3. Leave Last Name empty 4.Enter PostalCode 5 Click Continue | Error message saying": "Last Name is required should be displayed | Error: Last Name is required was displayed | Pass |
| T_012 | Attempt Checkout without a PostalCode | User has at least one item in the cart | 1.Click Checkout 2.Enter First Name 3.Enter Last Name 4. Leave the PostalCode empty 5 Click Continue | Error message: "PostalCode required" should be dislpayed | Error: PostalCode required was displayed  | Pass |


