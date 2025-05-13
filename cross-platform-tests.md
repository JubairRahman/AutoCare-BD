# 🔁 Cross-Platform Test Report: AutoCare Platform

This document outlines the results of cross-platform testing conducted on the AutoCare web application. The objective is to ensure consistent user experience and functionality across different devices, browsers, and operating systems.

---

## 🧪 Test Matrix

| Test Case ID | Feature             | macOS (Chrome) | macOS (Safari) | Windows (Chrome) | Windows (Firefox) | Android (Chrome) | iOS (Safari) |
|--------------|---------------------|----------------|----------------|------------------|-------------------|------------------|--------------|
| CP-001       | Website Accessibility | ✅              | ✅              | ✅                | ✅                 | ✅                | ✅            |
| CP-002       | Login/SignUp Flow     | ✅              | ✅              | ✅                | ✅                 | ✅                | ✅            |
| CP-003       | Product Search        | ✅              | ✅              | ✅                | ✅                 | ✅                | ✅            |
| CP-004       | Model Year Dropdown   | ❌ (Not visible) | ✅              | ❌ (Not visible)  | ✅                 | ✅                | ✅            |
| CP-005       | Checkout Flow         | ✅              | ✅              | ✅                | ✅                 | ✅                | ✅            |
| CP-006       | Order Confirmation    | ✅              | ✅              | ✅                | ✅                 | ✅                | ✅            |
| CP-007       | Invoice View/Download | ✅              | ⚠️ PDF layout issue | ✅           | ✅                 | ⚠️ Opens in new tab only | ✅       |

Legend:  
✅ = Works as expected  
❌ = Fails or major issue  
⚠️ = Minor issue or UI inconsistency

---

## 🌐 Platforms & Devices Covered

| Platform | OS Version          | Browser(s)             |
|----------|---------------------|------------------------|
| Desktop  | macOS Sonoma 14.1.1 | Chrome, Safari         |
| Desktop  | Windows 10 Pro      | Chrome, Firefox        |
| Mobile   | Android 13+         | Chrome (Mobile)        |
| Mobile   | iOS 17+             | Safari                 |

---

## 🔍 Observations

- **Model Year Filter** is not rendering on Chrome in macOS and Windows. This may indicate a browser-specific DOM rendering bug.
- **Invoice Download** works but displays differently on Safari desktop; layout breaks in PDF.
- Responsive behavior is consistent across mobile devices.
- Touch interactions (filter dropdowns, sliders) are fluid on iOS and Android.

---

## 📌 Recommendations

- Investigate and fix browser-specific issues for Chrome’s rendering of Model Year dropdown.
- Validate PDF rendering compatibility across all browsers.
- Continue testing on Edge and older Android/iOS versions for extended coverage.

---

## Related Files

- [Bug Reports](./Bug-reports.md)
- [Functional Scenarios](./functional-scenarios.md)
- [Test Cases](./test-cases.md)

