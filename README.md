![AutoCare Logo](https://autocare.sgp1.cdn.digitaloceanspaces.com/media/site_logo/F-2.png)

#  AutoCare-BD - QA Assessment Repository

This repository presents a structured **Quality Assurance (QA) assessment** for the AutoCare platform — a Bangladeshi online vehicle service and parts marketplace. The purpose of this repo is to showcase professional QA work including **functional scenarios, bug reports, cross-platform behavior**, and **test cases**.

---

##  About the Platform

**AutoCare** simplifies vehicle maintenance by allowing users to:

- Order automotive products and parts online
- Book vehicle-related services
- Manage bookings and deliveries through web and mobile platforms (Android/iOS)

---

## 📁 Folder & File Structure

```bash
AutoCare-BD/
├── screenshots/ # Visual references for reported bugs
├── bug-reports.md # Documented bugs with environment & severity
├── cross-platform-tests.md # Testing results across OS/devices
├── functional-scenarios.md # Realistic functional QA scenarios
├── summary-of-product.md # Overview of the platform and its use cases
├── test-cases.md # Structured QA test cases with shared spreadsheet link
├── ui-observations.md # UI/UX improvement recommendations with examples
└── README.md # This file
```
---

## Quick Access

Click below to jump directly to each section:

- [🪲 Bug Reports](./bug-reports.md)
- [🌐 Cross Platform Tests](./cross-platform-tests.md)
- [⚙️ Functional Scenarios](./functional-scenarios.md)
- [📘 Summary of Product](./summary-of-product.md)
- [🧪 Test Cases](./test-cases.md)
- [🎨 UI Observations](./ui-observations.md)

---
---

##  Key QA Artifacts

###  Functional Scenarios
Detailed walkthrough of QA use cases such as login, service booking, checkout flow, etc.

###  Bug Reports
UI, UX, and logic-related bugs with reproduction steps, screenshots.

### 🔀 Cross-Platform Testing
Results of platform behavior on:
- Windows 10 Pro (Chrome)
- macOS Sonoma 14.1.1 (Chrome)
- Android 15
- Display 14" & 22" monitor

> _Note: iOS was **not** tested during this assessment._

###  Test Cases
Test cases in tabular format including priority, test steps, expected vs actual results, and outcomes.

> 📎 **Test Case Sheet Link:** [Google Sheet](https://docs.google.com/spreadsheets/d/13hWKZHAP3dk51rsRNiN7ko92wRzPcQMa-eQKh0m93kk/edit?gid=1140583909#gid=1140583909)

---

## 🌐 Platforms Under Test

| Platform | Link |
|---------|------|
| Website | [https://autocare.com.bd/](https://autocare.com.bd/) |
| Android | [App Info](https://ison.com/topic/learn/142459/the-art-of-facilitation) |
| iOS     | [App Store](https://apps.apple.com/us/app/autocare-user/id6739961744) |

---

## 🧩 Recommendations

While testing, multiple UI and functional issues were found. The following improvements are recommended:

- Implement year-selector-first behavior in Date of Birth input.
- Add a cancel option in the order module.
- Ensure service order notifications trigger consistently.
- Improve mobile responsiveness and layout alignment in service detail views.
- Consider QA involvement during feature rollout to ensure end-to-end stability.

---

## 🙌 Contributing

Want to contribute or report a new issue? Feel free to fork the repo and submit a pull request, or raise an issue.
---

## 👨‍💻 Author

## Jubair Rahman  
### Software QA Engineer  


## 📬 Contact Me

[![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discordapp.com/992437670884151338) [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JubairRahman) [![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jubair-rahman0/) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jubairrahman64@gmail.com) [![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/8801645763353) [![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white)](https://www.facebook.com/thejubairjubu)


---

> ⚠️ _This project is for demonstration and assessment purposes only and is not affiliated with AutoCare official development._
> 🛠 Maintained with care by Jubair Rahman – Software QA Engineer

