# Test Case Samples
Below are some Test Case samples that I wrote while working on previous projects.

# Login Functionality
---------------------
**Test case 1: Login Failure with Incorrect Username and Password**

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

**Test case 2: URL Modification for Login Page to My Account Page**

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

**Test case 3: Successful Login with Correct Username and Password and "Remember Me" Option**

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

**Test case 4: SQL Injection Prevention**

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

-------------------------------------


# Search functionality on Emag.ro

-------------------------------------

**Test case 5: Basic Search Functionality on eMAG.ro**

**Description:**
Verify that the search functionality on eMAG.ro works correctly in the typical scenario.

**Steps to reproduce:**
1. Open a web browser and navigate to www.emag.ro.
2. On the homepage, locate the search bar at the top of the page.
3. Enter the search term "laptop" into the search bar.
4. Click the "Search" button or press the "Enter" key.
5. Observe the search results page.

**Expected Results:**
- The search results page should load and display products related to the search term "laptop".
- The displayed products should include laptops and related items.
- The search results should be relevant to the search term and display product names, images, prices, and ratings, where applicable.

------------------------

**Test case 6: Advanced Search with Filters and Sorting on eMAG.ro**

**Description:**
Verify that the search functionality supports advanced features such as filters and sorting.

**Steps to reproduce:**
1. Perform the steps from the "Basic Search Functionality Test" to search for a specific product category (e.g., "smartphone").
2. On the search results page, apply filters to narrow down the results, such as selecting a specific brand and price range.
3. Observe the updated search results based on the applied filters.
4. Select a sorting option, such as sorting by customer ratings.
5. Observe the results after sorting.

**Expected Results:**
- The search results should be refined based on the applied filters, showing products that match the selected criteria (e.g., brand and price).
- The sorting option should reorganize the displayed products based on the selected sorting parameter (e.g., ratings).
- The user should be able to easily apply and remove filters, as well as change sorting options.

--------------------------------

**Test case 7: Search for Non-Existent Product on eMAG.ro**

**Description:**
Verify that the search functionality on eMAG.ro handles the scenario where the user searches for a product that doesn't exist in the database.

**Steps to reproduce:**
Open a web browser and navigate to www.emag.ro.
Locate the search bar at the top of the page.
Enter the search term "abc123" (a non-existent product) into the search bar.
Click the "Search" button or press the "Enter" key.
Observe the search results page.

**Expected Results:**
The search results page should indicate that no products match the search term "abc123."
A message or an empty results page should inform the user that no products were found for the entered search term.
There should not be any products displayed in the search results.


