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

**Feature:** Registration Page


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

---

### BUG-02

**Issue:** The Search Filter accepts any keywords like “Test” and showing the products lists.


**Feature:** Search

**Bug Type:** Functional

**Steps to Reproduce:**

1. Go to the Homepage
2. Search for products in search filed
3. Input random keywords (ex: Test, abcd)
4. Observe the result displayed.



**Expected Result:**

* Only relevant product will show or alert will pop-up like “No Product Found”

**Actual Result:**

* Product list is showing.

**Status:** Open


---

### BUG-03

**Issue:** The secondary filter option is showing in Read-Only mode after first filter.

**Feature:** Search Filter

**Bug Type:** Functional, UI

**Steps to Reproduce:**

1. Go to the Homepage
2. Filter first time (with vehicle type, brand etc)
3. Products list will show
4. Try second time for filter.
5. Filter will show read-only mode.


**Expected Result:**

* The Filter will work perfectly.

**Actual Result:**

* The filter is not working. It’s showing the read-only mode. 


**Status:** Open

---

### BUG-04

**Issue:** The Ad section displays a static image file instead of dynamic content.

**Feature:** Ad section

**Bug Type:**  Functional, UI

**Steps to Reproduce:**

1. Goto Homepage
2. Search any thing for product
3. Below the filter section
4. Static image of Ad.

**Expected Result:**

* The ad should load from the ad server or support dynamic campaigns.
* Or it should be styled and formatted properly if using image banners.

**Actual Result:**

* A static image file is attached directly (hardcoded or improperly referenced).
* The ad looks like a placeholder and lacks interactivity or relevance.

**Status:** Open

---

### BUG-05

**Issue:** Filter is not working when new filter add for search a product. 
When filtered a product by “Lighting” a product list showing (ex: Head Light), also filtered with “Lighting”, and “Alternators both” it’s showing No Product Found.

**Feature:** Category Filter

**Bug Type:** Functional

**Steps to Reproduce:**
1. Navigate to the product list page.
2. Filter for “Lighting” - relevant product shown. (Head Light).
3. Filter with “Lighting” and “Alternators” 
4. Observe the page showing with No Product Found.


**Expected Result:**

* The relevant product should show based on filter.
**Actual Result:**

* The system fails to show the desired product list based on filter.


**Status:** Open

---

### BUG-06

**Issue:** The Price Filter not considering with discount price.
When filtering products by price range 0–658, a product with an original price of 700 and discounted price of 658 is not shown, even though it falls within the specified range based on the actual payable amount.

**Feature:**  Price Filtering

**Bug Type:** Functional

**Steps to Reproduce:**
1. Navigate the product list 
2. Filter with Price range 0–658
3. Observe the result.

**Expected Result:**

*  The product with discounted price 658 should appear in the results because it falls within the filtered range based on the user's cost.
  
**Actual Result:**

* The product is not showing with price range.

**Status:** Open

---

### BUG-07

**Issue:** “Home” breadcrumb link is not working on checkout page.

**Feature:** Checkout

**Bug Type:** Functional

**Steps to Reproduce:**
1. Select a product and click on Buy Now.
2. Checkout page will be redirected.
3. Click on Home button 
4. Button is not working


**Expected Result:**

* The page should redirect to the Homepage.
  
**Actual Result:**

* The Homepage link appears inactive or not linked.

**Status:** Open

---

### BUG-08

**Issue:** Fluctuating Product rating show between listing and details page.

**Feature:** Product Rating

**Bug Type:** Functional

**Steps to Reproduce:**

1. Navigate to the product list 
2. Product is showing with 5 star rating
3. Click on the product to view details 
4. Observe the rating section, it’s showing “0 Average Rating”


**Expected Result:**

* Rating displayed same in both field. 


**Actual Result:**

* Product listing shows 5 star rating, and In details page it’s showing 0 average.


**Status:** Open

---

### BUG-09

**Issue:** All products show 5-star rating with 3 reviews but No actual reviews in details page.

**Feature:** Product Rating and Review

**Bug Type:** Functional

**Steps to Reproduce:**
1. Navigate any related product card
2. All products are with 5-star rating and 3-reviews
3. Click on the product details 
4. Rating is showing 0 with no reviews

**Expected Result:**

* Product ratings and review counts should be based on actual customer reviews.
* Ratings must reflect real feedback both in listing and detail views.
* If there are no reviews, show: "No Ratings Yet" or hide the stars.

**Actual Result:**

* Listing pages falsely display identical rating and review counts.
* Details page reveals there are no actual reviews or ratings.


**Status:** Open

---

### BUG-10

**Issue:** Filter product with 1 star but list is showing with more than 1-star rating 

**Feature:** Rating

**Bug Type:** Functional

**Steps to Reproduce:**

1. Navigate product list 
2. Categorized with 1-star rating
3. Observe the product list including more than 1-star

**Expected Result:**

* The product should show with 1-star only
  
**Actual Result:**

* All kind of rated products are showing in product list.

**Status:** Open

---

### BUG-11

**Issue:** All services images are same in service list.

**Feature:**  Service Card

**Bug Type:** Functional, UI

**Steps to Reproduce:**

1. Search for any service.
2. Observe the suggestive service image


**Expected Result:**

* All images should be relevant with specific service.
  
**Actual Result:**

*  All service images are same.

**Status:** Open

---

### BUG-12

**Issue:** When adding “Address” for delivery without setting that as the default, the Address is not showing for shipping.

**Feature:** Add Address.

**Bug Type:** Functional, Usability

**Steps to Reproduce:**

1. Go to the address add for shipping
2. Input all required data
3. Uncheck the default delivery address and save
4. Observe there is no address showing


**Expected Result:**

* Address should appear in the list without default setting.
  
**Actual Result:**

* Address does not appear if it’s not set as default.

**Status:** Open

---

### BUG-13

**Issue:** Address is not showing if there is only one address added, The address appears only after adding a second one. 

**Feature:** Add Address

**Bug Type:** Functional, UI logic

**Steps to Reproduce:**

1. Add a single Address for delivery
2. Save the address without set as default
3. Observe no address will show
4. Add another address for delivery
5. Address will show in the list. 


**Expected Result:**

* Single address should show in the list.
  
**Actual Result:**

* When a single address is added it’s not visible, for multiple address the list is visible. 


**Status:** Open

---

### BUG-14

**Issue:** The registration form allows profiles to be created without saving the required field. 

**Feature:** Create Profile

**Bug Type:** Functional, Validation

**Steps to Reproduce:**

1. Sign up for a new account
2. Provide OTP
3. Input only name
4. Click on any place on device screen
5. Profile is created without saving other required fields.

**Expected Result:**

* There should be an alert or warning for profile creation without saving required field. 

**Actual Result:**

* Profile was created without the required field.


**Status:** Open

---

### BUG-15

**Issue:** Order number is not showing while request for Product return. 

**Feature:**  Product Return 

**Bug Type:** Functional

**Steps to Reproduce:**

1. Go to the Product return page
2. Cilck on Order Number field
3. Observe No order is suggesting



**Status:** Open

---

### BUG-16

**Issue:**  In the Invoice, there is no indicator for the discount amount, but the discount amount is counted.

**Feature:** Invoice

**Bug Type:** Functional, UI

**Steps to Reproduce:**
1. Buy a product using any Discount coupon or points
2. Confirm that order
3. Download Invoice 
4. Observe the Total Amount

**Expected Result:**

* All kind of detailed amount will show in the invoice breakdown.
  
**Actual Result:**

*  Discount details are not showing.

**Status:** Open

---

### BUG-17

**Issue:** Icons are overlapping on mobile

**Bug Type:** UI

**Steps to Reproduce:**

1. Add some product in favorite list
2. Navigate the favorite list
3. Observe the overlap


**Status:** Open

---

### BUG-18

**Issue:** The validation alert for inputting short  Phone number needs to change

**Feature:** Log in/ Sign Up


**Bug Type:** UI

**Steps to Reproduce:**

1. Go to Log in/ Signup page
2. Input 3-4 digit of a phone number
3. Click on log in or continue
4. Observe the warning message


**Expected Result:**

* The warning message should be different for short number entry “Mobile Number cannot be shorter than 11 digits.
  
**Actual Result:**

* The same warning message is showing for both short and long input. 

**Status:** Open

---

### BUG-19

**Issue:** It is showing “No Questions Available” while there are already questions available.

**Feature:** FAQ

**Bug Type:** Functional, UI

**Steps to Reproduce:**

1. Search for the product “Brake Show Rear”
2. Click on the details of that product
3. Observe the FAQ section

---

### BUG-20

**Issue:** Language Mode is not working.

**Feature:** Language

**Bug Type:** Functional

**Steps to Reproduce:**

1. Goto the homepage
2. Switch the language English to Bangla 
3. Observe the scenario ( Language is not working) 

**Expected Result**
* The language should change. 
**Actual Result**
* The language mode is not functioning.


---

##  About the QA

# Jubair Rahman

**Software Engineer (QA) | HealthTech | Passionate about testing, tools, and UI quality.**

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jubair-rahman/) [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JubairRahman) [![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/8801645763353)

