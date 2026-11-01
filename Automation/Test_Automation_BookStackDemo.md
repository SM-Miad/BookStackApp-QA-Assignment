
# **Test Automation** 
 
---

### AT-01: Valid Login  
**Objective:**   Verify that the user can login with valid credentials. 
 
**Precondition:**   The user needs to be logged out.
  
**Automated test steps:**
1.   Open base URL ( https://demo.bookstackapp.com/ )  
2.   Click “Log in”  
3.   Enter Email ( admin@example.com ) and Password (password)  
4.   Click the “Log in” button.  
5.   Wait for the homepage/dashboard to load.  
6.   Verify that the user logged in as “Admin” from the User menu.  
7.   Log out and verify that “Log in” button is shown again.  

**Expected result:**   The user with valid credentials can log in successfully.  

**Reason for automation:**   The login module is a most frequently used it is also one of the most smoke tested module. Automation of this module gives a fast feedback if authentication session handling has any issue.  


---


### AT-02: Add and remove books from bookshelf  

**Objective:**   Verify that the user can manage books in the bookshelf.  

**Precondition :** The logged in user has the permission to manage the bookshelf. Books exist on the bookshelf.  

**Automated test steps:**  
1.   Login with valid credentials of a user that has permission to manage shelves.  
2.   Click on “Shelves” in the navigation menu.  
3.   Click on “Internal Departments” shelf.  
4.   Click “Edit” from the actions menu.  
5.   Remove the “IT Department” book and add the “HR Information” book in the shelf.  
6.   Click the “Save Shelf” button.
7.   Reopen the “Internal Departments” shelf and verify that changes persist.  

**Expected result:**   The selected book added on the book shelf, and the removed book is absent on the shelf after reopening the shelf.  

**Reason for automation:**   The book organization of a shelf is a repeatable workflow. Automating this workflow helps to prevent bugs in multi-selection, saving, and data storage.  

---

### AT-03: Global search  

**Objective:**   Verify that a known content can be found by using search.  

**Precondition :** The content exist within the platform.  

**Automated test steps:**  
1.   Open the base URL ( https://demo.bookstackapp.com/ ).  
2.   Use global search and enter “hr information”.  
3.   Submit the search.  
4.   Verify if the search result page loads successfully.  
5.   Verify if any relevant search result is present.  
6.   Open the search result and verify if the title matches the search keywords.  

**Expected result:**   The search result shows relevant search results, and the routs the user successfully to desired result.  

**Reason for automation:**   Search is a primary way for people to find content. It is easy to test repeatedly, because it uses stable sample data. But it is prone to bugs in how results are indexed, displayed, and routed.

---
