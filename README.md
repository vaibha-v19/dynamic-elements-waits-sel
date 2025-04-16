# Selenium Dynamic Elements Handling Project

This project is a Selenium-based automation framework designed to demonstrate the handling of dynamic web elements, implementing various wait strategies, and managing exceptions effectively. The framework is built using Java and TestNG, and it utilizes the Page Object Model (POM) design pattern for better maintainability and readability.

## Project Structure

 /DynamicE
│
├── /src
│ ├── /main
│ │ └── /java
│ │ └── objRepo
│ │ └── Home.java # Page Object for the web page
│ │
│ └── /test
│ └── /java
│ └── mPackage
│ └── AppTest.java # Test class containing test cases
│
├── pom.xml # Maven configuration file
└── README.md # Project documentation
## Prerequisites

Before running the project, ensure you have the following installed:

- **Java Development Kit (JDK)**: JDK 8 or higher.
- **Apache Maven**: For managing project dependencies and building the project.
- **Web Browser**: Chrome (or any other browser you wish to test with).

## Setup Instructions

1. **Clone the Repository**: If this project is hosted on a version control system, clone it to your local machine.

   ```bash
   git clone <repository-url>
   cd DynamicE
Install Dependencies: The project uses Maven for dependency management. Run the following command to install the required dependencies:

mvn install
WebDriver Setup: The project uses WebDriverManager to automatically manage the browser driver binaries. Ensure you have an internet connection for WebDriverManager to download the necessary drivers.

Running the Tests
Using Maven: You can run the tests using the following command:

mvn test
Using an IDE: You can also run the tests directly from your IDE (e.g., Eclipse, IntelliJ IDEA) by right-clicking on the AppTest.java file and selecting “Run as TestNG Test”.

Test Configuration
The test is configured to run using TestNG. The configuration file testng.xml can be modified to include additional test classes or parameters if needed.
Test Output
After running the tests, you can find the test results in the target/surefire-reports directory. TestNG generates an HTML report that summarizes the test execution results.
Example Test Case
The main test case is located in AppTest.java and performs the following actions:

Navigates to the web page.
Selects options from a dropdown.
Performs a double-click action.
Handles alerts and verifies their text.
Asserts that the selected options and alert text are as expected.
Conclusion
This project serves as a practical example of how to handle dynamic web elements in Selenium, utilizing effective wait strategies and exception management to create robust automated tests.
