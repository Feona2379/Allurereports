Allure Reporting with TestNG and Selenium

Overview
This project demonstrates the integration of Allure Reporting with TestNG and Selenium WebDriver for generating interactive test reports. The test package 'allureReports' includes automated UI tests for the [nopCommerce demo store](https://demo.nopcommerce.com/), using the Chrome browser.

Features
- Automated UI testing with Selenium WebDriver.
- Test execution with TestNG.
- Integration of Allure Reports for detailed test insights.
- Includes test cases for login, logo verification, and registration.
- Uses WebDriverManager for automatic driver setup.

Prerequisites
Ensure you have the following installed:

- Java 8+
- Maven
- TestNG
- Allure Command-Line Tool

To install Allure CLI:

choco install allure  # Windows (using Chocolatey)
brew install allure   # macOS (using Homebrew)


Project Setup

1. Clone the repository:

git clone https://github.com/yourusername/allure-reporting.git
cd allure-reporting

2. Install dependencies:

mvn clean install

3. Run the TestNG tests:
mvn test

## Generating Allure Reports

After running tests, generate the Allure report with:

allure serve target/allure-results
This command will open an interactive test report in your browser.

## Test Cases

| Test Case          | Description                                 | Status         |
|--------------------|---------------------------------------------|--------------  |
| Logo Presence Test | Verifies that the site logo is displayed.   | ✅ Implemented |
| Login Test        | Attempts login and verifies the page title.  | ❌ Failed      |
| Registration Test | Skipped using SkipException.                 | ⏭ Skipped      |

Technologies Used
- Java
- Selenium WebDriver
- TestNG
- Allure Reporting
- Maven

License
This project is open-source and available under the [MIT License](LICENSE).

---
### Need Help?
For any issues or contributions, feel free to open a pull request or issue on GitHub!


