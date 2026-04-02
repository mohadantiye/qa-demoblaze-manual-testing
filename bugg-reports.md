Bug Reports – Demoblaze

BUG001 User can buy items without login
Steps
	1.	Open website
	2.	Select a product
	3.	Click “Add to cart”
	4.	Navigate to cart
	5.	Click “Place Order”
	6.	Fill in details and confirm purchase

Expected Result
User should be required to log in before placing an order
Severity:High

BUG002 – Weak input validation in signup form
Steps to Reproduce
	1.	Go to signup page
	2.	Enter username with invalid characters (e.g. admin@@@###)
	3.	Enter any password
	4.	Click Sign up

Expected Result
System should reject invalid username formats
Actual Result
System accepts usernames with any characters
Severity
Medium

BUG003 – Checkout form accepts invalid data
Steps to Reproduce
	1.	Add item to cart
	2.	Click “Place Order”
	3.	Enter:
	•	Numbers in name field (e.g. 12345)
	•	Letters in card field (e.g. abcde)
	•	Random country
	4.	Submit order

Expected Result
Form should validate input fields properly
Actual Result
Form accepts invalid and nonsensical data
Severity
High

BUG004 – Misleading error message on empty checkout
Steps to Reproduce
	1.	Add item to cart
	2.	Click “Place Order”
	3.	Leave all fields empty
	4.	Click Purchase

Expected Result
System should highlight all required fields clearly
Actual Result
Generic message shown: “Please fill out Name and Creditcard” even when all fields are empty
Severity
Low

BUG005 – Session persists after closing browser tab
Steps to Reproduce
	1.	Log in with valid credentials
	2.	Close browser tab
	3.	Reopen website

Expected Result
User session should expire or require login again
Actual Result
User remains logged in

Severity:Medium

BUG006 – Adding to cart allowed without authentication
Steps to Reproduce
	1.	Open website without logging in
	2.	Select a product
	3.	Click “Add to cart”

Expected Result
User should be prompted to log in
Actual Result
Product is added to cart without authentication
Severity:Medium

BUG007 – Duplicate username handling unclear
Steps to Reproduce
	1.	Attempt to sign up using common or simple usernames
	2.	Try variations with spaces or symbols
Expected Result
Clear validation rules and consistent error handling
Actual Result
System frequently returns “User already exists” even for unusual inputs
Severity:Low

