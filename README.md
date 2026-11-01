# BookStack Application – QA Assignment

## Project Overview

This repository contains the Quality Assurance (QA) testing deliverables for the **BookStack Demo Application**.

The purpose of this project is to evaluate the application's functionality, identify potential defects, document test results, and define suitable test scenarios for automation.

**Application:** [BookStack Demo](https://demo.bookstackapp.com/)

**Test Environment:**
- Application: BookStack Demo
- Test Module: Books Management
- Browser: Mozilla Firefox
- Testing Approach: Manual Testing and Automation Test Design

---

## Repository Structure

```
📁 BookStackApp-QA-Assignment
├── 📁 Automation
│   ├── 📄 Test_Automation_BookStackDemo.md
│   └── 📄 Test_Automation_BookStackDemo.pdf
├── 📁 Bug_Report
│   ├── 📁 Evidence
│   │   ├── 📄 Screenshot_8.png
│   │   └── 📄 Screenshot_9.png
│   ├── 📄 Bug_report_BookStackDemo.md
│   └── 📄 Bug_report_BookStackDemo.pdf
├── 📁 Test_Cases
│   └── 📄 Test_cases_BookStackDemo.xlsx
└── 📄 README.md
```

---

## Testing Scope

### 1. Functional Testing

Functional testing was performed on the BookStack Books Management module to verify that the application's core functionalities work as expected.

A total of **19 test cases** were designed and executed.

The test cases cover four testing techniques:

| Testing Type | Description |
|---|---|
| Positive Testing | Verifies expected behavior with valid inputs. |
| Negative Testing | Verifies application behavior with invalid or missing inputs. |
| Boundary Value Testing | Tests input limits and maximum/minimum values. |
| Edge Case Testing | Tests unusual conditions and unexpected user scenarios. |

**Key functionalities tested:**
- Create a new book
- Edit existing book details
- Create a new page
- Input validation for mandatory fields
- Maximum and minimum title length
- Duplicate book creation
- Special characters and Unicode input
- Page deletion and confirmation
- Moving pages between books
- Book sorting functionality
- Browser crash and network recovery scenarios

**Test Execution Summary:**

| Metric | Result |
|---|---:|
| Total Test Cases | 19 |
| Passed | 16 |
| Failed | 3 |
| Pass Rate | 84.2% |
| Fail Rate | 15.8% |

The detailed test cases, execution results, and supporting information are available in the `Test_Cases` directory.

### 2. Bug Hunting

Bug hunting was performed to identify functional and UI-related issues in the BookStack application.

Each documented bug report includes:

- Bug ID
- Bug Title
- Module
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Evidence

Only reproducible and verified issues should be considered confirmed defects.

Refer to the `Bug_Report` directory for detailed bug reports and supporting evidence.

### 3. Test Automation

Three scenarios were selected as candidates for future UI automation.

| Test ID | Automation Scenario |
|---|---|
| AUT-01 | Add and Remove Books from a Bookshelf |
| AUT-02 | Move a Page Between Chapters |
| AUT-03 | Add, Update, and Remove Page Tags |

Each automation scenario includes:

- Test Objective
- Preconditions
- Test Data
- Detailed Test Steps
- Expected Results
- Automation Justification
- Key Validation Points

**Recommended Automation Technology:**
- JavaScript
- Playwright
- Page Object Model (POM)

These scenarios were selected because they involve repeatable workflows, multiple user interactions, and data persistence validations.

The detailed automation test designs are available in the `Automation` directory.

---

## Testing Techniques

The following testing techniques were considered throughout the assignment:

- **Positive Testing:** Valid input and successful workflows.
- **Negative Testing:** Invalid input and validation handling.
- **Boundary Value Analysis:** Minimum and maximum input limits.
- **Edge Case Testing:** Unusual conditions, such as network interruptions and browser recovery.
- **Exploratory Testing:** Investigating application behavior beyond predefined test scenarios.

---

## Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| BookStack Demo | Application Under Test |
| Microsoft Excel | Test Case Documentation |
| Microsoft Word / PDF | Bug Reports and Automation Documentation |
| Playwright | Proposed UI Automation |
| JavaScript | Automation Programming Language |
| Git & GitHub | Version Control and Project Submission |

---

## Conclusion

This QA assignment provided an opportunity to evaluate the BookStack application's Books Management functionality through structured manual testing, defect identification, and automation test planning.

The testing process helped identify validation issues, evaluate boundary conditions, examine unusual user scenarios, and define reusable automation candidates.

The documented deliverables provide a structured overview of the application's tested behavior and areas that may require further investigation.

---

## Author

**Shoab Mahmud Miad**

GitHub: [SM-Miad](https://github.com/SM-Miad)

Project Repository: [BookStackApp-QA-Assignment](https://github.com/SM-Miad/BookStackApp-QA-Assignment.git)

Application Under Test: [https://demo.bookstackapp.com/](https://demo.bookstackapp.com/)
