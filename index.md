# Table of contents

* [Goals](#goals)
* [About](#about-wash-n-dash)
* [Installation](#installation-instructions)
* [Application design](#application-design)
* [Development history](#development-history)
  * [Milestone 1: Mockup and Data Model Development](#milestone-1:-mockup-and-data-model-development)
  * [Milestone 2: Authentication and Administration](#milestone-2:-authentication-and-administration)
  * [Milestone 3: Raspberry Pi](#milestone-3:-raspberry-pi-appliance-monitor)
* [Contact us](#contact-us)


# Goals
Our goals for this project are the following:
<ol>
  <li>To become more familiar with designing a project using IntelliJ Idea</li>
  <li>To learn how to implement a multi-user system</li>
  <li>To utilize databases (mongoDB) efficiently</li>
</ol>

### What will our system eventually provide?
Our web application will provide a reliable way for UH students to track the status of the washers/dryers in their dorm's laundry room. 


# About Wash-N-Dash
The problem: UH students often waste too much time walking down with a full basket of laundry just to find all the washing machines are in use.  

The solution: A web application that allows students to update the status of washing machines in use. This way, students won’t have to walk down and be disappointed when no washing machines are available. The minimal version of this app requires a student to manually use the app to indicate the status of the washers when they are in the room. In the future the application may utilize a raspberry pi appliance monitor to automatically update the status of each machine’s availability on the website. This status will be displayed in the app with a timestamp, so that students accessing the app from their room can assess the reliability of the information. An admin user will have the additional capability to override the displayed status of the machines including showing if a washing machine/dryer is broken. This application is uniquely designed to reflect the status of UH Manoa laundry room(s).  

### Mockup Pages
*insert images*

Landing Page

Login Page

Signup Page

Admin Page

Washing Maching/Dryers Usage Page for each dorm

User Page showing available laundry rooms


# Installation Instructions
How to download, install, and deploy the system:
1. [install Meteor](https://www.meteor.com/install).

2. [download a copy of Wash-N-Dash](https://github.com/wash-n-dash), or clone it using git.
  
3. cd into the app/ directory and install libraries with:

 ```
 $ meteor npm install
 ```

4. run the system with:

 ```
 $ meteor npm run start
 ```
 
If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000). If you have an account on the UH test CAS server, you can login. 

# Application Design

### Directory Structure
Coming Soon

# Development History

### Milestone 1: Mockup and Data Model Development
This milestone started on 4/2/18 and ends on 4/12/18

The goals of Milestone 1 include the following: 
* Create a set of HTML pages providing a mockup of the pages in the system
* Implement the data model which is the underlying set of Mongo Collections and the operations upon them that would support our application
* Connect the user interface to the underlying data model

Milestone 1 consisted of 8 issues (2 per developer), and progress was managed via the [Wash-N-Dash GitHub Project M1](https://github.com/wash-n-dash)


### Milestone 2: Authentication and Administration
This milestone started on 4/12/18 and ends on 4/24/18

The goals of Milestone 2 include the following:
* Set up authentication using the University of Hawaii test CAS system
* Create an administrator role in the system to override non-admin users' actions

Milestone 2 consisted of 8 issues (2 per developer), and progress was managed via the [Wash-N-Dash GitHub Project M2](https://github.com/wash-n-dash)


### Milestone 3: Raspberry Pi Appliance Monitor
This milestone started on 4/24/18 and ends on 5/4/18

The goals of Milestone 3 include the following:
* Applying a raspberry pi appliance monitor (using an accelerometer) in order to more accurately reflect the usage of the washing machines/dryers in the laundry room(s)

Milestone 3 consisted of 8 issues (2 per developer), and progress was managed via the [Wash-N-Dash GitHub Project M3](https://github.com/wash-n-dash)


# further requirements to be completed by 4/12:

Up-to-date screen shots showing the state of the project. Each screenshot should be documented with a link to the same page running on Galaxy.

A link to the running deployment of your system on Galaxy.

A link to the M1 Project page, showing what issues were completed for this milestone. It is appropriate that by the time of the due date, there are no issues in the BackLog or In Progress for this milestone.

A link to the M2 Project page, showing the issues expected to be addressed during the second Milestone for this project.

Adherence to the GitHub hosting guidelines.


# Contact Us
If you have comments or questions please contact one of the developers of the system:
<ul>
  <li>Riley Cammack (CENG): rcammack@hawaii.edu</li>
  <li>Justin Pham (CS): jpham79@hawaii.edu</li>
  <li>Olivia Murray (CS): omurray4@hawaii.edu</li>
  <li>David Badke (CS): @hawaii.edu</li>
</ul>
