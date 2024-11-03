# SQT-Porject
American International University-Bangladesh (AIUB) Department of Computer Science Faculty of Science &Technology (FST) FALL 22-23
Section: F Software Quality Assurance and Testing
STUDENT MANAGEMENT SYSTEM
Report Submitted By
SN Student Name Student ID
1
MD. RABBI ISLAM SAJID
20-42181-1
2
ASIF ZAMAN
20-42212-1
3
TAMIMUL ALAM
20-42215-1
4
MEHADI HASAN SHOJIB
20-42713-1
Under the supervision of
ISRAT JAHAN MOURI
Assistant Professor
Department of Computer Science
Faculty of Science & Technology
American International University-Bangladesh
Software Test Plan
for
Student Management System
Version 1.0 approved
Prepared by,
Md. Rabbi Islam Sajid
Asif Zaman
Tamimul Alam
Mehadi Hasan Shojib
American International University-Bangladesh
25th December, 2022
Checked By Industry Personnel
Name:
Designation:
Company:
Sign:
Date:
Table of Contents
Revision History .............................................................................................................................3
1. TEST PLAN IDENTIFIER:RS-MTP01.3 ............................................................................4
2. REFERENCES .........................................................................................................................4
3. INTRODUCTION....................................................................................................................4
Background to the Problem ...................................................................................................................... 4
Solution to the Problem ............................................................................................................................ 4
4. REQUEIREMNT SPECIFICATION ....................................................................................5
4.1 System Features ............................................................................................................................ 5
4.2 System Quality Attributes ............................................................................................................. 7
5. FEATURES NOT TO BE TESTED .......................................................................................8
6. TESTING APPROACH ............................................................................................................8
6.1 Testing Levels .................................................................................................................................. 8
6.2 Test Tools ........................................................................................................................................... 9
6.3 Meetings ........................................................................................................................................... 11
7. TEST CASES/TEST ITEMS ..................................................................................................12
8. ITEMS PASS/FAIL CITERIA ...............................................................................................38
9. TESTING SCHEDULE ...........................................................................................................38
Revision History
Revision
Date
Updated by
Update Comments
0.1
2022.12.20
Md. Rabbi Islam Sajid
First Draft
0.2
2022.12.21
Tamimul Alam
Second Draft
0.3
2022.12.22
Asif Zaman
Third Draft
0.4
2022.12.23
Mehedi Hasan Shojib
Fourth Draft
0.5
2022.12.24
Tamimul Alam
Fifth Draft
0.6
2022.12.25
Md. Rabbi Islam Sajid
Sixth Draft
1. TEST PLAN IDENTIFIER:RS-MTP01.3
2. REFERENCES
o https://www.eskooly.com/
o Software Engineering Course Slide
o Software Quality and Testing Course Slides
o Selenium Testing Files Provided by Course Teacher
3. INTRODUCTION
Background to the Problem
1) Student management is becoming a fundamental requirement in education in the present era, and it automates every daily task carried out in the school, college, and university. This technology allows us to swiftly gather all the data required for management. The primary goal is to develop software that will manage these many modules. What is the root cause of this problem? why is this problem is so important to consider?
2) Eskooly is the company we've chosen. The system can dynamically manage and save student, faculty, and teacher information. The suggested strategy provides the most straightforward method for managing all facets of student and university management. The program enables exploration of all internal activities that students are unaware of taking place at the school, college, or institution.
Solution to the Problem
The activities of students and teachers are provided by our system. With the use of this system, users may handle things like student information, grade data, registration, class schedules, notes, and payments. We are making sure that student data is secure. Our main offerings include
1) Result and Academic Transcript
2) Accounts
3) Online Admission
4) Messaging System
5) Students/Parents Login
6) Student Manager
3) We have a strong desire to offer first-rate service. Since ensuring customer satisfaction is our top priority, we also provide our training, operational management, professional skill, and recruitment divisions special attention.
Since ensuring customer satisfaction is our top priority, we also provide our training, operational management, professional skill, and recruitment divisions special attention.
4) Information on students, instructors, and teachers can be stored and managed by our business, eSkooly. Arena Phone Bd Ltd produced the cloud-based eSkooly application. It features SMS service and mobile apps. The use of eSkooly is free for educational institutions. It allows staff members to efficiently complete their regular duties and keep an eye on a variety of other institutional operations. In addition, parents are updated on their children's growth.
4. REQUEIREMNT SPECIFICATION
4.1 System Features
1. Software Features
Functional Requirements
1.1 The user login into the software with their username and password.
1.2 If the login successful the main home page in this software will be displayed.
1.3 If the user forgets the username and password so they can be reset password
using their valid email address and phone number.
1.4 If the user input 3 times wrong password, the system will block the user account
login for half one hour.
Priority level: High
Precondition: User have valid username and password.
Cross-references: None
2. Admin
Functional Requirements
2.1 Monitoring user information by maintaining accurate database of all ID.
2.2 If the user is valid based on his/her information then “activate” card otherwise
“reject” and report to the user.
2.3 Admin will able to see the payment status. If paid then allow to request otherwise report to the user for payment. After reporting 2 times if user doesn’t
pay then admin can deactivate the user ID.
Priority level: High
Precondition: Admin must have the rights to access the whole system.
Cross-references: 1.1, 1.2, 3.1
3. Accounts
Functional Requirements
3.1 The payment transaction will be done using user ID.
3.2 The payment slip can be gotten from the account department using ID.
3.3 Then the payment information will show in the portal.
Priority level: High
Precondition: Payment system must be pay using user ID.
Cross-references: 2.1, 2.2, 2.3
4. Search
Functional Requirements
5.1 User can search for what service he/she expecting.
5.2 System gives user review of their expecting service.
5.3 User can also search for the information (Admission, Cost and Other details).
Priority level: Medium
Precondition: Must be in logged in condition
Cross-references: 5.1, 6.2
4.2 System Quality Attributes
There are some quality attributes that are very important to ensure the quality of a software.
Usability: Any skilled user should be able to register and login to the system.
Efficiency: Each and every functional need must be fulfilled.
Portability: This will be capable of running properly on all the devices.
Maintainability: If any issue locates or detect in the system then it will be possible to fix
it.
Correctness: Mentioned all features will be completed according to the preferences of
the patients.
Functionality: Will display available slot list, their details and it will also show if they
are parking or not.
Accessibility: It’s a web-based software so it will be accessible from anywhere on the
Internet.
Readability: It's critical to rely on appointment software to properly and containing
accurate scheduling demands. It is so important to check to see if the system is durable
enough to sustain any situation. So, regular counting on parking slot.
Reliability: All features will perform in various working environments or devices. o
Flexibility: Will flexible enough to modify in terms of any needs.
Integrity/Security: System integrity or security should be sufficient to prevent
unauthorized access to system functions, information loss, and virus infection of software,
as well as to protect the privacy of data entered into the system. Actually, Integrity comes
with security
5. FEATURES NOT TO BE TESTED
The following is a list of the areas that will not be specifically addressed. All testing in these
• areas will be indirect as a result of other testing efforts. For example:
• How to perform our application under low network that will not be tested.
• External functionality over the program is not supported by this system. As a result,
• application to server testing should be avoided.
• Browser compatibility
6. TESTING APPROACH
6.1 Testing Levels
UNIT Test: The fundamental level of testing is the unit test. After creating each feature,a developer will verify that it functions as intended inside the component design. Because
they are the ones who understand how these specific features functioned and because
they are familiar with internal logic, program structure, etc., developers will perform this
testing. In our application, the developer will conduct UNIT testing, and the development
team leader will provide their approval. Before unit testing is accepted and handed off to
the tester, the programmer must show the team leader proof of it (test case list, sample
output, data printouts, defect information). The test person will also receive access to all
unit test data.
Integration Test: The second level of testing is integration testing. the present level. The
modules or features will be linked together one at a time. The leader of our development
team will oversee this testing and determine whether or not the data transmission between
these modules is accurate. At this level, we'll use strategies like the sandwich strategy,
big bang approach, bottom-up integration, and top-down integration.
System Test: Our quality assurance team will carry out this testing level once the unit
test and integration test have been completed. Our quality team will check the complete
system against the customer's specification once our full program has been developed.
These testing methods are known as black boxes. Various testing methods will have been
used at this testing level. In addition to performing functional testing, our testing team
also performs nonfunctional testing such as volume, load, and performance testing.
Acceptance Test: We will move on to the acceptance testing level once our entire
application has been completed and the first three levels have been tested. At this stage,
the test team leader will work with the end user to evaluate our product. In essence, we
will check the software's usability and functionality. We will ensure that our system
satisfies all user requirements after this testing phase.
6.2 Test Tools
The ‘Selenium IDE’ – testing tool has been used to build test cased and test our website.
Selenium IDE has been used because it supports automated testing. We will perform manual testing initially, and then we will perform automation testing. The most crucial tool for automation testing is Selenium. Selenium is an open-source, free framework for assessing web applications across a variety of platforms and browsers. Scripts for Selenium tests can be written in a variety of programming languages, including Java, C#, Python, and others. However, we'll be automating our testing using Java. Below are a few screenshots of selenium.
Fig-1
Fig-2
Fig-3
Fig-4
6.3 Meetings
In order to discuss about the project, we must go through group meetings. We used Discord to arrange our virtual meetings. We also organized some in person meeting at university. Before the group meeting we all prepared each of our stand alone plan for the project. In the meeting we had decided to follow the best plan. We equally shared our work in this project. The meetings were often organized to keep updating our work
7. TEST CASES/TEST ITEMS
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_1 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): High Test Executed by: Tamimul Alam Module Name: Registration Session Test Execution date: 24/12/2022 Test Title: Successful Registration Check Description: Test website’s Registration Page and storing username and password to the database. Precondition (If any): Must land on sign up page from website homepage successfully. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Click on signup 3. Enter E-mail 4. Enter password 5. Enter_Confirm password 6. Accept terms and condition button 7. Click signup button E-mail: tamim@gmail.com Password: 56565656 Confirm Password: 56565656
User should register successfully to the website As expected, Pass Post Condition: User is registered with database and can be log in later.
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_2 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): High Test Executed by: Tamimul Alam Module Name: Registration input field validation Test Execution date: 24/12/2022 Test Title: Registration Field Validation Check Description: Test website’s Registration Field Precondition (If any): Must land on sign up page. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website’s signup page 2. Skip E-mail’s field 3. Enter password 4. Enter confirm password 5. Accept terms and condition button 6. Click signup button 7. Clear the confirm password input field 8. Enter Confirm password 9. Enter E-mail 10. Didn’t click terms and condition button 11. Click signup button E-mail: aiub@gmail.com Password: 23232323 Confirm Password: 23232323 User should not register successfully to the website and must show a message Result not as expected, Fail Post Condition: User isn’t registered with database and can’t be log in later.
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_3 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): Medium Test Executed by: Tamimul Alam Module Name: Registration input field functionality 1.0 Test Execution date: 24/12/2022 Test Title: Registration’s E-mail Pattern Validation Checking Description: Testing username field functionality as an e-mail’s pattern validation Precondition (If any): Must land on sign up page. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website’s signup page 2. Enter E-mail 3. Enter password 4. Enter confirm password 5. Accept terms and condition button 6. Click signup button E-mail: sqtgmail Password: tamim Confirm Password: tamim
User should not register successfully to the website Result not as expected, Fail Post Condition: User can’t be registered.
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_4 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): High Test Executed by: Tamimul Alam Module Name: Registration input field functionality 1.1 Test Execution date: 24/12/2022 Test Title: signup password/confirm password input field validation Description: Testing password/confirm password field in signup page Precondition (If any): Must land on sign up page. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website’s signup page 2. Enter E-mail 3. Enter password 4. Enter confirm password 5. Accept terms and condition button 6. Click signup button E-mail: alamin@gmail.com Password: 25698 Confirm Password: 25478
User should not register successfully to the website Result not as expected, Fail Post Condition: User isn’t registered with database and can’t be log in later.
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_5 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): Medium Test Executed by: Tamimul Alam Module Name: Registration UI/UX check session Test Execution date: 25/12/2022 Test Title: Signup page’s button check Description: Testing Signup page’s all button Precondition (If any): Must land on sign up page. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website’s signup page 2. Click on sign up button 3. Click on Terms & Conditions button 4. Click on login button 5. Back to sign up page by clicking (I do not have an account yet) 6. Click on eSkooly logo
N/A All the buttons should work properly As expected, Pass Post Condition: User can easily land any page from signup page by clicking signup page’s buttons.
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_6 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): High Test Executed by: Tamimul Alam Module Name: Registration input field functionality 1.2 Test Execution date: 25/12/2022 Test Title: Registration’s existing e-mail validation Checking Description: Testing email field functionality as existing e-mail’s validation Precondition (If any): Must land on sign up page and at least one email should be registered in the database Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website’s signup page 2. Enter an existing e-mail
E-mail: tamim@gmail.com User should not register successfully to the website As expected, Pass Post Condition: Must show a warning message.
Project Name: Student Management System Test Designed by: Tamimul Alam Test Case ID: FR_7 Test Designed date: 23/12/2022 Test Priority (Low, Medium, High): Medium Test Executed by: Tamimul Alam Module Name: Registration session Test Execution date: 25/12/2022 Test Title: Employee’s account registration Description: Testing a successful registration of Employee’s account and storing username and password to the database. Precondition (If any): Must land on login page and have an admin’s account. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Enter admin username 4. Enter admin password 5. Click submit 6. Click on employee 7. Add new 8. Enter name of employee 9. Enter mobile number 10. Enter joining date 11. Enter salary 12. Enter father’s name 13. Enter CNIC 14. Enter education qualification 15. Enter gender 16. Enter religion 17. Enter Employee’s email 18. Enter blood group 19. Enter previous job experience 20. Enter Date of birth 21. Address 22. Click on submit
E-mail: tamim@gmail.com Password: 56565656 Employee’s name: Prottoy Rahman Number: 01711111111 Joining date: 2002-12-14 Salary: 25000 Father’s name: Tamim Rahman Gender: Male CNIC: 2500 Employees’ email: Example1@gmail.com Education: BSc Blood group: A+ Date of birth: 2022-12-06 Address: West Kazipara
Admis should register employees’ account successfully to the website As expected, Pass Post Condition: Employee’s account is registered with database and can be log in later using provided username and password
Project Name: Student Management System Test Designed by: Md. Rabbi Islam Sajid Test Case ID: FR_8 Test Designed date: 23-12-22 Test Priority (Low, Medium, High): High Test Executed by: Md. Rabbi Islam Sajid Module Name: Login Session Admin Test Execution date: 24-12-22 Test Title: Successful Login Check Description: Test website login page for user- Admin Precondition (If any): User must have valid username and password Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Enter admin username 4. Enter admin password 5. Click submit Username: admin@gmail.com Password: admin00 User should login into the application As expected, Pass Post Condition: User is validated with database and successfully login to account. The account session details are logged in the database.
Project Name: Student Management System Test Designed by: Md. Rabbi Islam Sajid Test Case ID: FR_9 Test Designed date: 23-12-22 Test Priority (Low, Medium, High): High Test Executed by: Md. Rabbi Islam Sajid Module Name: Login Validation 1.0 Test Execution date: 24-12-22 Test Title: Login with Incorrect Credentials Description: Checking for log into admin account with incorrect username and password Precondition (If any): Must be on the Login page. Username and password must be registered in the database before checking Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Enter incorrect admin username 4. Enter incorrect admin password 5. Click submit Username: rabbi1234@yahoo.com Password: 789456123 User shouldn’t be log in to different accounts As expected, Pass Post Condition: Must be shown Incorrect username and password after login
Project Name: Student Management System Test Designed by: Md. Rabbi Islam Sajid Test Case ID: FR_10 Test Designed date: 23-12-22 Test Priority (Low, Medium, High): High Test Executed by: Md. Rabbi Islam Sajid Module Name: Login Validation 1.1 Test Execution date: 24-12-22 Test Title: Login Validation Different Users Description: Checking for log into different users with same username and password Precondition (If any): Username and password must be registered in the database before checking Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Enter admin username into employee username 4. Enter admin password into employee password 5. Click submit Username: admin@gmail.com Password: admin00 User shouldn’t be log in to employee accounts As expected, Pass Post Condition: User must have different username and password for log into different accounts.
Project Name: Student Management System Test Designed by: Md. Rabbi Islam Sajid Test Case ID: FR_11 Test Designed date: 23-12-22 Test Priority (Low, Medium, High): High Test Executed by: Md. Rabbi Islam Sajid Module Name: Login and Logout Session Test Execution date: 24-12-22 Test Title: Login and Logout Functionality Description: Checking the login and logout functionality working successfully Precondition (If any): Must be on the Login page. Username and password must be correct. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Enter correct username 4. Enter correct password 5. Click submit 6. Click logout Username: teacher@yahoo.com Password: teacher1 User should be able login and logout successfully As expected, Pass Post Condition: Same as precondition
Project Name: Student Management System Test Designed by: Md. Rabbi Islam Sajid Test Case ID: FR_12 Test Designed date: 23-12-22 Test Priority (Low, Medium, High): High Test Executed by: Md. Rabbi Islam Sajid Module Name: Login Functionality Session Test Execution date: 24-12-22 Test Title: Login Credential Functionality Description: Checking the credentials functionalities working properly or not Precondition (If any): Must be on the Login page. Username and password should be incorrect format Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Enter incorrect username format 4. Enter incorrect password format 5. Click submit Username: student@yahoo Password: 123 User shouldn’t be able to login Not as expected Fail Post Condition: Must give warning while giving incorrect information’s
Project Name: Student Management System Test Designed by: Md. Rabbi Islam Sajid Test Case ID: FR_13 Test Designed date: 23-12-22 Test Priority (Low, Medium, High): Medium Test Executed by: Md. Rabbi Islam Sajid Module Name: Login Feature Session Test Execution date: 24-12-22 Test Title: Login Forgot Password Feature Checking Description: Checking forgot password option working properly or not Precondition (If any): Must be on the Login page. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to the website 2. Go to login page 3. Click forgot password 4. Enter correct username 5. Click reset password Username: admin@gmail.com
User should be able to reset password and get login info in email As expected, Pass Post Condition: User should get login information’s via email
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_14 Test Designed date: 20-12-22 Test Priority (Low, Medium, High): High Test Executed by: Asif Zaman Module Name: Employee addition feature Test Execution date: 25-12-22 Test Title: Add employee with valid input Description: Checking the addition of a new employee by providing the valid information in both required and optional section of the employee form Precondition (If any): Must be landed on the dashboard page. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Enter employee name 6. Enter mobile no 7. Enter joining date 8. Enter employee-type 9. Enter monthly salary 10. Enter father name 11. Enter CNIC 12. Enter education 13. Enter gender 14. Enter religion 15. Enter blood group 16. Enter experience 17. Enter email 18. Enter date of birth 19. Enter address 20. Click on submit
Name: Sajid Mob no: 01824500704 Joining-date:1998-02-26 Employee-type: Teacher Monthly-salary:10000 Father-name: Rahim CNIC:3123 Education: AIUB Gender: Male Religion: Islam Blood group: A+ Experience: Teaching Email:sajid@gmail.com Date of birth:2022-12-1 Address:Uttara Bangladesh User must be registered as an employee As expected, Pass Post Condition: The registered user got a new role as an employee in the website. The data must be stored into the database
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_15 Test Designed date: 20-12-22 Test Priority (Low, Medium, High): High Test Executed by: Asif Zaman Module Name: Employee form validation 1.0 Test Execution date: 25-12-22 Test Title: Add employee with invalid input Description: Checking the addition of a new employee by providing the invalid information in required section of the employee form Precondition (If any): Must be landed on the employee form page during the addition of the new employee. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Enter employee name 6. Enter mobile no 7. Enter joining date 8. Enter employee-type 9. Enter monthly salary 10. Click on submit
Name: 1234 Mob no: 01644412678 Joining-date:2022-12-1 Employee-type: other Monthly-salary: -9000 Father-name:Null CNIC: Null Education: Null Gender: Null Religion: Null Blood group: Null Experience: Null Email: Null Date of birth: Null Address: Null Employee should not able to be registered. Not as expected, Fail Post Condition: The registered user will not able to add as an employee. A warning must be showed for the invalid name and the invalid salary
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_16 Test Designed date: 20-12-22 Test Priority (Low, Medium, High): High Test Executed by: Asif Zaman Module Name: Employee form validation 1.1 Test Execution date: 25-12-22 Test Title: Add employee with invalid mobile no Description: Checking the addition of a new employee by providing the invalid mobile no in the required section of the employee form Precondition (If any): Must be landed on the employee form page during the addition of the new employee. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Enter employee name 6. Enter mobile no 7. Enter joining date 8. Enter employee-type 9. Enter monthly salary 10. Click on submit
Name: Invalid phone, String number Mob-no:Null, String_)(*&^&^^% Joining-date: 2022-12-1, 2022-12-1 Employee-type:Store manager, Other Monthly-salary: 3000,2000 Father-name: Null CNIC: Null Education: Null Gender: Null Religion: Null Blood group: Null Experience: Null Email: Null Date of birth: Null Address: Null Employee should not able to be registered. Not as expected, Fail Post Condition: The registered user will not able to add as an employee and not add the information to the database. A warning need to be showed for the null input in the required section and the invalid string input as the mobile number.
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_17 Test Designed date: 20-12-22 Test Priority (Low, Medium, High): High Test Executed by: Asif Zaman Module Name: Employee form validation 1.2 Test Execution date: 25-12-22 Test Title: Add employee without other required input Description: Checking the addition of a new employee without providing the inputs in the required section of the employee form Precondition (If any): Must be landed on the employee form page during the addition of the new employee. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Land on the employee form section 6. Enter mobile number 7. Enter employee name, employee type and salary keeping joining date empty 8. Enter joining date, employee type and salary keeping employee name empty 9. Enter employee name, joining date, and salary keeping employee type empty 10. Enter employee name, joining date, employee type keeping salary empty 11. Click on submit Name: test_req, Null Mob-no: 01824500704 Joining-date:Null, 2022-12-1 Employee type: Other, Null Monthly-salary: 1000,Null Father-name: Null CNIC: Null Education: Null Gender: Null Religion: Null Blood group: Null Experience: Null Email: Null Date of birth: Null Address: Null Employee should not able to be registered. As expected, Pass Post Condition: The blank textboxes in required information must show the warning and new employee is not registered or not added to the database.
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_18 Test Designed date: 22-12-22 Test Priority (Low, Medium, High): High Test Executed by: Asif Zaman Module Name: Employee form validation 1.3 Test Execution date: 25-12-22 Test Title: Add employee with null optional input Description: Checking the addition of a new employee without providing the inputs in the optional section of the employee form Precondition (If any): Must be landed on the employee form page during the addition of the new employee and must provide the valid information in the required section. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Enter employee name 6. Enter mobile no 7. Enter joining date 8. Enter employee-type 9. Enter monthly salary 10. Click on submit
Name:Null option check Mob-no: 01824500704 Joining-date:2022-12-15 Employee type: Other Monthly-salary: 1000 Father-name: Null CNIC: Null Education: Null Gender: Null Religion: Null Blood group: Null Experience: Null Email: Null Date of birth: Null Address: Null Employee can able to be registered. As expected, Pass Post Condition: Employee is registered based on the required information and store the information to the database.
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_19 Test Designed date: 22-12-22 Test Priority (Low, Medium, High): Medium Test Executed by: Asif Zaman Module Name: Employee form validation 1.4 Test Execution date: 25-12-22 Test Title: Add employee with invalid optional input Description: Checking the addition of a new employee providing the invalid inputs in the optional section of the employee form Precondition (If any): Must be landed on the employee form page during the addition of the new employee and must provide the valid information in the required section. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Enter employee name 6. Enter mobile no 7. Enter joining date 8. Enter employee-type 9. Enter monthly salary 10. Enter father name 11. Enter education 12. Click on submit
Name: Invalid mail Mob-no:01644412678 Joining-date:2022-12-16 Employee type: Other Monthly-salary: 1000 Father-name: 1234 CNIC: Null Education: 1234 Gender: Null Religion: Null Blood group: Null Experience: Null Email: Null Date of birth: Null Address: Null Employee cannot able to be registered. Not as expected, Fail Post Condition: The invalid data in the textbox must show warning and the user should not be registered as an employee when the submit button is clicked. The information must not store into the database as well.
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_20 Test Designed date: 22-12-22 Test Priority (Low, Medium, High): Medium Test Executed by: Asif Zaman Module Name: Employee form validation 1.5 Test Execution date: 25-12-22 Test Title: Add employee with invalid optional email Description: Checking the addition of a new employee providing the invalid email in the optional section of the employee form. Precondition (If any): Must be landed on the employee form page during the addition of the new employee and must provide the valid information in the required section. Username must be registered to database. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click Add new button 5. Enter employee name 6. Enter mobile no 7. Enter joining date 8. Enter employee-type 9. Enter monthly salary 10. Enter email 11. Click on submit
Name:Invalid mail Mob-no:01644412678 Joining-date:2022-12-16 Employee type: Other Monthly-salary: 1000 Father-name: Null CNIC: Null Education: Null Gender: Null Religion: Null Blood group: Null Experience: Null Email: asif_gmail.com Date of birth: Null Address: Null Employee cannot able to be registered. As expected, Pass Post Condition: The invalid email in the textbox showed warning and the user is not registered as an employee when the submit button is clicked. The information must not store into the database as well.
Project Name: Student Management System Test Designed by: Asif Zaman Test Case ID: FR_21 Test Designed date: 22-12-22 Test Priority (Low, Medium, High): High Test Executed by: Asif Zaman Module Name: Employee edit and delete feature Test Execution date: 25-12-22 Test Title: Employee edit and delete check Description: Checking the deletion of an existing employee and editing the internal data of an employee Precondition (If any): User must be an existing employee and the data must be in the database for the deletion and the edit operation. Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Land to the dashboard section 2. Go to Employees in menu bar 3. Click on All Employees 4. Click the edit button 5. Enter employee name 6. Click on update 7. Enter email address 8. Click on update 9. Click the bin/delete button to delete an existing employee. Name:Rahman Mob-no:Null Joining-date:Null Employee type: Null Monthly-salary: Null Father-name: Null CNIC: Null Education: Null Gender: Null Religion: Null Blood group: Null Experience: Null Email: rahman@gmail.com Date of birth: Null Address: Null Employee data should be updated after edit and deleted after the deletion As expected, Pass Post Condition: The data in the database must be updated after the edit. If the employee is deleted from the all employee section then the data of the employee must be removed.
Test Case ID: EMP_1 Test Designed date:12/22/2022 Test Priority (Low, Medium, High): HIGH Test Executed by: Mehadi Hasan Shojib Module Name: Available ALL Employee Test Execution date: 12/25/2022 Test Title: Searching all available employee by admin account Description: Test eskooly admin searching all employee page Precondition (If any): Admin must have log in by username and password Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1. Go to website 2. Click Employees 3. Click All Employee 4. Search in the search box Search By: Sajid/Prottoy/Asif Zaman / Tamimul
Admin could search all the employees As expected, Pass Post Condition:
Test Case ID: CLC_1 Test Designed date:12/22/2022 Test Priority (Low, Medium, High): High Test Executed by: Mehadi Hasan Shojib Module Name: Class create Test Execution date: 12/25/2022 Test Title: Creating a class by admin account Description: Test the Create classes page Precondition (If any): Admin must have log in by username and password Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1.Go to Website 2.Click Classes 3.Click New class 4. Type class name, tuition fees, Assign class teacher Name of the Class: Class 9/Class 10 Monthly Tuition Fees:1200 Select Class Teacher: Sajid/Asif Zaman Admin can create class As expected Pass Post Condition: Admin successfully added the class and the information saved in database.
Test Case ID: AS_1 Test Designed date:12/22/2022 Test Priority (Low, Medium, High): High Test Executed by: Mehadi Hasan Shojib Module Name: Assign Subject Test Execution date: 12/25/2022 Test Title: Assigning subject by admin account Description: Test the Subject page Precondition (If any): Admin must have log in by username and password and Class must have been created Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1.Go to Website 2.Click Subjects 3.Click Assign Subjects 4. Select Class, Name of the subject and marks. Select Class: Class 9/Class 10 Name of Subject: Physics/Math Marks: 100 Admin submit successfully As expected, Pass Post Condition: Admin successfully added the subject and the information saved in database.
Test Case ID: ADS_1 Test Designed date:12/22/2022 Test Priority (Low, Medium, High): High Test Executed by: Mehadi Hasan Shojib Module Name: Add Student Test Execution date: 12/25/2022 Test Title: Adding student by admin account Description: Test the add student page Precondition (If any): Admin must have log in by username and password and Class and Subject must have been created Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1.Go to Website 2.Click Students 3.Click add new 4.Fill up all the required textbox Name of Student: Any Name. Registration Number: not registered number Select Class: Any available class Admission Date: Admission date Admin added student successfully As expected, Pass Post Condition: Admin successfully added student and the information saved in database.
Test Case ID: CR_1 Test Designed date:12/22/2022 Test Priority (Low, Medium, High): High Test Executed by: Mehadi Hasan Shojib Module Name: Student Test Execution date: 12/25/2022 Test Title: Verifying student registration number. Description: Test two page of one student to check registration number is same Precondition (If any): Admin must have log in by username and password and Student must have been created Test Steps Test Data Expected Results Actual Results Status (Pass/Fail) 1.Go to Website 2.Click Students 3.Click All Students 4.Check registration number of a student 5.Go to that student report page 6. Check registration No 7.Match both pages Registration no Reg No: 12202127 Both pages has to be the same registration number of a student As expected, Pass
8. ITEM PASS/FAIL CRITERIA
• Unit test done in each and every module or feature
• All the modules added one by one and integration test done after every module
integrated
• 100% integration test passed
• No major defects are outstanding
• Not more than 15 minor defects are outstanding
• Code coverage tools indicates all code covered
• Ensuring all critical Test Cases are passed
• Identifying and fixing all the high-priority defects
9. TESTING SCHEDULE
The project schedule includes time for the upcoming testing activities. The precise hours and dates for each task are listed in the project plan timetable. The project schedule and strategy also detail the personnel requirements for each step. The project manager will coordinate the personnel required for each task, the test team, the development team, management, and the client in collaboration with the leaders of the development and test team
GANT CHART (dec20-25)
