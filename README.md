DEMOBLAZE QA TESTING PROJECT

OVERVIEW
This project documents manual and API testing performed on the demo e-commerce website Demoblaze. The goal was to validate core user flows such as Sign-Up, Login, Cart, and Checkout through UI and API testing, identify defects, and demonstrate QA documentation quality.

SCOPE
The project includes both UI and API functional testing.

UI testing covers boundary, validation, and usability checks for key user flows.

API testing focuses on verifying endpoints for sign-up, login, cart operations, and order placement.

The tools used were Google Chrome 115, Windows 10, Postman, DevTools, Excel, and GitHub.

All test data used synthetic usernames (for example, TestUser80, TestUser88) and non-sensitive dummy credentials.

DELIVERABLES
- TestCase_Demoblaze.xlsx – contains all test documentation.
- Tab 'TestCase_UI': 28 functional UI tests for Sign-Up, Login, Cart, and Checkout.
- Tab 'BugReport_UI': 8 reported UI defects with severity, priority, and screenshots.
- Tab 'TestCase_API': 24 Postman API test cases, including positive, negative, and boundary scenarios.
- Tab 'BugReport_API': 2 backend defects with linked screenshots.
- Postman folder – includes collection and environment JSON files for API testing.
- Screenshots folder – includes subfolders 'UI' and 'API' with evidence for failed and notable cases.
- JS_Scripts tab – example Postman script for response validation (optional).

TEST EXECUTION SUMMARY
UI testing included 28 test cases, of which 18 passed, 6 failed, and 4 were not executed.
API testing included 24 test cases, of which 16 passed, 2 failed, and 6 were partially executed due to demo environment limitations.
In total, 52 tests were executed with 10 unique bugs identified (8 UI and 2 API).

ENVIRONMENT NOTES
The backend API is a public demo and does not persist session data.
Cart and order operations are session-based and simulated rather than fully functional.
Partial Pass results represent expected limitations of the demo environment and are not considered defects.

KEY FINDINGS
UI Bugs:
- Password validation too weak (BUG-001, BUG-002).
- Username accepts SQL-like input (BUG-003).
- Items can be added to cart without login (BUG-004).
- Quantity update feature missing in cart (BUG-005).
- Layout issues on mobile devices (BUG-006).
- Video loading and console JavaScript errors (BUG-007, BUG-008).

API Bugs:
- Empty credentials cause a 500 internal server error (BUG_API-001).
- Invalid product ID accepted without validation (BUG_API-002).

CONCLUSION
The testing project demonstrates a complete QA cycle: from test design and execution to defect reporting and documentation.
All materials follow professional QA standards, with clear linkage between test cases, bugs, and evidence.
Demo-environment limitations were documented separately from functional issues.

FOLDER STRUCTURE
### 📁 FOLDER STRUCTURE
QA-API-Testing-Demoblaze-Project
│
├── TestCase_Demoblaze.xlsx
├── README.md
│
├── Screenshots
│ ├── UI
│ └── API
│
├── Postman
│ ├── Demoblaze_API_Collection.json
│ └── Demoblaze_API_Environment.json
│
└── Exports
├── TestCase_UI.pdf
├── BugReport_UI.pdf
├── TestCase_API.pdf
└── BugReport_API.pdf

