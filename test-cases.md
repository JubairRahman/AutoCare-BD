#  Test Cases: AutoCare Platform

This document provides a collection of detailed test cases for validating key functionalities of the AutoCare web application. The purpose is to ensure that the system performs as expected under various user actions and edge scenarios.

Each test case includes the test case ID, scenario description, input data, expected results, and actual results. These cases help ensure quality and consistency across major features such as authentication, product search, checkout flow, and order tracking.

---

##  Complete Test Case Spreadsheet

For full detailed test case execution, input data variations, test steps, and actual result tracking, please refer to the shared spreadsheet:

🔗 [AutoCare Detailed Test Cases - Google Sheet](https://docs.google.com/spreadsheets/d/13hWKZHAP3dk51rsRNiN7ko92wRzPcQMa-eQKh0m93kk/edit?gid=1140583909#gid=1140583909)

---

##  Test Environment

- **Platform:** Web Application  
- **URL:** [https://autocare.com.bd](https://autocare.com.bd)  
- **Browser:** Chrome v136.0.7103.93  
- **Devices Tested:**
  - macOS Sonoma 14.1.1
  - Windows 10 Pro

---

## 📋 Sample Test Cases

| Test Case ID | Feature        | Test Scenario                                   | Input Data                  | Expected Result                                             | Status  |
|--------------|----------------|--------------------------------------------------|-----------------------------|-------------------------------------------------------------|---------|
| TC-001       | Sign Up        | User signs up with valid mobile and OTP         | Valid name, mobile, OTP     | User is redirected to homepage with success message         | Pass    |
| TC-002       | Login          | Login with invalid credentials                  | Wrong password              | System shows warning "Incorrect password"                   | Pass    |
| TC-003       | Search Filter  | Apply filters including Model Year              | Brand: Toyota, Year: 2020   | Products filtered accordingly; Model Year visible           | **Fail**|
| TC-004       | Add to Cart    | Add product to cart and proceed to checkout     | Logged-in user, product     | Product added, address prompt shown                         | Pass    |

---

### 📌 Notes

- This file provides a preview of important test scenarios.
- Please refer to the spreadsheet for step-by-step instructions, test data sets, edge cases, and regression coverage.
- All issues encountered during testing have been documented in the [Bug Reports](./bug-reports.md) file.

