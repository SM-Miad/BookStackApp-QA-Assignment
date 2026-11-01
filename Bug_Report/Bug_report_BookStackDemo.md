
**Bug report**   
Date: 30-Oct-2026

---

**Bug Report Details**

●   **Bug ID:**   BUG-01  
●   **Bug Title:**   Token expiry date can be set back in time.  
●   **Severity:**   Medium  
●   **Priority:**   High  
●  **Environment:**    Mozilla Firefox Version 159.0 (64-bit), Windows 11,   BookStack v26.09.2  
●   **URL:**   https://demo.bookstackapp.com/  
●   **Module:**   API Token management.  
●   **Precondition:**   User need to be logged in as Admin.  

**Description:**   While creating an API Token for the client, the user can set the API expiry date in the past date.  

**Steps to reproduce:**  
1.   Open the   URL   in the web browser.  
2.   Login using valid credential (Email: admin@example.com ), (Password: password )  
3.   Click on “Settings” on the top navigation menu.  
4.   Navigate to the “Users”.  
5.   Click and open any user.  
6.   Click on the “Create token” button from the “API Tokens” section.  
7.   Enter name (example: TestAPI1), select a past Expiry Date (example: 01/30/2025 ) .  
8.   Click “Save”.  

**Expected result:**   An inline validation message will be displayed for the invalid expiry date, the API token creation failed  Actual result : API token is successfully created and redirects the user to the API Token page.


**Evidence:**  
A screenshot given below displays, user can create API Token with a past expiry date .
![alt text](https://github.com/SM-Miad/BookStackApp-QA-Assignment/blob/main/Bug_Report/Evidence/Screenshot_8.png?raw=true)

---

●   **Bug ID:**   BUG-02  
●   **Bug Title:**   Books creation containing duplicate name.  
●   **Severity**:   Low  
●   **Priority:**   Low  
●   **Environment:**   Mozilla Firefox Version 159.0 (64-bit), Windows 11,   BookStack v26.09.2  
●   **URL:**   https://demo.bookstackapp.com/  
●   **Module:**   Book management.  
●   **Precondition:**   User need to be logged in as Admin.  

**Description:**   The user can create books with existing names causing duplicate books to exist.  

**Steps to reproduce:**  
1.   Open the   URL   in the web browser.  
2.   Login using valid credential (Email: admin@example.com ), (Password: password ).  
3.   Click on the "Books" in the top nav and navigate to the Books page.  
4.   Click "Create new book" on the action section.  
5.   Create a new book “Test book” and save it.  
6.   Create another book containing the same name as the previous one and save it.  
7.   navigate to the Books page.  
8.   Verify if two books containing the title “Test book” exist.  

**Expected result:**   A warning message is displayed for duplicate books, and book creation rejected.  

**Actual result :** The duplicate book created successfully without any validation error and both books containing the title “Test book” exist.  Evidence:  A screenshot given below displays duplicate books with the title ”Test Book” created .

**Evidence:**  
A screenshot given below displays, user can create API Token with a past expiry date .
![alt text](https://github.com/SM-Miad/BookStackApp-QA-Assignment/blob/main/Bug_Report/Evidence/Screenshot_9.png?raw=true)

---


