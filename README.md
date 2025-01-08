# Google Calendar Automation

## Project Overview
This project automates interactions with Google Calendar using Selenium. It focuses on creating, updating, and managing tasks within Google Calendar, along with verifying the functionalities of the Calendar homepage and task management features. The implementation includes dynamic XPath usage and methods for handling a signed Google Chrome instance.

## Scope of Work
The following functionalities have been automated:

1. **Verify Calendar Home Page**: Ensures the Google Calendar homepage is loaded correctly.
2. **Verify Calendar Navigation and Add Task**: Automates navigation through the calendar and adds a new task.
3. **Verify Task Details Updation**: Updates the details of an existing task and validates the changes.
4. **Verify Task Deletion**: Deletes a task from the calendar and confirms its removal.

## Skills Used
- **Selenium**: For browser automation and interaction with Google Calendar.
- **Dynamic XPaths**: To efficiently locate and interact with web elements.
- **Chrome Instance Management**: Utilized methods to handle a signed-in Google Chrome instance for seamless interactions with Google Calendar.

## Prerequisites
- **Java**: Ensure you have Java 8 or higher installed.
- **Selenium WebDriver**: Set up and configured for your project.
- **ChromeDriver**: Compatible with your version of Google Chrome.
- **Maven/Gradle**: For managing dependencies.

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project directory:
   ```bash
   cd google-calendar-automation
   ```

3. Install dependencies (if using Maven):
   ```bash
   mvn install
   ```

4. Download the appropriate version of ChromeDriver from [ChromeDriver Download](https://chromedriver.chromium.org/downloads) and place it in the system's PATH.

5. Configure your Google account to remain signed in for the Chrome instance.

## Execution Instructions
1. Run the test cases using your preferred test framework (e.g., TestNG or JUnit):
   ```bash
   mvn test
   ```

2. Upon execution, the following test cases will be validated:
   - Calendar homepage verification
   - Calendar navigation and task addition
   - Task details updation
   - Task deletion


## Example Dynamic XPath Usage
```java
// XPath to locate a specific task by its title
String taskXpath = "//span[contains(text(),'Task Title')]";
WebElement taskElement = driver.findElement(By.xpath(taskXpath));
```

## Key Challenges
- Handling Google sign-in and maintaining session consistency.
- Managing dynamic element locators due to frequent changes in the Google Calendar interface.
- Efficiently locating and interacting with elements using dynamic XPaths.

## Future Enhancements
- Add support for recurring tasks.
- Extend functionality to include event creation and management.
- Integrate with CI/CD pipelines for continuous testing.

