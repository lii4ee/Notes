## Software Development and Testing
### SDLC
1. **Planning and Requirement Analysis** 
    Business needs and Project fesability
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

##