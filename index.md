# Table of contents

* [Goals](#goals)
* [About](#about-wash-n-dash)
* [Installation](#installation-instructions)
* [Application design](#application-design)
* [Development history](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)
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

Admin Page

User Page showing available laundry rooms

Washing Maching Usage Page for each dorm


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

### Milestone 1: Mockup development
Use GitHub issues and a GitHub project called “M1” to manage the development of this release of the system.
Use Issue Driven Project Management practices.

Up-to-date screen shots showing the state of the project. Each screenshot should be documented with a link to the same page running on Galaxy.

A link to the running deployment of your system on Galaxy.

A link to the M1 Project page, showing what issues were completed for this milestone. It is appropriate that by the time of the due date, there are no issues in the BackLog or In Progress for this milestone.

A link to the M2 Project page, showing the issues expected to be addressed during the second Milestone for this project.

Adherence to the GitHub hosting guidelines.

Landing Page

Washing Machines/Dryers Page

Clone of Pages for each location

Timers

# Contact Us
If you have comments or questions please contact one of the developers of the system:
<ul>
  <li>Riley Cammack (CENG): rcammack@hawaii.edu</li>
  <li>Justin Pham (CS): jpham79@hawaii.edu</li>
  <li>Olivia Murray (CS): omurray4@hawaii.edu</li>
  <li>David Badke (CS): @hawaii.edu</li>
</ul>
