# Week-2
# Flawed Enforcement of Business Rules – PortSwigger Lab

## Overview

This repository contains the demonstration and solution for the **Flawed Enforcement of Business Rules** lab from PortSwigger Web Security Academy.

The lab focuses on identifying and exploiting a **Business Logic Vulnerability** where discount coupons can be applied multiple times due to improper server-side validation.

By manipulating requests using **Burp Suite**, it is possible to repeatedly apply discount codes and reduce the product price to $0, successfully completing the lab.

---

## Lab Details

- Platform: PortSwigger Web Security Academy
- Category: Business Logic Vulnerabilities
- Tool Used: Burp Suite Community Edition
- Difficulty: Apprentice

---

## Vulnerability

The application fails to properly enforce business rules regarding coupon usage.

### Intended Behavior
- Coupon codes should only be applied once.
- Multiple discounts should not reduce the price below allowed limits.

### Actual Behavior
- Coupons can be repeatedly applied.
- Total product cost can be reduced to $0.
- Order can be placed without paying the original amount.

---

## Attack Steps

1. Login to the lab account.
2. Add the target product to the cart.
3. Open Burp Suite and intercept requests.
4. Apply discount coupons repeatedly.
5. Forward modified requests.
6. Observe continuous price reduction.
7. Complete the purchase at $0.
8. Lab marked as solved.

---

## Tools Used

- Burp Suite
- Google Chrome
- PortSwigger Web Security Academy

---

## Result

Successfully exploited the business logic flaw and completed the lab.

Store Credit Remaining: $100

Final Product Cost: $0

Lab Status: Solved

---

## Learning Outcomes

- Understanding Business Logic Vulnerabilities
- Request Manipulation with Burp Suite
- Coupon Abuse Attacks
- Improper Server-Side Validation
- Secure Business Rule Enforcement

---

## Disclaimer

This repository is created strictly for educational purposes using PortSwigger's legal training environment. Do not attempt these techniques on systems without proper authorization.

## Acknowledgements

Special thanks to RedKross Research Foundation for their support, mentorship, and cybersecurity training resources that contributed to the successful completion of this project.
#redkrossresearchfoundation @redkrossresarchfoundation
