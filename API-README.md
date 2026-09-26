# RealBugz API Testing

## Project Overview

This section contains manual API tests performed using Postman against the RealBugz API.

The tests cover CRUD operations and relationships between expeditions, participants, and artifacts.

## Tools

* Postman
* REST API
* GitHub
* HTTP methods: GET, POST, PUT, DELETE
* JSON

## API

**Base URL:** `https://api.realbugz.com/`

**Swagger Documentation:** `https://api.realbugz.com/docs`

## Tested Entities

### Expeditions

* Create expedition
* Update expedition
* Delete expedition
* Retrieve full expedition information

### Participants

* Create participants
* Update participant
* Delete participant
* Verify participant deletion

### Artifacts

* Create artifact
* Verify artifact existence

## Test Cases

| #  | Test Case                     | Method | Result |
| -- | ----------------------------- | ------ | ------ |
| 01 | Create Expedition             | POST   | PASS   |
| 02 | Update Expedition             | PUT    | PASS   |
| 03 | Delete Expedition             | DELETE | PASS   |
| 04 | Create New Expedition         | POST   | PASS   |
| 05 | Create Three Participants     | POST   | PASS   |
| 06 | Update First Participant      | PUT    | PASS   |
| 07 | Delete Third Participant      | DELETE | PASS   |
| 08 | Create Artifact               | POST   | PASS   |
| 09 | Check Full Expedition Details | GET    | PASS   |
| 10 | Delete Expedition             | DELETE | PASS   |

## Test Results

**Total test cases:** 10
**Passed:** 10
**Failed:** 0

**Overall result:** 10/10 tests passed.

## Testing Approach

For each test case:

1. Send the API request using Postman.
2. Verify the HTTP response status.
3. Validate the response body.
4. Compare actual and expected results.
5. Perform additional GET requests when required.
6. Document the test result in GitHub.

## Skills Demonstrated

* REST API testing
* Postman
* CRUD operations
* HTTP methods
* JSON validation
* Status code validation
* API resource verification
* Testing relationships between API entities
* Test documentation
* Git and GitHub
