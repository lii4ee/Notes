# Software Development and Testing
## SDLC
1. **Planning and Requirement Analysis** 
    Business needs and Project feasibility
2. **System Design** 
    Create Architectural and detailed design specification
3. **Implementation**
    Convert Design into source code
4. **Testing and Integration**
    Detect and fix Bugs, Unit, Integration, System testing.
5. **Deployment**
    Deploy to production environment
6. **Maintenance and Updates**
    Monitor performance, ensure stability and scalability.
   
## Agile Development
Relies on frequent collaboration and communication refered as Agile Cerimonies
- **Sprint Planning**
    Product owner prioritizes the backlog,
    Team Selects backlog items to work on,
    Define Sprint
- **Daily Stand Up**
    Developer Team - What is completed yesterday, today, Do I have any Bloackages?
- **Sprint Reviews**
    Showcase Completed Work
    Stakeholder Feedback
- **Sprint Retrospect**
    - Reflect on sprint and improve process what went well,
    - what didn't go well
    - What can we improve
- **Back Refinement**
    - Prepare backlog for future sprints
    - Prioritize and clarity user stories
    - Break large stoeies into smaller teasks
- Release Planning
- Story Kickoff
- Bug Triage
- Spike Discussion

## Agile Methodologies 
  - Scurm - Iterative sprints
  - Kanban - Countinous Delivery with a visual board
  - XP - Extreame programming, frequent releases
  - Lean - Optimizing resources, reducing waste

## Reporting a bug
  - Bug's Title
  - a clear description of the problem
  - steps to reproduce it
  - The Expected Result
  - The Actual Result 

## Roles of Tester in Agile
  - Work closely with dev to understand requirements 
  - Countinously test during dev
  - Automate test where possible 
  - Participate in psrint cremonies
  - Ensure quick feedback to developers

## User Stories
  - A small functionsal requirement written from user's perspective
  - Example
    - As a user, I want to rest my password so that I can regain account access

## Acceptance Criteria
  - Conditions that must be met for the story to be considered completed

## Verification
  - Ensure the product is being built correctly 
  - Meets Design Specification
  - eg
    - Code reviews
    - Static analysis
    - walk through
    - inspection

## Validation
  - Ensures the right prouct is being built
    - Functional testing
    - UAT
    - Executing the code

## Regression testing
  - Ensures the recent changes in the code base do not negatively impact ehe existing functionality 
  - It is performed after bug fix, updates, or enhancement.

## Black box testing
- Does not need the knowledge of the internal code structure
- Focuses on input and output

## White box testing
- Testers have knowledge of the internal working of the application and tests logic, loops and conditions

## Smoke Testing
- A high level test to check if the basic functionality of the application are working

## Sanity testing
- A focused test to verify specific functionality after minor changes or bug fixes

## Test Case 
- A set of steps, inputs, expected results to validate a specific function

## Test Scenario
- A high level description of what needs to be tested withut specific steps

## Severity 
- Impact of the defect on the functionality
  - Critical, high, medium, low

## Priority 
- How urgent the defect needs to be fixed 
  - High, medium, low
*Login button missing (**High severity, high priority**)*

## Performance Testing
- Evaluates the speed, responsiveness and stability of an application under load.
1. Load Testing
   - System Behavior under expected load
2. Stress Testing
   - Pushes system beyond limits to find stability
3. Spike Testing
   - Tests sudden surges in traffic
Tools - Jmeter, load runner

## Software Testing Life Cycle
1. Requirement Analysis 
   - Understand what needs to be tested 
2. Test Planning
   - Creating test Startegy
   - Estimating efforts
3. Test Case Development
   - Writing Test cases 
   - Preparing test data
4. Test Environment Setup
   - Configurating the testing environment
5. Test Execution 
   - Running tests
   - Logging defects
6. Test Closure
   - Documenting lessions learned
   - Finalizing testing

## Defect Life Cycle
1. New - by Tester
2. Assigned - To dev
3. In progress - By Dev
4. Fixed - By Dev
5. Retest - By Tester
6. Closed 
7. Repoen
- Defered
- Rejected 
- Duplicate
- Not a bug

## Functional Testing
- Tests if software works as expected
  - Unit Testing
  - Integration
  - System
  - UAT

## Non Functional Testing
- Performance Testing
- Usability
- Load Testing
- Stress testing
- Security Testing

## Boundary Value Analysis
- BVA is a black box Testing technique where test cases are created for boundary values
  - Min 
  - Max just inside
  - Max just outside
- For a field 1 - 100
  - TC would be
    - 0
    - 1
    - 2
    - 99
    - 100
    - 101

## Equivalence Partitioning
- Divides input data into valid and invalid classes
- So that testing just one value from each class suffices
- For 1 - 100
  - 1 to 100 test 50
  - <1 test -5
  - >100 test 150

## Exploratory Testing
- is an ad hoc testing
- Unscripted approch where testers explore the application without pre defined test cases, relying on intuition and experience

## Aplha Tetsting
- Done by internal teams before Release

## Beta Testing
- Done by external useres before official Launch

## Test Coverage
- Measures how much of the applicationis tested
- Code coverages (lines of code)
- Functional coverage 
- Requirement Coverage

## Test Strategy
- A high level doc outlining the overall approch, principles
- To define the principles followed
- high level guidence
- High level overview 
- Early in project
- overall testing direction

## Test Plan 
- A detalied Doc describing specific activities, resources, schedules and responsibilities
- How, when and what to test
- Detailed instruction
- After Test Strategy

## TDD
- TDD is a development approch where tests are written before writing the actual code.
1. Write a failing test case
2. Write minimal code to pass the test
3. refactor and improve code while ensuring the test still passes
- Benefits
  - Reduces defects early
  - Improve code quality
  - maintainbility

## BDD
- Extents TDD by writing test cases in natural language using Gherkin Syntax
  - Given : 
  - When :
  - Then :
- Benefits
  - Improved collab between testers, developers, business stake holders
  - increases test readability

## Definition of Done
- DOD defines the criteria that must be met before a user story is considered complete
- Eg
  - Code is developed and reviewed 
  - TC are written and passed
  - No critical defects remain
  - Feature is deployed to staging

# Selenium

## Internal Working of Selenium
- after writing automated code
- Selenium webdriver uses
- JSON write protocol with
- HTTP client as a communication handler
- To communicate with the browser
- Then the browser gives the response in the same way.

## Selenium
- Selenium is a open Source automation testing tool used for web application
- Components
  - Selenium IDE
  - WebDriver - Tool used to interact wit browser
    - RC
    - Webdriver
  - Selenium Grid
- Limitation
  - Cannot automate desktop application
  - No buildt in reporting cabalities
  - limited CAPTCHA support 
  - OTP
  - requires 3rd party for handling test management and execution

## Element Locators
1. id
2. name
3. classname
4. tagname
5. link Text
6. Partial Link Text
7. CSS selector
8. Xpath

## findElements() and findElement()
- WebElement throws a exception if nothing is found
- WebElements returns a list, if nothing if found returns a empty list

## Dropdown in selenium
```
Select dropdown = new Select(driver.findElement(By.id("idName")));
dropdown.selectByVisibleText("option1");
dropdown.selectByIndex(2);
dropdown.selectByValue("optionValue");
```

## Alerts
```
Alert alert = driver.switchTo().alert();
alert.accept();
alert.dismiss();
alert.getText();
```

## Frames
```
driver.switchTo().frame("frameName");
driver.switchTo().defaultContent();
```

## Handle multiple Window
```String parentWindow = driver.getWindowHandle();
Set<String> allWindows = driver.getWindowHandles();
for(String window: allWindows)
{
  if(!window.equals(parentWindow))
  { 
    driver.switchTo().window(window); 
  }
}
```

## Implicit Wait
```
driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));
```

## Explicit Wait
```
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
wait.until(ExpectedConditions.visibilityOfElement(By.id("id")));
```

## Fluent Wait
```
Wait <WebDriver> wait = new FluentWait<>(driver)
                                        .withTimeout(Duration.ofSeconds(20))
                                        .pollingEvery(Duration.ofSeconds(5))
                                        .ignoring(NoSuchElementException.class);
WebElement ele1 = wait.until(driver -> driver.findElement(by.id("id")));
WebElement ele2 = wait.until(ExpectedConditions.visibilityOfElement(by.id("id")));
```

## Page Object Model - 
- Design pattern that enhances test maintenance by seprating UI elements and test logic
- By is used 
- Simple Constructor

## Page Factory
- Is a design pattern that suggest to create seprate class for each page
- @FindBy annotation is used
- Enhanced version of POM
```
PageFactory.initElements(driver, this);
```
- is used to initilise in the constructor for webelement

## Screenshot
```
@After
public void Screenshots(Scenario SceneObj)
{
  if(sceneObj.isFailed())
  {
    byte[] screenshot = ((takesScreenshot) drive).getScreenshotAs(OutputType.BYTES);
    sceneObj.attach(screenshot, "image/png", sceneObj.getName());
  }
}
```

## JavaScript Executor
```
JavascriptExecutor js = (JavascriptExecutor) driver;
js.executeScript("window.scrollBy(0,500)"); 
```

## Actions
```
Action action = new Action(driver);
WebElement element = driver.findElement(By.id("id"));
action.moveToElement(element).perform();
```

# Java
## JDK, JRE, JVM
- **JVM**: VM that runs Java byte code
- **JRE**: has JVM and set of libraries needed to run java program
- **JDK**: includes JRE along with tools like compliers and debuggers

## Method overloading vs Overriding 
- Method overloading - Same Method name that has diferent parameters
- Methond overriding - Sub class provides implementation of method in super class with same name and parameters

## String vs StringBuilder vs StringBuffer
- String is immutable 
- StringBuilder is not thread safe meant for single thread thus the fastest
- StringBuffer is thread safe and mutable

## Cheacked exception vs Uncheacked 
- **Checked Exception**:
  - checked at complie time
  - They Must be caught or declared using throws
  - eg
    - IOException
    - SQLException
- **Unchecked Exception**:
  - Occurs at run time 
  - Doesn't needs to be handled
  - eg
    - NullPointerException
    - ArrayIndexOutOfBound

## Interface
- is a reference type similar to class that contains only constants, methods, signatures, default method, static method
- Cannot have instances or constructors
- A class implements an interface to provide implementation for the abstract methods in it

## Super and This
- **This**: Referes to the current object, instance variable, methods or constructor
- **Super**: referes to the superclass (Parent class) 
  - Used to access variables and methods of parent class

## Lambda
- pass a method as an argument to a method without writing a seprate class

## Inheritance:
- allows a class to inherit properties and methods from another class thus promoting re-use and establish relationships
- Extends
- Implements 

## Polymorphism
- Method Overloading
- Method OverRiding

## Encapsuation
- is a concept of wrapping the data and methods that operate on the data into a single class
- It involves controlling access to data by making fields PRIVATE and providing PUBLIC methods (getters and setters) to access or modify them

## Abstraction
- Hiding implementation details and showing only the essential features of a object 
- Achieved using abstract classes and interface

## Abstract class
- cannot be instantiated on its own and must be inherited 
- it can have abstract and non abstract methods

## Interface
- A contract that defines methods that a class must implement

## Java Collections
- Framework that provides architecture 
  - Interfaces
    - List
    - Set
    - Queue
    - Map
    - etc
  - Implementations
    - Arraylist
    - HashSet
    - HashMap
    - PriorityQueue
  - Algorithms
    - Sorting
    - Searching

**Map**: TreeMap, LinkedHashMap
**Set**: HashSet, TreeSet, LinkedHashSet, EnumSet

## Iterator
- Privides a way to traverse through a collection
- hasNext(): Returns true
- next(): teturns the next element

## HashMap vs HashTable
- **HashMap** 
  - allows null values and keys
  - Not snchronized 
  - so not Thread safe
- **HashTable**
  - Synchoronized 
  - thread safe
  - does not allow null keys or values
  - *out dated*

## volatile
- keyword used to indicate variable could be changed by different threads
- permits caching the variable locally in the thread
- is public to all thread.