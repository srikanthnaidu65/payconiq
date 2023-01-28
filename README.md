# Payconiq Assignment – Software Engineer
Application
Create a JVM based backend application using REST. That contains the following endpoints:
The initial list of stocks should be created on application start-up. Use a database that is most appropriate for this use-case (Hint: Use Docker and provide user instructions).
The stock object contains at least the following fields:
• ID;
• name (String);
• currentPrice (Amount);
• lastUpdate (Timestamp).
Configure the GET /api/stocks endpoint to support request pagination (the number of stocks per page must be configurable).
Each endpoint must be compliant with the HTTP/1.1 and REST standards. Use Spring Boot to build and test this application.
Nice to have (Optional)
The codebase should have a comprehensive documentation of its API (Ex: OpenAPI). The codebase should target Java 11 or higher.
Implementing the project in Kotlin is a plus.
Implementation
Treat this application as a real MVP that should go to production.
All main use cases must be covered by at least one unit or(and) integration test.

### Run JUnit Tests
```bash
./gradlew clean test --info
```

### Build
```bash
./gradlew clean build
```

### Deploy/Start the application
```bash
java -jar build/libs/stock-1.0.0-RELEASE.jar
```

### GET /api/stocks (get a list of stocks)
```
http://localhost:8081/payconiq/api/stocks?pageNo=5&pageSize=5&sortBy=id
```

### POST /api/stocks (create a stock)
```
http://localhost:8081/payconiq/api/stocks
```

### GET /api/stocks/1 (get one stock from the list)
```
http://localhost:8081/payconiq/api/stocks/100
```

### PATCH /api/stocks/1 (update the price of a single stock)
```
http://localhost:8081/payconiq/api/stocks/19
```

### DELETE/api/stocks/1 (delete a single stock)
```
http://localhost:8081/payconiq/api/stocks/100
```

### API documentation
```
http://localhost:8081/payconiq/v3/api-docs
```

### Swagger UI
```
http://localhost:8081/payconiq/swagger-ui.html
```

#### Please refer the file [Payconiq_Assignment_Tests.pdf](https://github.com/srikanthnaidu65/payconiq/blob/main/Payconiq_Assignment_Tests.pdf) for the test evidences
