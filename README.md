# SimpleRestService
This project is a simple RESTful web service built using Spring Boot. It allows users to receive a greeting message that can be customized through a query parameter.

Before you begin, ensure you have met the following requirements:

- **Java Development Kit (JDK) 11** or later installed on your machine.
- **Maven** installed on your machine (optional, but useful for building the project).
- **An IDE** (e.g., IntelliJ IDEA, Eclipse) for editing and running the project.



## Running the Application

### Step 1: Project Initialization

1. Go to [Spring Initializr](https://start.spring.io/).
2. Set the following configurations:
   - **Project:** Maven Project
   - **Language:** Java
   - **Spring Boot:** 2.7.0 (or the latest stable version)
   - **Group:** com.example
   - **Artifact:** simple-rest-service
   - **Name:** SimpleRestService
   - **Package Name:** com.example.simplerestservice
   - **Packaging:** Jar
   - **Java:** 11 (or the version you have installed)
3. **Add Dependencies:**
   - Spring Web
4. Click on **"Generate"** to download the project, then unzip it.

### Step 2: Import Project

1. Open your IDE (e.g., IntelliJ IDEA, Eclipse,vscode).
2. Import the unzipped project as a Maven project.

### Step 3: Create the RESTful Web Service

1. **Model Class:**
   - Create a package named `model` under `src/main/java/com/example/simplerestservice`.
   - Create a Java class named `Greeting` inside the `model` package.
   - Create a Controller:
   - Create a package named controller under src/main/java/com/example/simplerestservice.
   - Create a Java class named GreetingController inside the controller package
     Main Application Class: Ensure that the SimpleRestServiceApplication class is located in the src/main/java/com/example/simplerestservice package.

##  Running and Testing the Application
1. Run the Application:
     o Run the SimpleRestServiceApplication class.
     o The application will start on the default port 8080.
2. Test the RESTful Web Service:
     o Open Postman (or any other REST client).
     o Make a GET request to http://localhost:8080/greeting.
     o You should see a JSON response similar to:
       {
         "id": 1,
         "content": "Hello, World!"
       }
    o Test with a query parameter: http://localhost:8080/greeting?name=John.
    o You should see a JSON response similar to:
       {
        "id": 2,
        "content": "Hello, John!"
       }
