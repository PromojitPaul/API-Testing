# API Testing Project

## About
This project tests APIs using **Postman and RestAssured with Java**. It covers functional, regression, and performance testing to ensure API reliability.

## Features
- Tests **GET, POST, PUT, DELETE** requests.
- Validates responses, status codes, and headers.
- Supports authentication methods (OAuth, JWT, API Key, Basic Auth).
- Runs tests using **Postman and Newman**.
- Generates reports using **Newman and Extent Reports**.
- Integrates with CI/CD pipelines.

## Technologies Used
- **Tools**: Postman, RestAssured
- **Language**: Java
- **Test Framework**: TestNG
- **Build Tool**: Maven
- **Performance Testing**: JMeter
- **Reporting**: Newman, Extent Reports
- **CI/CD**: GitHub Actions, Jenkins

## Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/PromojitPaul/API-Testing.git
   ```
2. Navigate to the directory:
   ```sh
   cd API-Testing
   ```
3. Install dependencies:
   ```sh
   mvn clean install
   ```

## Running Tests
- Run Postman tests with Newman:
  ```sh
  newman run collection.json -e environment.json
  ```
- Run API tests with Maven:
  ```sh
  mvn test
  ```
- Generate reports:
  ```sh
  mvn allure:serve
  ```

## Folder Structure
```
├── src/
│   ├── main/java/
│   │   ├── base/            # API request setup
│   │   ├── utils/           # Utility classes
│   ├── test/java/tests/     # API test scripts
│   │   ├── GetAPITest.java
│   │   ├── PostAPITest.java
│   │   ├── PutAPITest.java
│   │   ├── DeleteAPITest.java
│   │   ├── testdata/        # Test data (JSON, CSV)
│   ├── resources/
│   │   ├── postman/         # Postman collections
│   │   │   ├── collection.json
│   │   │   ├── environment.json
│   │   ├── config.properties # API configurations
│   │   ├── testng.xml        # Test execution config
├── reports/                 # Test reports
├── logs/                    # Execution logs
├── pom.xml                   # Maven dependencies
├── README.md                 # Documentation
```

## CI/CD Integration
- Tests run on **code push and pull requests**.
- Automated test execution using **GitHub Actions/Jenkins**.
- Reports generated after execution.

## Contact
For more details, check the repository or connect via GitHub.

