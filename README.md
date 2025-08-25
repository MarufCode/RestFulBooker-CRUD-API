# Restful Booker API - Project

This project demonstrates API testing on the **Restful Booker API**, covering all major HTTP methods (GET, POST, PUT, PATCH, DELETE) along with authentication, payload handling, schema validation, and automation using Postman/Rest Assured.

---

## 📌 API Features

### Public Endpoints
- **Create Booking** – `POST`
  - Fields: `firstname`, `lastname`, `checkin`, `checkout`, `depositpaid`, `additionalneeds`, `phone`
- **Fetch Bookings**
  - Get All Bookings – `GET`
  - Get Booking by ID – `GET`

### Authorized Endpoints
(Only authorized users can perform these actions)
- **Update Booking**
  - Partial Update – `PATCH` (amount, dates, phone number)
  - Full Update – `PUT`
- **Delete Booking** – `DELETE`

---

## 📌 Testing Scope

1. **Endpoints**
   - GET, POST, PUT, PATCH, DELETE
2. **Request Details**
   - **URL** → Base URL + Endpoint + Params
   - **Payload** → JSON Body
   - **Headers** → `Content-Type`, `Accept`, `Cookies`
   - **Authentication** → Identify Auth type (e.g., Basic, Token, etc.)
   - **Request & Response Body**
   - **Response Validation** → Status code, Body, Response time
   - **Schema Validation** → JSON Schema
   - **Security Testing** → Basic checks
3. **Authentication**
   - Required for Update & Delete endpoints
   - Verify supported auth types (Postman supports 11 types)

---

## 📌 Postman

- **Collection** → Organize requests
- **Tests in Postman**
  - Verify response body
  - Verify status codes
  - Validate headers
  - Check response times
  - Auth validation
- **Grouping Requests**
- **Data-Driven Testing**
- **Performance Testing Support**
- **Execution of Test Cases**

⚠️ For large test suites (**200+ cases**), **REST Assured** is preferred over Postman to avoid duplicate code and ensure maintainability.

---

## ✅ Requirements

- **Tools:** Postman, Newman (for CLI execution), or REST Assured (for automation)
- **Languages (optional):** Java / Python
- **Auth Details:** Username, Password, Token (as per API docs)

---

## 📌 How to Run

1. Import API Collection into **Postman**
2. Configure **Environment Variables** (Base URL, Auth)
3. Execute requests manually or via **Newman CLI**
4. Validate responses using inbuilt test scripts
5. For automation, implement with **REST Assured**

---

## 🚀 Future Enhancements

- Automation framework with **REST Assured**
- CI/CD integration with **Jenkins/GitHub Actions**

----

📌 This project helps in learning **API Testing**, **Postman Collections**, **Authentication Handling**, and **REST Assured Automation**.
