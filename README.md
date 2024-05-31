# GYM Management System by Team - Software Geeks

Team members:
* Chirudeep Gorle (016682627)
* Dhanasree Rajamani (016715530)
* Sravani Thota (016422406)
* Abdul Vahed Shaik (016452540)

## Schedule for Scrum Meetings:

* Tuesday
* Friday

[Sprint Tasks](https://docs.google.com/spreadsheets/d/1f6_WJecyFG6abPi0M-z7i5wODgQrWlI7Mtdzm5qNGeA/edit?usp=sharing).

[Google Sprint Task Sheet](https://docs.google.com/spreadsheets/d/1OKYuhcoTM6NbxkynXi5L-uJd86wTY79SjqccoMy8iQw/edit?usp=sharing).

<img width="850" alt="image" src="https://github.com/gopinathsjsu/team-project-software-geeks/assets/111466561/58f96d81-08b8-44b3-a16b-fb09100108df">

## XP Core Values

* **Communication** : We collaborated and communicated with one another on weekly zoom sessions to discuss important areas of the project. These meetings helped us understand the feature each team member is working on, plan the task to be performed in the next week, demo implemented features, provide feedback and develop significant components which work well together as one application.
* **Feedback** : Team members frequently provided demo and updates on their work during the meetings(sometimes even outside the scheduled meetings), received comments and valuable feedback on it, and refactored the code to correct issues and make it better for working code. Providing feedback also sparked interesting discussions and decide how and what features to implement such that it adds value to the users of the application.

**How the team kept the core value?**
* Diagrams were drawn during team meetings to show the structure of the tables in the back-end.
* Every Standup includes a summary of the work finished, the challenges faced, and any implementation variations from diagrams.
* Demo the work done in the previous week to make sure all team members are aware of what each team member is working on
* Frequents meetings and demos helped provide feedback on each others work


## Technology Stack

**Front End:**
* Html 
* css 
* Javascript

**Back End:**
* Flask
* Python

**Database:**
MySQL

**Version Control and Collaboration:**
Github

**Application Hosted on:**
AWS

# Contributions:

### Sravani Thota

Implement frontend and backend for the following functionalities:

* Create role-based access - Admin/Members
* Create Navbar with home and logout buttons
* Feature for employees to sign-up new members to gym (Name, Username, Email, startdate, update enddate automatically based on startdate and plan selected).
* Feature for employees to sign-up users for 7-day free-trial.
* Feature for employees to renew expired membership.
* Feature for employees to deactivate a member.
* Handle cases such as member login on membership expiration, email validation, password character length check etc.

### Dhanasree Rajamani

Components Owned : Home page, Gym Information for non members, All Member Functionalities(sign up for class, log hours, member analytics), Host the application on AWS

Implement front-end, back-end and APIs for the following functionalities :
* Create home page with login and gym details(name, address, location, phone)
* Create page for members and non-members to view the gym information(location, membership fee, classes, timings, instructors) and equipments available
* Feature for members to enroll and unenroll themselves in various classes based on location
* Feature for members to view their classes schedule
* Feature for members to log and view the number of minutes they spent on various gym equipments/classes with date, time and location
* Feature for members to view their activities analytics - in the past week, month and 90 days
* Feature for employee to View members of the Gym
* Handle cases such as membership expiration for members enrolled to classes, class capacity when members enroll to a class, etc. 
* Migrate Server side rendering to Client side rendering for member flows(made rest API calls from front end to flask server)
* Host the application AWS

### Vahed Shaik

Components Owned: CheckIn, CheckOut, CheckIn/CheckOut HTML Template, Database operations related to check in/check out.

Implement front-end, back-end, and API's for the following functionalities :
* Create checkin/Checkout page with form that accepts only a vaild member email (email)
* Create a component that allows admins to see who is currently checkin, and enable admins to checkout members accordingly
* Handle cases for when an empty email is provided, when non email format sting is entered, when a non member email is entered
* Created functions to perform CRUD operations on checkin/checkout table to execute logic

### Chirudeep Gorle

Components Owned: Analytics API for Admin, HTML Analytics Dashboard for admin, Database operations related to fetch data to show in admin analytics dashboard.
* Create Analytics page for admin to view analytics dashboard showing User activity
* Create APIs to fetch data from different tables for analytics
* Create chart to show Classes and enrollment by day/week
* Create chart to show Hours spent in the gym by day/week/month
* Create HTML table to show number of visitors by the hour each day, weekday, weekend


# Component Diagram:

![ComponentDiagram jpg (1)](https://github.com/gopinathsjsu/team-project-software-geeks/assets/111466561/5dd646bc-e093-42b4-8094-7e2d4b0f593b)


# **Architecture Diagram:**


![Gym Management Application - 202 Software Systems Engineering](https://github.com/gopinathsjsu/team-project-software-geeks/assets/111466561/358153e1-e351-4ba0-b59a-22858b398229)


## **Class Diagram:**

![Class Diagram](https://github.com/gopinathsjsu/team-project-software-geeks/blob/main/Wellness%20City/app/static/assets/gym_class_diag.jpeg)

## Design Decisions:

* **API Design**: The APIs' input and output formats will be JSON, and they will have error handling and input validation to guarantee the security and integrity of the data.

* **Web UI**: The APIs will be presented utilizing a web user interface that enables members, non-members, and staff members of gym to access various functionalities according to their roles.

* **User Roles**: Members, Non-Members, and Gym Employees (Admins) are the three roles that the system will support. Each role will have unique access privileges and capabilities.

* **Home Page**: The home page will have details about the gym, membership packages, and class schedules. All users will be able to view it.

* **Member Functionality**: Members who are enrolled and logged in will have access to their personal class schedule, activities from the previous week, month, or 90 days, the option to register for classes in advance, and the ability to log hours spent using particular machines or lifting weights.

* **Gym Employee Functionality**: The ability to sign up new members, check members in and out daily, sign up non-members for free trials, and view an analytics dashboard summarizing user activity by location, class enrollment, hours spent in the gym, and the number of visitors by the hour, day, weekday, and weekend will all be available to gym staff.

* **Location Selection**: Users can choose their preferred location on the home page to browse relevant timetables, presuming the gym membership is valid at several locations.

* **Cloud Deployment**: The API will be made available on AWS in an automatically scaling EC2 cluster.
 
* **Database Design**: The sample data for classes, locations, timetables will be kept in a special database that will be built. The database design will guarantee effective data retrieval and storage for the application.

## Feature Set:
* **Users** can view info about address, fees, classes available at different gym locations.
* **Employees** can Add/Remove/Signup_free_trails mebers.
*  **Employees** can check-in/checkout members on daily basis.
*  **Employees** can view analytics about members (classes enrolled, time spent on each equipment, total members etc..).
*  **Members** can enroll to classes of their interest based on classes availability.
*  **Members** can view the classes they have enrolled.
*  **Members** can log and view their hours spent in the gym and equipment used.
*  **Members** can view their activities for week/month/90days/All.

 
