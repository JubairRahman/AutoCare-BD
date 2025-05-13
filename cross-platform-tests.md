# 🔁 Cross-Platform Test Report: AutoCare Platform

This report documents cross-platform testing results for the AutoCare web application. The goal is to verify consistent performance and functionality across different devices, operating systems, and browsers.

---

## 🧪 Test Matrix

| Test Case ID | Feature               | macOS (Chrome) | Windows (Chrome) | Windows (Firefox) | Android  |
|--------------|-----------------------|----------------|------------------|-------------------|------------------|
| CP-001       | Website Accessibility | ✅              | ✅                | ✅                 | ✅                |
| CP-002       | Login/SignUp Flow     | ✅              | ✅                | ✅                 | ✅                |
| CP-003       | Product Search        | ✅              | ✅                | ✅                 | ✅                |
| CP-004       | Model Year Dropdown   | ❌ Not visible  | ❌ Not visible    | ✅                 | ✅                |
| CP-005       | Checkout Flow         | ✅              | ✅                | ✅                 | ✅                |
| CP-006       | Order Confirmation    | ✅              | ✅                | ✅                 | ✅                |
| CP-007       | Invoice Download      | ✅              | ✅                | ✅                 | ⚠️ Opens in new tab only |
| CP-008       | Order Notification    | ✅              | ✅                | ✅                 | ✅                |

Legend:  
✅ = Works as expected  
❌ = Major issue  
⚠️ = Minor issue or inconsistency

---

## 🌐 Platforms & Devices Covered

| Platform | OS Version          | Browser(s)       |
|----------|---------------------|------------------|
| Desktop  | macOS Sonoma 14.1.1 | Chrome           |
| Desktop  | Windows 10 Pro      | Chrome, Firefox  |
| Mobile   | Android 15         | App           |
| Display   | 14"          | 22"           |

---

##  UI/UX Observations & Recommendations

The following observations were made during testing regarding the layout, responsiveness, alignment, and visual consistency of the AutoCare web platform:

### ➩ UI Issues
- Misalignment of "Add to Cart" and "Buy Now" buttons on product cards (mobile view).
- Overlapping labels on login and registration forms (small screen).
- Date picker UI opens in May 2012 by default — not intuitive.

### ➩ Responsiveness Issues
- Some text and buttons overflow outside viewport on smaller screens.
- Filter sections not collapsing properly in mobile view.

### ➩ Functional + UI Combined
- Model Year dropdown not visible in Chrome (covered in functional bug, but affects UX).
- Missing feedback on some button clicks (e.g., “Add to Favorites”).

### 💡 Recommendations
- Standardize padding, margins, and alignment using responsive frameworks like Tailwind or Bootstrap Grid.
- Apply consistent font sizes and spacing across forms and buttons.
- Conduct mobile-first design QA pass using browser tools and actual devices.
- Add loading indicators and feedback messages where necessary.


---

## Related Documentation

- [Functional Scenarios](./functional-scenarios.md)
- [Bug Reports](./bug-reports.md)
- [Test Cases](./test-cases.md)
