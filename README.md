# Restful-Booker API Testing Project

This project demonstrates API testing for the Restful-Booker demo API (https://restful-booker.herokuapp.com) using Postman. It covers core CRUD operations including authentication, creating bookings, retrieving bookings, and updating bookings fully or partially.

---

## Project Overview

Restful-Booker is a demo hotel booking API supporting Create, Read, Update, and Delete (CRUD) operations with authentication. This project uses Postman to automate API tests for the following HTTP methods:

- **POST** (Create Booking, Authenticate)
- **GET** (Retrieve Booking details)
- **PUT** (Full update of Booking)
- **PATCH** (Partial update of Booking)

---

## Setup Instructions

1. **Install Postman**

   Download and install Postman: https://www.postman.com/downloads/

2. **Create Postman Environment**

   - Create a new environment named `Restful-Booker`.
   - Add a variable `rb_url` with value `https://restful-booker.herokuapp.com`.

3. **Import or Create Requests**

   Add and configure the following requests in the Postman collection:

   - Authenticate (POST `/auth`) to get token.
   - Create Booking (POST `/booking`).
   - Get Booking (GET `/booking/:id`).
   - Update Booking (PUT `/booking/:id`).
   - Patch Booking (PATCH `/booking/:id`).

4. **Save Requests to a Collection**

   Organize requests under a collection named `Restful-Booker API Tests`.

---

## Running Tests

- Use Postman’s **Tests** tab inside each request to validate response status, body contents, headers, and performance.
- Use the **Collection Runner** to run all requests sequentially as a batch job with automatic test validation.
- Optionally, use Newman CLI for running tests in CI/CD pipelines.

---

## Example Assertions Included

- Status code validations (e.g., HTTP 200 OK).
- Verify presence and correctness of response fields (e.g., `bookingid`, `firstname`).
- Check for JSON response headers.
- Validate response times.

---

## How to Use

1. Select the `Restful-Booker` environment.
2. Run the Authenticate request to obtain a token.
3. Use the token in headers (as `Cookie: token={{token}}`) for update and patch requests.
4. Run requests individually or use the Collection Runner to automate full test execution.
5. Monitor pass/fail status in the Tests tab or Collection Runner results.

---

## Useful Links

- Restful-Booker API: https://restful-booker.herokuapp.com
- Postman Download: https://www.postman.com/downloads/
- Postman Documentation: https://learning.postman.com/docs/

---

## License

This project is provided for learning and API testing practice purposes.

---

*Created by Akib Mahmud*

