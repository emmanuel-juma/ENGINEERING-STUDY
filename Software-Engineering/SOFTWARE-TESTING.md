# Objectives of this file 

To Understand the purpose and importance of software testing. 
Differntiate betweeen errors, defects and failures. 
Dive into software testing principles amd the testing lifecycle. 
Explore types of software testing and understand static vs Dynamic testing. 

## FUNDAMENTALS OF SOFTWARE TESTING 

Software Testing is the process of evaluating and verifying that a software product or application does what it is supposed to do. It involves the execution of software/system components using manual or automated tools to evaluate one or more properties of interest. 

## WHY SOFTWARE TESTING MATTERS

Software testing ensures software reliability and functionality before release. It helps identify bugs, reduce development costs and ensure quality. 
Think of it as a necessary safety procedure, similar to a pre-flight inspection for aircarft. 

It plays a crucial role in:

1. Identifying Defects => Catching bus early avoids costly fixes after release. 
2. Improve Quality => It ensures software behaves correctly under expected conditions. 
3. User Satisfaction => Well-tested software earns user trust and satisfaction. 
4. Compliance => Critical in domains where regulations require rigorous validation. 
5. Risk Management => Testing mitigates risks by catching critical issues before deployment. 

## PRINCIPLES OF SOFTWARE TESTING

1. Testing shows Presence of Defects => Testing can demonstrate that defects exist, but note prove there are none. 
2. Exhaustive testing is impossible  => It is not feasible to test all combinations. Focus on high-risk areas. 
3. Early testing => Involve testing activities as early as possible in the software development lifecycle. 
4. Defect Clustering => A small number of modules tend to contain the majority of defects. 
5. Pesticide Paradox => Repeating the same tests will eventually fail to find new, regualarily update and revise tests. 
6. Testing is Context Dependent => Different software requires different testing approaches. 
7. Absence of errors fallacy =>  A software system that does noe fail is not necessarily useful if it doesn't meet user expectations. 


## TYPES OF SOFTWARE TESTING 


1. Functional testing => focuses on the software's operations, checking whether each function works as expected .This includes boundary value analysis, equivalence partitioning, decision tables and state transition testing. 
2. Non-Functional testing => examines how the system behaves under specific conditions. This includes
- Performance testing (speed, scalability)
- Load testing (behavior under expected user load)
- Stress testing (behavior under extreme conditions)
- Usability testing (user-friendliness)
- Security testing (data protection, access control)

3. Regression testing => ensures that new code changes do not negatively affect existing functionalities. 
4. Smoke testing => is a quick, broad test to ensure the basic functions of an application are working before deeper testing begins. 
5. Sanity testing => is focused and narrow, often conducted after mirror changes to validate that a particular function or bug fix works as expected. 

## LEVELS OF SOFTWARE TESTING

1. Unit Testing => This is the lowest level of testing where individual functions, methods or components are tested in isolation. It is usually performed by developers and helps catch bugs early. Tools such as JUnit(Java) or Pytest(python) are commonly used. 

2. Intergration Testing => After unit testing, components are intergrated and their interactions are tested. This ensures data flows correctly between modules and identifies issues like interface mismatches or data format errors. 

3. System Testing => The entire system is tested as a whole yo validate that it meets the specified requirements.
That includes functional testing(what the system does) and non functional testing (how well it does it)

5. Acceptance Testing => This is conducted by the client or end users to ensure the system meets business needs and is ready for deployment. There are two types
- Alpha Testing => (In-house, by users)
- Beta Testing => (real environment, by selected customers)


## TEST ARTIFACTS

Software testing produces several important documents and assets that support and track the testing process

1. Test plan - A formal document outlining the testing scope, strategy, objectives, resources, schedules and deliverables. 
2. Test case - A set of inputs, execution conditions and expected results developed for a particular objective. 
3. Test Script - A set of instructions executed by a testing took (automated testing) or (manual testing).
4. Defect Report (Bug Report) - Documents any issues found during testing, including severity, steps to reproduce and environment in which it was found. 
5. Test Summary Report - An evaluation report at the end of a test cycle, detailing outcomes coverage defects and recommendations. 

## TESTING TECHNIQUES

There are several proven testing techniques used to design effective tests

1. Black-box Testing - Tests functionality without looking at internal code structure. It's based entirely on inputs and expected outputs. 
2. White-box Testing - Tests internal structures or workings of an application. It's used for unit testing and relies on knowledge of the source code. 
3. Grey-box Testing - A hybrid  approach where the tester has limited knowledge of the internal workings of the software. 

Key design techniques include:

- Equivalence Partitioning - Dividing inputs into valid and invalid partitions to reduce the number of test cases. 
- Boundary Value Analysis - Focuses on values at the boundaries of input ranges, where errors often occur. 
- Decision table testing - Represents complex business rules in a tabular form to ensure coverage. 
- State Transition testing - Checks system behavior for different input states and transitions. 
- Use Case Testing - Derived from system use cases to validate end-to-end functionality. 

## AUTOMATION VS MANUAL TESTING 

Manual testing involves human testers executing test cases without automation tools. It is useful for exploratory, usability, and ad-hoc testing, where human judgement. 

Automated testing involves the usage of tools and scripts to perform testing tasks automatically. It is efficient for regression testing, performance testing and large-scale repetitive tasks, common tools include;

1. Selenium for web applications. 
2. Jenkins for CI/CD pipelines. 
3. TestNG, JUnit and postman for API testing. 

Automation saves time in the long run but requires a higher initial investment in scripting and maintainence. 

## TEST COVERAGE AND METRICS

Test coverage refers to how much of the application's code or requirements are covered by the tests. Common cpverage types includes:

1. Code Coverage.  
2. Requirement Coverage. 
3. Test Case Execution Coverage. 

Metrics help quantify testing efforts and quality:

1. Defect Density.  
2. Test Pass percentage. 
3. Mean Time to Detect(MTTD) and Mean Time to repair (MTTR) - Measures of responsiveness and resolution efficiency. 

## TESTING AND AGILE/DEVOPS

Modern development methodologies like Agile and DevOPs have transformed how testing is performed. In Agile, testing is continous and collaborative. Testers work closely with developers and product owners often writing test cases in parallel with requirements using behavior-driven development (BDD) tools like Cucumber. 

In DevOPs, testing is intergrated into the CI/CD pipeline, enabling continous intergration and continous delivery. Automation is essential here and testing occurs at every stage of development to ensure fast, reliable deployments. 
            
## SOFTWARE TESTING LIFE CYCLE ( STLC )    

           The STLC defines phases that help streamline the testing process. 

           |-------------------------------------------|
           |             REQUIREMENT ANALYSIS   | The Engineer review and analyze the requirements to identify testable aspects. 
           |-------------------------------------------|
                                
                                
           |-------------------------------------------|
           |             TEST PLANNING          | Strategies, tools, timelines and scope are defined in a formal test plan. 
           |-------------------------------------------|


           |-------------------------------------------|
           |             TEST CASE DESIGN       | Detailed scenarios and data are created to guide execution. 
           |-------------------------------------------|


           |-------------------------------------------|
           |             TEST ENVIRONMENT SETUP | The System's testing infrastructure is established. 
           |-------------------------------------------|


           |-------------------------------------------|
           |             TEST EXECUTION         | Tests are execution and results logged. Any failures are analyzed. 
           |-------------------------------------------|



           |-------------------------------------------|
           |             DEFECT REPORTING       | Bugs are logged, tracked and communicated to developers. 
           |-------------------------------------------|



           |-------------------------------------------|
           |             TEST CLOSURE           | Final reporting, review of test coverage, defect status and restrospective analysis is performed. 
           |-------------------------------------------|

Software Testing is a vital pillar of software development. It assures quality, improves reliability and fosters user confidence. By Understanding errors, testing principles, test types and lifecycle stages, testers can proactively prevent failures, not just detect them. 

Testing is not just a task - it's a mindset
Mastering it sets you apart a software professional dedicated to building trustworthy technology. 

## DEFECT MANAGEMENT 

- Defect Management is the structured



         
