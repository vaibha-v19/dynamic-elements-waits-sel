Selenium Dynamic Elements Handling Project
Overview
This project is a Selenium-based automation framework designed to demonstrate the handling of dynamic web elements, implementing various wait strategies, and managing exceptions effectively. The framework is built using Java and TestNG, and it utilizes the Page Object Model (POM) design pattern for better maintainability and readability.

Features
Dynamic Element Handling: Interacts with web elements that may change state or visibility during runtime.
Explicit and Implicit Waits: Implements both explicit and implicit waits to ensure that elements are ready for interaction before performing actions.
Exception Management: Catches and handles exceptions gracefully, providing informative error messages and stack traces for debugging.
Page Object Model: Organizes code using the POM design pattern, separating page-specific actions from test logic.
Technologies Used
Java: Programming language used for writing the test scripts.
Selenium WebDriver: Library for automating web browsers.
TestNG: Testing framework for running and managing test cases.
WebDriverManager: Library for managing browser drivers automatically.
Project Structure
/DynamicE
│
├── /src
│   ├── /main
│   │   └── /java
│   │       └── objRepo
│   │           └── Home.java         # Page Object for the web page
│   │
│   └── /test
│       └── /java
│           └── mPackage
│               └── AppTest.java       # Test class containing test cases
│
├── pom.xml                             # Maven configuration file
└── README.md                            # Project documentation
Setup Instructions
Clone the Repository:

git clone <repository-url>
cd SeleniumDynamicElementsProject
Install Dependencies:

Ensure you have Maven installed. Run the following command to install the required dependencies:
mvn install
Run the Tests:

You can run the tests using the following command:
mvn test
Code Explanation
Home.java
This class represents the page object for the web page being tested. It contains methods to interact with the dropdown and the double-click button.

AppTest.java
This class contains the test methods that utilize the Home class to perform actions on the web page. It demonstrates:

Navigating to the web page.
Selecting options from a dropdown.
Performing a double-click action.
Handling alerts and verifying their text.
Wait Strategies
Implicit Wait: Set globally for the WebDriver to wait for a specified time when trying to find an element.
Explicit Wait: Used for specific elements to wait until certain conditions are met (e.g., visibility, clickability).
Exception Handling
The test methods are wrapped in try-catch blocks to handle exceptions gracefully. If an exception occurs, it prints an error message and the stack trace for easier debugging.
