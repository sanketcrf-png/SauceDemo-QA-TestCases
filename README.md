# Sauce Demo - Comprehensive Manual Test Case Suite

## 📄 Project Artifact
You can view or download the complete, detailed test suite execution sheet here:
👉 **[Click here to view Feb9_ Test Cases for saucedemo.com.pdf](./Feb9_ Test Cases for saucedemo.com.pdf)** 

---

## 🔍 Project Overview
This repository hosts a meticulously structured manual test suite executed against **[Saucedemo.com](https://www.saucedemo.com/)**. The test cases span across multiple core modules, focusing on Functional Validation, UI/UX consistency, Security/Session boundaries, Error Handling, and Device Responsiveness.

### Modules Tested
* **Login Page (`login.html`):** Verified input behavior (masking, placeholders), negative workflows (blank/invalid inputs), and UI formatting (error box wrapping).
* **Products Page (`inventory.html`):** Tested sorting mechanisms (A-Z, Z-A, Price Low-High), cart counter badge persistence, hover attributes, and session timeouts.
* **Global Header & Footer:** Validated responsive side navigation panels, App State resets, social media cross-linking, and header positioning properties.
* **Shopping Cart (`cart.html`):** Ensured URL persistence, item absolute state values, direct address bar access restrictions, and empty state behaviors.
* **Checkout Journey (`checkout-step-one.html` & `two.html`):** Tested form validations, field characters/lengths (postal codes), billing summary accuracy, and checkout completion.

---

## 🛠️ Testing Matrix & Parameters
The suite evaluates individual test components utilizing the following structural architecture:
* **Test IDs Assessed:** `TC_001` through `TC_026` + Header specialized cases (`TC_H_001` - `TC_H_014`).
* **Design Techniques:** Boundary Value Analysis (BVA), Equivalence Partitioning, Negative Testing, and State Transition.
* **Device Responsiveness Profiles:** Tested layouts against specific hardware breakpoints:
  * iPhone 14 Pro ($430 \times 932$)
  * Samsung Galaxy S20 Ultra ($412 \times 915$)
  * iPad Pro ($1024 \times 1366$)

---

## 📈 Key Defect Deficiencies Discovered (Sample Bugs Logged)
During execution, several unexpected deviations from expected behaviors were documented:
1. **Security / Masking Failure (`TC_014` - Login):** Password characters masked using a period (`.`) configuration instead of standard asterisk symbols (`*`).
2. **Missing Validation Handling (`TC_020` - Login):** Leaving username and password fields blank triggered an inconsistent `"Username is required"` message instead of the expected unified error block.
3. **UI / Structural Errors (`TC_H_013` - Header):** Global header element fails to maintain a fixed position during deep vertical scrolling, becoming inaccessible to users.
4. **Voucher Validation Defect (`TC_011` - Checkout Step Two):** Promised universal payment gateways (Apple Pay, PayPal) and promotional voucher/coupon fields were completely absent from the final overview sheet layout.
