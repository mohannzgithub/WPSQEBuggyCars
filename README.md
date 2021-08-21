Westpac Interview Senior QE(Mohan)
1.	Buggy Car Test approach
2.	Buggy Car Test artifacts (Test plan, Test Scenarios & bug report)
3.	Buggy Car UI and API Test automation
4.	Buggy Car Performance Test

1.Buggy Car Test approach

   1.1 Scope
   The testing approach for this Buggy car rating website shall be done in a fashion that will accommodate the Current functionality in Buggy car rating products being 
   developed for users on Register, login to view Popular Make and Model, and Provide Rankings for their Popular Make and Model by Entering their comments and Voting. 
   
   1.2 Testing levels/Types & Roles and Responsibilities
   
     •	Unit Testing: Developers performed testing through programming on Individual Component  
     •	Integration Testing: Check the Data flow from one module to another module. Manual and Automation tester will perform this via API testing.  
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
         Ex: Test the Secure attribute of the login component, we can then say the 'Login component is Secure When un-authorized user Do NOT have access to Buggy Car ratings’.
      
    •	Acceptance Testing: check the requirements of a specification or contract as per its delivery. UAT /Testing team will perform this testing and the Testing team will help       the UAT team to perform the testing.
