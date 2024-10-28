# confident-spring-01-backend-without-spring
This repository is related to module 1 in Marco Behler's course "The confident Spring professional" https://www.marcobehler.com/ which I purchased in order to understand the fundamentals of Spring. The course starts with plain Java backend and introduces plain Spring features little by little, showcasing what Spring Boot hides under the hood. At the end of the course Spring Boot features are implemented. 

## Learning goals, module 1
In this module a simple backend is created using plain Java w/o any Spring features.    
- Creating pom.xml by hand.  
- Setup Tomcat.  
- Servlet class with endpoints.  
- Service layer.  
- Domain class.  
- Jackson dependency and annotations for handling JSON requests and responses.
- "Poor man's dependency injection" using global Application class.

## Getting Started

To run the application, you have two choices:
1. Run locally
2. Run in Docker

### Locally

1. Ensure all the dependencies are installed
2. Clone the repository  
3. Build the project using Maven: 
    ```sh
    mvn clean install
    ```
4. Run the application with: 
    ```sh
    java -jar target/pdfinvoices-1.0-SNAPSHOT.jar
    ```

### Run in Docker
1. Build the image:
    ```shell
    docker build . -t confident-01:latest     
    ```
2. Run the image:
    ```shell
    docker run -it -p 8080:8080 confident-01:latest 
    ```
3. Open the api in http://localhost:8080

## Documentation
Endpoints for local use:
- GET "/" returns html greeting
- GET "/invoices" returns all posted invoices as JSON
- POST "/invoices?user_id=jeff&amount=40" creates an invoice and returns it as JSON
- POST "/*" returns 404 
