# Lab2
SWT301-Group6-Lab2

# Option A: SpringBoot + Option C: React
Clone the repository:
   ```bash
   git clone https://github.com/doggyB12/Lab2.git
   ```
   or dowloand file and extract.
  
Option A: Spring Boot: Todo API
-----------------------
This is a simple Todo API built with Java and Spring Boot. The application allows users to create, read, update, and delete (CRUD) todo items.
This project file is **Todo-main**.
How to Test:

1) This assignment uses MySql Workbench:
   
   Set the password in MySql Workbench and password default: 12345678
   or you can change password in :
   ```bash
   src/main/resources/application.properties
   in line 5: spring.datasource.password=12345678
   ```
   change to your password setting in MySql Workbench
2) Reload maven in pom.xml.
3) Running the Application
   You can run project and use this link to test api:
   ```bash
   localhost:8080/swagger-ui/index.html
   ```
4) Unit test file
   Test files are in:
   ```bash
   src/test/java/com/project/Todo
   ```
   Test include: Controller, Service, DTO.
   
   Because repository implements from JpaRepository -> maybe do not need to write test. :)
   
   Files include:
   ```bash
       src
       ├── main
       └── test
           └── java
               └── com.project.Todo
                   ├── controller
                   │   └── TodoAPITest.java
                   ├── dto
                   │   └── TodoDTOTest.java
                   └── service
                       └── TodoServiceTest.java
   ```
   To run the Unit Test, in /src/test/java, right click to com.project.Todo -> Run 'Test in 'com.project.Todo''
6) Test Coverage
   To check the test coverage in IntelliJ IDEA:
   
   Right-click on the src/test/java directory or a specific test class.
   
   Select Run 'All Tests' with Coverage or Run 'SpecificTest' with Coverage.
   
   After the tests run, you can view the coverage report.

Option C: React: Todo List Application
-----------------------
This is a Todo List Application using React and Api in java SpringBoot (Option A)
The React project's name is **Task-list-main**
How to test:
1) Run the Java project of the Option A first.
2) Open Task-list-main in Visual Studio Code.
3) Open cmd and input this command to run the React project:
   ```
   npm i jest
   npm i vite 
   npm run dev
   ```
4) Unit test file:
   Test file is in
   ```
   \src\Test
   ```
   To run test file, in cmd input:
   ```
   npm run test:cov
   ```
5) Open terminal and type:
   ```
   npm run test:cov
   ```

Video Links
-------------------
```
[Click here to view the video](https://drive.google.com/file/d/1ao_Zp6KZLEIuPVEi3lGiz9FrLmqzLkMp/view?usp=sharing)
```


