#  Bug Report: AutoCare Platform

This document provides a structured report of bugs identified during exploratory and functional testing of the AutoCare web platform. The goal is to highlight issues affecting usability, functionality, and performance to support improvement efforts.


##  Environment

* **Platform:** Web Application
* **URL:** [https://autocare.com.bd/](https://autocare.com.bd/)
* **Browser:** Chrome (v136.0.7103.93)
* **Tested Devices:**

  * macOS Sonoma 14.1.1
  * Windows 10 Pro

---

### BUG-01

**Issue:** Date of Birth filed defaults to May 2012, which is not user-friendly and suitables for the users.
**Module:** Registration Page
**Bug Type:** UI

**Steps to Reproduce:**

1. Navigate to the Sign Up / Registration page.
2. Click on the "Date of Birth" field.
3. Observe the default value shown.

**Expected Result:**

* Date of Birth picker should open with a year selector or empty state to ease date selection.

**Actual Result:**

* The picker defaults to May 2012, which is not user-friendly.

**Status:** Open
