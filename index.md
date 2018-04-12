# Table of contents

* [Goals](#goals)
* [About](#about-wash-n-dash)
* [Installation](#installation-instructions)
* [Application design](#application-design)
  * [Directory structure](#directory-structure)
* [Development history](#development-history)
  * [Milestone 1: Mockup and Data Model Development](#milestone-1-mockup-and-data-model-development)
  * [Milestone 2: Administration](#milestone-2-administration)
  * [Milestone 3: Raspberry Pi](#milestone-3-raspberry-pi-appliance-monitor)
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

Landing Page
![](docs/mockLanding.png)

Login Page
![](docs/mockLogin.png)

Signup Page
![](docs/mockSignup.png)

Washing Usage Page
![](docs/mockWashers.PNG)

Dryer Usage Page
![](docs/mockDryers.PNG)

Admin Page
![](docs/mockAdmin.PNG)


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
The top-level directory structure contains:

```
app/        # holds the Meteor application sources
config/     # holds configuration files, such as settings.development.json
.gitignore  # don't commit IntelliJ project files, node_modules, and settings.production.json
```

This structure separates configuration files (such as the settings files) in the config/ directory from the actual Meteor application in the app/ directory.

The app/ directory has this top-level structure:

```
client/
  style.css     
  main.html      
  main.js        # import all the client-side html and js files. 

imports/
  api/           
    machine/
  startup/       # Define code to run when system starts up (client-only, server-only)
    both/
    client/        
    server/        
  ui/
    components/  # templates that appear inside a page template.
    layouts/     # Layouts contain common elements to all pages (i.e. menubar and footer)
    pages/       # Pages are navigated to by FlowRouter routes.

node_modules/    # managed by Meteor

private/
  database/      # holds the JSON file used to initialize the database on startup.

public/          
  images/        # holds static images for landing page and predefined sample users.
  
server/
   main.js       # import all the server-side js files.
```


# Development History

### Milestone 1: Mockup and Data Model Development
This milestone started on 4/2/18 and ended on 4/12/18

The goals of Milestone 1 included the following: 
* Create a set of HTML pages providing a mockup of the pages in the system
* Implement the data model which is the underlying set of Mongo Collections and the operations upon them that would support our application

Milestone 1 consisted of 8 issues (assigned to at least 2 per developer), and progress was managed via the [Wash-N-Dash GitHub Project M1](https://github.com/wash-n-dash/wash-n-dash/projects/1)

[View the deployed app here](http://washndash.meteorapp.com/#/)

The following pages were implemented during M1:

Landing Page
[<img width="400px" src="docs/Landing-New.png">](http://washndash.meteorapp.com/#/)
Signin Page
[<img width="400px" src="docs/Sign-In-1.png">](http://washndash.meteorapp.com/#/signin)
Signup Page
[<img width="400px" src="docs/Sign-Up-1.png">](http://washndash.meteorapp.com/#/signup)
Washer Usage Page
[<img width="400px" src="docs/Washer-Page-1.png">](http://washndash.meteorapp.com/#/washers)
Dryer Usage Page
[<img width="400px" src="docs/Dryer-Page-1.png">](http://washndash.meteorapp.com/#/dryers)


### Milestone 2: Administration
This milestone started on 4/12/18 and ends on 4/24/18

The goals of Milestone 2 include the following:
* Edit washer/dryer pages to be interactive
* Connect the user interface to the underlying data model
* Create an administrator role in the system to override non-admin users' actions

Milestone 2 consisted of 8 issues (2 per developer), and progress was managed via the [Wash-N-Dash GitHub Project M2](https://github.com/wash-n-dash/wash-n-dash/projects/2)


### Milestone 3: Raspberry Pi Appliance Monitor
This milestone started on 4/24/18 and ends on 5/4/18

The goals of Milestone 3 include the following:
* Set up authentication using the University of Hawaii test CAS system
* Applying a raspberry pi appliance monitor (using an accelerometer) in order to more accurately reflect the usage of the washing machines/dryers in the laundry room(s)

Milestone 3 consisted of 8 issues (2 per developer), and progress was managed via the [Wash-N-Dash GitHub Project M3](https://github.com/wash-n-dash/wash-n-dash/projects/3)


# Contact Us
* Riley Cammack (CENG): rcammack@hawaii.edu
  * loves ice cream and playing catan
* Justin Pham (CS): jpham79@hawaii.edu
  * Student by day, gamer by night
* Olivia Murray (CS): omurray4@hawaii.edu
  * 
* David Badke (CS): @hawaii.edu
  * 
