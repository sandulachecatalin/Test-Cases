# Test Case Samples
Below are some Test Case samples that I wrote while working on previous projects.

Login Functionality
---------------------
**Title**
Test case 1: Login Failure with Incorrect Username and Password

**Description:**
Verify that the system handles login attempts with incorrect username and/or password appropriately by displaying an error message and not allowing access.

**Steps to reproduce:**
1. Launch the application.
2. Navigate to the login screen.
3. Enter an incorrect username.
4. Enter an incorrect password.
5. Click on the "Login" button.

**Expected result:**
- The system should display an error message indicating that the login attempt has failed due to invalid credentials.
- The user should not be granted access to the application.

**Test data:**
Incorrect Username: catalin
Incorrect Password: pass12345

----------------------

**Title**
Test case 2: URL Modification for Login Page to My Account Page 

**Description:**
Verify that the system properly handles URL modification attempts from the login page to the "My Account" page and provides the appropriate redirection.

**Steps to reproduce:**
1. Launch a web browser.
2. Enter the URL website.com/login in the address bar.
3. Press "Enter" to navigate to the login page.
4. Observe the URL in the address bar.
5. Modify the URL to website.com/myaccount.
6. Press "Enter" to attempt navigation to the "My Account" page.

**Expected Results:**
- The system should detect the modified URL and recognize that the user is not logged in.
- The system should redirect the user back to the login page to authenticate before accessing the "My Account" page.
- An appropriate error message should be displayed, indicating that the user needs to log in to access their account.

---------------------------

**Title**
Test case 3: Successful Login with Correct Username and Password and "Remember Me" Option

**Description:**
Verify that the system successfully logs in the user with the correct username and password when the "Remember Me" option is selected, and the session remains persistent even after the user closes the browser.

**Steps to reproduce:**
1. Launch a web browser.
2. Enter the URL website.com/login in the address bar.
3. Press "Enter" to navigate to the login page.
4. Enter a valid username and password.
5. Check the "Remember Me" checkbox.
6. Click on the "Login" button.

**Expected Results:**
- The system should validate the entered credentials and allow access to the user account.
- The user should be successfully logged in and redirected to their account dashboard or home page.
- If the "Remember Me" option is selected, the system should create a persistent session that remains active even after the user closes the browser.
- Upon returning to the website within a reasonable timeframe, the user should still be logged in without needing to enter credentials again.

---------------------------

**Title**
Test case 4: SQL Injection Prevention

**Description:**
Verify that the application is protected against SQL injection attacks, ensuring that user input is properly sanitized and validated to prevent unauthorized database access.

**Steps to reproduce:**
1. Launch the application.
2. Navigate to a page where user input is accepted, such as a search box or a login form.
3. Attempt a SQL injection attack by entering malicious SQL code into the input field.

**Expected Results:**
- The system should properly validate and sanitize user input to prevent SQL injection attacks.
- If the input is detected to contain malicious SQL code, the system should:
    - Reject the input and display an appropriate error message.
    - Prevent the execution of the injected SQL code.
- The application should not display sensitive information about the database or the SQL query error in the response.
- The application's logs should record the attempted attack, if applicable.

