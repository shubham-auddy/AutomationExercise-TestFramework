# Requirement Analysis

**Project:** AutomationExercise-TestFramework  
**Application Under Test (AUT):** https://automationexercise.com/  
**Version:** 1.0  
**Prepared By:** Shubham Auddy  
**Date:** July 2026

---

# 1. Introduction

This document captures the functional requirements identified during the analysis of the Automation Exercise web application. The purpose of this document is to identify the application's modules, user flows, business-critical functionalities, automation scope, and assumptions before beginning framework development.

---

# 2. Objective

- Understand the application's functionality.
- Identify automatable features.
- Define the scope of UI and API automation.
- Identify reusable UI components.
- Prepare the foundation for the Test Strategy and Framework Design.

---

# 3. Application Overview

Automation Exercise is an e-commerce demonstration website designed for automation practice. It provides UI workflows and REST APIs covering user authentication, product browsing, shopping cart operations, and account management.

---

# 4. Functional Modules

| Module | Description | Priority | UI Automation | API Automation |
|---------|-------------|----------|---------------|----------------|
| Home | Landing page with featured products and navigation | High | Yes | No |
| Products | Product listing, search, filters, product details | High | Yes | Yes (Search APIs) |
| Product Details | Individual product information | High | Yes | Yes |
| Login | Existing user authentication | Critical | Yes | Yes |
| Signup | New user registration | Critical | Yes | Yes |
| Account Management | Create/Delete account | Critical | Yes | Yes |
| Cart | Shopping cart operations | Critical | Yes | Limited |
| Checkout | Purchase flow | High | Yes | Limited |
| Contact Us | Customer contact form | Medium | Yes | No |
| Subscription | Newsletter subscription | Medium | Yes | No |
| Test Cases | Static navigation page | Low | Yes | No |
| API Testing | API documentation page | Low | Yes | N/A |

---

# 5. Homepage Features

The homepage contains the following components:

- Navigation Bar
- Hero Carousel
- Featured Products
- Product Cards
- Categories Panel
- Brands Panel
- Recommended Products Carousel
- Footer
- Subscription Section
- Scroll-to-Top Button

---

# 6. Product Page Features

The Products page provides:

- Complete product catalogue
- Product search
- Category filtering
- Brand filtering
- Product details navigation
- Add to Cart functionality

---

# 7. User Journeys

### Guest User

- Visit Homepage
- Browse Products
- Search Products
- View Product Details
- Subscribe
- Contact Us

### Registered User

- Login
- Browse Products
- Add Products to Cart
- Checkout
- Logout
- Delete Account

---

# 8. Business Critical Functionalities

The following functionalities have the highest business impact:

- User Registration
- User Login
- Product Search
- Add to Cart
- Checkout
- Account Creation
- Account Deletion

Failure in these modules directly affects user experience.

---

# 9. Reusable UI Components

The following UI elements are common across multiple pages and should be designed as reusable components:

- Navigation Bar
- Footer
- Categories Panel
- Brands Panel
- Product Card
- Search Bar
- Hero Carousel
- Product Carousel

---

# 10. Initial Automation Scope

### UI

- Navigation
- Authentication
- Product Search
- Product Filters
- Cart
- Checkout
- Contact Form
- Subscription

### API

- Products
- Search
- Login
- Signup
- Account Creation
- Account Deletion

---

# 11. Out of Scope

The following items are currently outside the scope of this project:

- Performance Testing
- Security Testing
- Accessibility Testing
- Mobile Automation
- Cross-device Testing
- Database Validation
- Cloud Execution

---

# 12. Assumptions

- The website remains publicly accessible.
- Test data remains stable.
- APIs remain available.
- Browser compatibility is limited to modern browsers.
- Internet connectivity is available during execution.

---

# 13. Risks

- Website data may change over time.
- Product counts may vary.
- UI locators may change.
- APIs may change without notice.
- Network latency may affect execution timing.

---

# 14. Deliverables

The Requirement Analysis document serves as the baseline for:

- Test Strategy
- Framework Architecture
- Test Case Design
- Automation Development
- CI/CD Integration