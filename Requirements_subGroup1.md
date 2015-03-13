# User Requirements #
1.   Student records shall be kept at the database

2.  	The contact details of the students should be accessed by interface

3.  	The system should be easy and accessing way to any function should be convenient

4.  	The documents of both incoming and outgoing students should be checked out by the system

5.  	Users shall have password to login system

6.  	Users shall print passport and visa document on system interface.

7.  	The system shall keep all information of applicant students such as name, surname number, department, faculty, e-mail, phone number, GPA, etc.

8.  	The progress of the total grant shall be displayed

9.  	The system shall provide an interface for editing information of student

10.  The agreements between the universities shall be stored with details

11.  Reporting feature should be applied. To form reports, a multi-functional filter is needed to serve reports by needs.

12.  Excel import/export should be added

13.  System keeps the result of student’s Erasmus exam and users shall see student’s Erasmus exam result

14.  The system should provide a password reminder via e-mail to consultant and Erasmus office employee

15.  Users can access to system according to their responsibilities

16.  Backups should be taken manually and periodically

17.  All transactions on the system should be logged with the details of who did the operation and did what

18.  The flow of the grants should be displayed with different perspectives like daily, weekly, monthly etc.

19.  The consistence of the information about grants must be supplied

20.  The system should be managed easily without having a technical knowledge.

21.  There should be a screen to manage the users of the system

22.  Users shall/shan’t access the functions with having their own permissions

23.  Due to the policy of the university, the system should be working in intranet.

24.  System shall recover itself when a system failure occurred.



# System Requirements #


**Membership**


System would consist of administrator, head manager, managers, employees, part time students, and consultant teachers.

All memberships operations would be only controlled by administrator.

Role-based membership shall be applied; permissions are set by administrator for each member group.

Members must only see the screens that they have permission to access, restrictions shall be applied based on groups.



**Student Mobility**


The basic information of students shall be stored at the system.

The documents delivered by the student should be stored and displayed.

Student exam results should be kept in the system.


**Grants**


Total progress of annual grant shall be calculated instantly.

All income and outcome of grants should be displayed.

The system will keep logs of any operation in grants.

Consistency shall be kept by using manual or automatic checks.


**Email**


Emails shall be sent to students, consultants, and university contacts.

Emails should be logged at the system.

Email module shall be capable of receiving and sending mails over current emails by configuration.


**Prints**


The system shall print the student documents with filling the student
data, such as visa application form, passport application form.

The system should provide template based printing mechanism.

**Reports**


The system shall generate reports with the multifunctional filter, and the reports should be displayed as tables.

Reports should be expressed with using graphics tools such as bar chart.

**Integrity**


The system should provide excel import mechanism for bulk data importing such as students, universities, agreements.

All lists should have exporting feature to Excel.

The system should provide RPC calls to give or obtain data from external sources such as getting the transcript data from school management system.


**Universities**


Universities shall be stored with the details of university name, country, city.

Bilateral agreements shall be stored with making connection between the university and the agreed department.

Bilateral agreements should also consist of the numbers of students, start and end date.

Contact details should be kept.

**Backup**


System shall have routine backups and manual backups.

Backups can be downloaded, can be sent to the email, and can be moved to dropbox.

Backups must be encrypted with a password.

Restoration from backup shall be provided.




# Domain Requirements #

1- The system shall be an intranet application.

2- The amount of a student grant would be calculated by daily precision and the unit amount of the grant is country changeable.

3- The unit grants are announced every year.

4- All the payments detail must be kept and be reportable. At the end of the year, reports are sent to the Main International Office with the details.