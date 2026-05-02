| Test ID | API Name | Method | Test Scenario | Expected Result | Actual Result | Status |
|---------|----------|--------|---------------|----------------|---------------|--------|
| API_001 | List Users API | GET | Verify users are returned successfully | Status code 200, response time < 1s, response contains id, name, email fields | Status 200, 212ms, required fields present | Pass |
| API_002 | Single User API | GET | Verify single user is returned successfully | Status code 200, response time < 2s, response contains id = 1, name, username, email | Status 200, 1.08s, required fields present | Pass |
| API_003 | Invalid User API | GET | Verify API returns 404 for non-existing user | Status code 404, empty response body | Status 404, 2.54s, empty body | Pass |
| API_004 | Create User API | POST | Verify new user can be created successfully | Status code 201, response contains created user data and id field | Status 201, 555ms, id=11 returned | Pass |