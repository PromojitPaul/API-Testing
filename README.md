# API Testing Automation Project

## About
This project is an **API testing framework** designed to validate the functionality, reliability, performance, and security of APIs. Built using **Postman and RestAssured with Java**, it ensures efficient API automation, covering various testing methodologies like functional, regression, and performance testing. The project follows **SDET best practices** to enhance API quality, maintainability, and CI/CD integration.

## Key Features
- Automated API test execution using **Postman and RestAssured**.
- Validates **GET, POST, PUT, DELETE** API endpoints.
- Implements **data-driven testing** using external JSON/CSV files.
- **Response validation** with assertions on status codes, headers, and body.
- **Authentication testing** (OAuth, JWT, API Key, Basic Auth).
- **Performance testing** using JMeter.
- **CI/CD integration** for automated API validation.
- Detailed **test reports** using Newman, Allure, and Extent Reports.

## Technologies Used
- **API Testing Tools**: Postman, RestAssured
- **Programming Language**: Java
- **Test Framework**: TestNG
- **Build Tool**: Maven
- **Performance Testing**: JMeter
- **Reporting**: Allure, Extent Reports, Newman
- **Version Control**: Git, GitHub
- **CI/CD**: GitHub Actions, Jenkins

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/PromojitPaul/API-Testing.git
   ```
2. Navigate to the project directory:
   ```sh
   cd API-Testing
   ```
3. Install dependencies using Maven:
   ```sh
   mvn clean install
   ```

## Running API Tests
- Execute all Postman API tests using Newman:
  ```sh
  newman run collection.json -e environment.json
  ```
- Run API tests using RestAssured with Maven:
  ```sh
  mvn test
  ```
- Generate Allure reports:
  ```sh
  mvn allure:serve
  ```

## Test Coverage
- **Functional Testing**: Validates API request-response integrity.
- **Security Testing**: Tests authentication and authorization mechanisms.
- **Regression Testing**: Ensures existing APIs work after new updates.
- **Performance Testing**: Evaluates API response time and scalability.
- **Error Handling**: Tests API behavior for invalid inputs and edge cases.

## Folder Structure
```
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── base/             # Base setup for API requests
│   │   │   ├── utils/            # Utility classes for request handling, data management
│   ├── test/
│   │   ├── java/
│   │   │   ├── tests/            # API test scripts
│   │   │   │   ├── GetAPITest.java
│   │   │   │   ├── PostAPITest.java
│   │   │   │   ├── PutAPITest.java
│   │   │   │   ├── DeleteAPITest.java
│   │   │   ├── testdata/         # Test data files (JSON, CSV)
│   ├── resources/
│   │   ├── postman/
│   │   │   ├── collection.json   # Postman test collection
│   │   │   ├── environment.json  # Postman environment variables
│   │   ├── config.properties     # API base URL and credentials
│   │   ├── testng.xml            # TestNG execution configuration
├── reports/                      # API test execution reports
│   ├── allure-results/           # Allure test reports
│   ├── extent-reports/           # Extent report logs
├── logs/                         # API test execution logs
├── pom.xml                        # Maven dependencies
├── README.md                      # Documentation
```

## CI/CD Integration
- Configured **GitHub Actions/Jenkins** for automated API test execution.
- Test execution triggered on **code push or pull requests**.
- Reports generated after test execution for tracking results.

## Conclusion
This **API testing automation** project demonstrates expertise in **API validation, automation frameworks, and CI/CD pipelines**, making it an ideal addition to an SDET/QA portfolio.

## Contact
For more details, explore the repository or connect via GitHub.

