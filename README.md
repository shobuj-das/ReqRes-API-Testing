# ReqRes-API-Testing
This project demonstrates API testing using Postman, providing a collection of tests to validate various endpoints of the API.


##  Features
- Tests for GET, POST, PUT, DELETE requests
- Collection of tests covering different API endpoints
- Environment setup for easy switching between environments
- Pre-request scripts for data setup
- Test scripts for assertions and validations
## API Documentation
https://reqres.in/api-docs/#/
## Technology used:
- Postman
- Newman
## Prerequisite:
- Node Js
- Newman
- Newman Html Report Library
## Installation
1. Postman: If you haven't already, [download and install Postman.](https://www.postman.com/downloads/)
2. Clone the repository:
```
https://github.com/shobuj-das/ReqRes-API-Testing.git
```

3. Import the Postman collection:
   - Open Postman.
   - Click on the Import button.
   - Select the file from the repository.

4. Import the Postman environment:
   - In Postman, click on the gear icon in the top right corner.
   - Select Import and choose the file.

5. Newman and Report Installation Process:
   - Newman Install Command:
   ```
    npm install -g newman
    ```
   - Newman Html Report Install Command:
   ```
    npm install -g newman-reporter-htmlextra
   ```
## Uses

1. Select Environment:
   - In Postman, select the appropriate environment (e.g., Development, Production) from the top-right dropdown.
2. Run Collection:
   - Select the imported collection from the Collections sidebar.
   - Click on the Runner button to open the collection runner.
   - Select the desired environment.
   - Click Start Test to run the collection.
3. View Results:
   - Once the tests are complete, view the results in the Runner tab.
   - Detailed test results can be viewed for each request.

## API End-points
### User
- GET /api/users?page={{page}} — List users
- GET /api/users/2 — Single user (found)
- GET /api/users/23 — Single user (not found → 404)
- POST /api/users — Create user

### Resources (Colours)
- GET /api/unknown — List resources
- GET /api/unknown/2 — Single resource (found)
- GET /api/unknown/23 — Single resource (not found → 404)

### Auth (Simulated)
- POST /api/register — Register (success)
- POST /api/register — Register (missing password → 400)
- POST /api/login — Login (success)
- POST /api/login — Login (missing password → 400)

### Misc
- GET /api/users?delay={{delay}} — Delayed response (simulate loading)

### Newman HTML Report:
<img width="736" height="857" alt="image" src="https://github.com/user-attachments/assets/b3481071-bf28-40fd-8fd6-5f30284b735c" />
<img width="737" height="869" alt="image" src="https://github.com/user-attachments/assets/f2ef3aa7-0443-4288-aa17-a2bec15bcd39" />
<img width="737" height="473" alt="image" src="https://github.com/user-attachments/assets/dbc7351c-13e3-490a-81c2-a7e19c462d71" />


