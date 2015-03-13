# Introduction #

Requirements Specification


University Exchange Students Manager

**Introduction:**
This section introduces the requirement specification document for the University Exchange Students Manager application. . It provides the purpose and scope of the system. Any definitions and references are listed in this section as well as an overview of the remaining requirements specification document.

**Purpose:**
This requirement specification document describes the functions and requirements specified for this project. This project is needed to reach a powerful database to finding all of information of students, about the grant and agreements. Every year there are a lot of students invokes to the student exchange program. For this students we want to make a program and also for the officers at the International Office.

**Scope:**
Students who wish to participate in the student exchange program will apply online and officers will check whether it is suitable, to do this, use our program. The officers will access information of students(transcript, student certificate etc.). If the student's application is acceptable officers will make feedback via email on this program and system can keep the history of emails. Including of these messages about the grant, bilateral agreements, language exam date…The same thing will be provided students which are within the program.


-

**User requirements**

•	This system should include full details of students

•	Access students’ information from this system, when they are needed

•	Follow through the system which of the students did not bring the necessary documents or which of the documents did not completed

•	Conditions and details of bilateral agreements can be reached

•	Send emails through the system to the students and supervisors, and system can keep the history of emails.

•	Manage through the system the operations about the grant that will be paid to the student by taking reference of student’s country

•	Letter of visa printed for students using this system

•	Graphical reports can be generated at any time.

•	Just office workers can access this system

•	There must be Access levels for each users

•	Administration must be included so that the highest level
administrator can assign users assuming their Access levels.

•	Erasmus Office can include volatile worker circulation mostly
set up by students.

•	Due to worker circulation, very simple interface must be applied and avoid of any training sequence for every single newbie.

•	All actions must be kept to be followed when needed.

•	System should be backed up in proper time intervals, any breakdowns must be avoided as possible as it can be.

•	Student information should be integrated with BYS or another reliable system used by university.

•	In every step of documentation, there should be full and comprehensive report and documents management.

•	Even if this system is only available in university network, when needed, this system must be accessed out of the university somehow (e.g. an officer’s home)

•	Grant processes and budget should be handled.

•	System must be flexible to be added another features while development or post-development


-

**System requirements**

•	Student information will be accessed from both BYS and provided also by students (Any required authorization and permission must be granted by Unipa, erasmus office should ask and make an agreement between each other, also university managers, dean should be included in this agreement. As soon as this permission granted, student information will be retrieved from BYS)

•	Student information taken from BYS must be cached in Erasmus database, and this information only renewed in every term. Not more frequently to keep the system fast, and avoid data retrieval from BYS for all actions.

•	These Cached student information should be non-clustered indexed in the database (Student ID and Student Name) to speed up search times amongst students.

•	Back-up policy will be decided later by developer team by assuming the current system state.

•	Server should lie on a linux server as it is easy to handle php based e-mail services.

•	Interface should be programmed with php. This is another reason to stick to Linux server.

•	As followed in Libsys of Marmara University, Authorized proxy access should be included to access the interface out of the university.

•	Administration level tree should be like followed here;

**Administrator –** Full access to interface; user handling, authorization; Able to crash report directly to software house, full access all kind of reports

**Moderator –** Full access to interface, Able to crash report directly, almost full access all kind of reports (instructions will be defined later)

**User –**Full access to interface, half access to all kind of reports.

•	There will be a simple integration with the bank account. Only grant budget and transactions will be listed on our system. There will be no interaction by user. This information will be provided by the bank. Information request will be done on a simple background SMS service which is developed by “Ziraat Bankası Ar-Ge” Software Development Team. When user wants to display grant information, our system prepares an sms text at the background which including a monthly use confirmation code, sms service User ID, and action number, and sends this SMS to relevant ZiraatBank database, and this responds our server in same way. Turkcell network service will be preferred. By doing this, we will avoid of any database integration, requests, communication between bank database which is a cheaper way to handle this issue.

•	Programming process should be modular. Customer can add/remove any features during development or post development.

•	.xls files should be imported/exported throughout the system

•	Reports, documents also should be exported as .pdf file, and printed.

•	Reports and documents templates should be personalized by users on a simple text editor interface.

• E-Mails automatically sent to students when confirmed by user in any step. User should preview the e-mail before sending. This preview should be as pop-up page to keep it simple and eye-friendly.

• Student's completed documents should lie on the system with a B-Tree data structure whose root is student's ID. So that listing the missing or completed documents for each student would be easy to handle and faster.


-


**Domain requirements**

•	Only Marmara network can connect to our system as known as Intranet.

•	All kind of requests between bank must be encrypted with 128 bit SSL.

