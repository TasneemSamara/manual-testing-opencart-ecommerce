# OpenCart E-commerce Testing Portfolio

**Author:** Tasneem Samara  
**Role:** Junior Manual QA Engineer  
**Project:** OpenCart Frontend Manual Testing  
**Duration:** 8 days (21 Oct – 28 Oct 2026)  
**Application Under Test:** [OpenCart Frontend](https://demo.opencart.com/)  
**Version:** 1.0

---

## 🎯 Project Overview

A comprehensive manual testing cycle on the OpenCart e-commerce frontend application covering **31 modules** and **514 test cases**. The project followed the complete Software Testing Life Cycle (STLC) — from requirement analysis through test execution, defect management, and test closure.

All testing was performed against a live demo application. Findings, bugs, and documentation are public in this repository for transparency and portfolio review.

---

## 📋 What Was Tested

| Module Group | Modules Covered |
|---|---|
| **Authentication** | Register, Login, Logout, Forgot Password |
| **Product Discovery** | Search, Product Compare, Product Display Page, Home Page |
| **Shopping Flow** | Add to Cart, Wish List, Shopping Cart, Checkout |
| **Account Management** | My Account, Account Information, Change Password, Address Book |
| **Orders** | Order History, Order Information, Product Returns, Downloads, Reward Points, Returns, Transactions, Recurring Payments |
| **Marketing** | Affiliate, Newsletter, Contact Us, Gift Certificate, Special Offers |
| **Site-Wide** | Header/Menu/Footer, Currencies |

---

## 📊 Test Results Summary

| Metric | Value |
|---|---|
| Total Test Scenarios | 31 |
| Total Test Cases | 514 |
| Executed (Pass + Fail) | 494 (96.1%) |
| **Pass** | **445 (90.1%)** |
| **Fail** | **49** |
| **Blocked** | **20** |
| **Bugs Found (OpenCart)** | **32** |
| **Bugs Found (TutorialsNinja — comparative testing)** | **10** |

### Bugs by Severity

| Severity | Count |
|---|---|
| 🔴 Critical | 6 |
| 🟠 Major | 14 |
| 🟡 Minor | 12 |

### Bugs by Priority

| Priority | Count |
|---|---|
| P0 (High) | 8 |
| P1 (Medium) | 16 |
| P2 (Low) | 7 |
| P3 (Lowest) | 1 |

---

## 🐛 Notable Bugs Found

### Critical (P0) — Full List

| Bug | Summary |
|---|---|
| BUG-7 | User logged out on browser back after login |
| BUG-9 | Password visible in plain text in page source |
| BUG-17 | Future date accepted in Return Order Date |
| BUG-19 | Non-affiliate user can log in via Affiliate Login |
| BUG-20 | Canon EOS 5D 'Select' dropdown empty |
| BUG-31 | Registration succeeds with invalid email format |

### Major (P1) — Selection

| Bug | Summary |
|---|---|
| BUG-1 | 'Thank you for registering' email not received |
| BUG-2 | Telephone validation missing (letters accepted) |
| BUG-4 | Telephone field accepts spaces only |
| BUG-5 | Weak password accepted (no complexity check) |
| BUG-8 | User auto-logged in on browser back after logout |
| BUG-14 | Negative/zero/null quantity accepted on Product Page |
| BUG-15 | Cart shows "empty" on negative quantity (no warning) |
| BUG-16 | Estimate Shipping shows $8 instead of $5 |
| BUG-22 | First Hero image on Home links to wrong product |
| BUG-23 | Blank Contact Us page after form submit |
| BUG-27 | No clear error when quantity below minimum |
| BUG-28 | Cannot navigate back to Billing Details in checkout |
| BUG-29 | UK postcode not validated |
| BUG-30 | Past date accepted in Delivery Date field |
| BUG-32 | Forgot Password accepts invalid email formats |

Full details for all 32 bugs: see `Tasneem_OpenCart_BugReport.xlsx`

---

## 📁 Files in This Repository

| File | Description |
|---|---|
| **`Tasneem_OpenCart_TestScenarios.xlsx`** | 31 test scenarios with priority and test case count |
| **`Tasneem_OpenCart_TestCases.xlsx`** | 514 detailed test cases across 31 modules |
| **`Tasneem_OpenCart_TestExecution.xlsx`** | Execution results — Pass/Fail/Blocked per test case |
| **`Tasneem_OpenCart_BugReport.xlsx`** | 32 OpenCart bugs + 10 TutorialsNinja bugs with full steps, expected results, actual results, severity, priority |
| **`Tasneem_OpenCart_RTM.xlsx`** | Requirement Traceability Matrix — 100% coverage of all 31 requirements |
| **`Tasneem_OpenCart_TestSummary.xlsx`** | Final Test Summary Report with execution metrics, defect analysis, and recommendations |

**How to view:** Click any file to download, then open in Microsoft Excel or Google Sheets.

---

## 🛠️ Skills Demonstrated

- **Test Design Techniques:** Equivalence Class Partitioning (ECP), Boundary Value Analysis (BVA), Decision Table, State Transition, Error Guessing
- **Test Documentation:** Test Plan, Test Scenarios, Test Cases, Bug Reports, Requirement Traceability Matrix, Test Summary Report
- **Bug Management:** Severity vs Priority classification, root cause grouping, defect lifecycle tracking
- **Cross-Browser Testing:** Windows 11 (Chrome, Edge), Mac OS (Safari), Android (Chrome), iPhone (Safari)
- **SDLC / STLC Knowledge:** Full lifecycle applied — from requirement analysis to test closure
- **Comparative Analysis:** Tested OpenCart against TutorialsNinja (a newer installation) to identify which bugs had been fixed in newer versions

---

## 💡 Key Learnings

1. **Group bugs by root cause, not by symptom.** One broken email setup caused failures across 4 different modules — logging it once as a single bug is clearer than logging it four separate times.

2. **Not every unexpected behavior is a bug.** Forgot Password showing the same success message for unregistered emails is a **security best practice** (prevents user enumeration attacks), not a defect.

3. **Silent failures are worse than visible errors.** Several bugs (quantity below minimum, negative cart quantity) fail with no message at all — worse UX than a clear error message would be.

4. **Environment limitations mean BLOCKED, not PASS.** With only Cash on Delivery available in the demo, payment-dependent test cases are marked Blocked with the reason documented, not marked as passing.

5. **Cross-browser testing reveals environment-specific bugs.** Session behavior bugs (like logout not syncing across browsers) only show up when testing across multiple environments.

---



## 📜 Note

This project is for **educational and portfolio purposes only**. All testing was performed on a public demo application. No proprietary or confidential content is included.

---

*Last updated: October 2026*