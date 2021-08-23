# Westpac Interview Senior QE(Mohan)
1.	Buggy Car Test approach
2.	Buggy Car Test artifacts (Test plan, Test Scenarios & bug report)
3.	Buggy Car UI and API Test automation
4.	Buggy Car Performance Test

# 1.Buggy Car Test approach

   1.1 Scope
   The testing approach for this Buggy car rating website shall be done in a fashion that will accommodate the Current functionality in Buggy car rating products being 
   developed for users on Register, login to view Popular Make and Model, and Provide Rankings for their Popular Make and Model by Entering their comments and Voting. 
   
   1.2 Testing levels/Types & Roles and Responsibilities 
   
     •	Unit Testing: Developers performed testing through programming on Individual Component  
     •	Integration Testing: Check the Data flow from one module to another module. Manual and Automation tester will perform this via API testing.  
     •   Acceptance Testing: check the requirements of a specification or contract as per its delivery.UAT team will perform this testing and the Testing team will help UAT             team to perform the testing.
     •	System Testing: System testing enables testers to ensure that the product meets business requirements, as well as determine that it runs smoothly within its operating           environment. Manual and Automation testers perform the System testing in Dev and QA Environments. I am following the testing technique called ACC (Attribute, 
          component, capability) Matrix for System testing. It is also followed by Google Company as well.        
              Attributes:
              o	Auditable: Test to trace the user transactions.
              o	Accessible: Test the application accessible to those with disabilities and other conditions.
              o	Secure: To test any vulnerability in the application.
              o	Compliance: To test the expected results or any acceptance criteria.
              o	Responsive: Test the application in different browsers and in different screen widths.    
            Components: Components are the modules of the application like Login, Registration, Vote, Popular Make, Popular Model, etc.
            Capability: A capability is the Combination of an attribute and a component
            Ex: Test the Secure attribute of the login component, we can then say the 'Login component is Secure When un-authorized user Do NOT have access to Buggy Caratings’.
            
 # 2.Buggy Car Test artifacts (Test plan, Test Scenarios & bug report)
 
 Please find above attached ACC matrix
 
 ![image](https://user-images.githubusercontent.com/88992582/130419471-432f7574-7028-4ea6-b4c2-37914595414a.png)

 
  Note:
      This document contains three tabs.
      
      Summary: 360 view of the overall testing progress, summary of the test execution including number of open/close defects, number of failed capabilities and total number of       capabilities or scenarios.
      
      Scenarios: Details of each capability/scenario that has been tested, I also have added few comments on the capabilities that have failed.
      
      Defects: this tabs contains a bug report, document is ready to perform a defect triage and keep record of the team conversation around each defect, collaboration is key:)
 
# 3.Test automation
3.1 Test strategy
For this use case I have made use of the testing quadrant and test pyramid, I have break the automation in two projects, one project focus in integration testing validating the API, and the other testing focus at UI or functional level, testing user interactions, since UI test tends to add more cost and maintenance effort, is always a good practice to cover critical functionalities at integration level and use UI automation as functional testing support.

3.2 Automation projects can be found:

 [Integration Test](https://github.com/mohannzgithub/WestpacBuggyCarAPIProject)
 
 [UI Test](https://github.com/mohannzgithub/WestpacBuggycarsUIProject)
 
Note:
Setup instructions can be found on each project

# 4.Performance Testing Approach:
we do the performance test for the API. Prepare the Below performance Workmix template based on the Approximate Usage of the application based on the analytics.

Ex:let's say if 3600 is the target users per hour(THROUGHPUT) then we have below configuration to test API endpoints.

| Syntax | Description |
| ----------- | ----------- |
| Virtual users|	20|
|Time per iteration(secs)|	10|
|Iteration pacing|	20|
|Iterations/hr per vuser|	180|
|Total Iterations/hr|	3600|
