## Table of contents

* [Deployed Page](http://studiousmanoa.meteorapp.com)
* [Overview](#overview)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Team Members](#team-members)

## Overview 

Studious Manoa is a mockup website that allows students to find study spots in and around the UH Manoa campus. In this website, 
we use will be using the following frameworks and toolsets that we have learned in class:

* [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code. 
* [React](https://reactjs.org/) for component-based UI implementation and routing.
* [Semantic UI React](https://react.semantic-ui.com/) CSS Framework for UI design.
* [Uniforms](https://uniforms.tools/) for React and Semantic UI-based form design and display.

**The Problem**

Students typically limit themselves to only studying consistent locations when there are hundreds of available study spots all over
campus. Sinclair or Hamilton library are the “go-to” study spots, but both can get busy throughout the week and especially during finals
week. There are many spots available to students that are not utilized because students are not aware of it.

**The Solution**

A website that will allow students to post and rate study spots throughout the UH Manoa campus and the surrounding areas so that 
other students become aware of possible study spots. The entry for each location will list hours, capabilities, capacity of the 
location, and accessibility to different types of students. In addition, there is a “real-time” feature, where students can login 
and provide time-stamped notifications about the current state of the study space. This can inform other students about whether 
the space is noisy, or crowded, or even quiet and empty.


## User Guide

This section provides a walkthrough of the Studious Manoa user interface and its capabilities. 

### Landing Page

The landing page is presented to users when they visit the top-level URL to the site. This also shows a map uh UH Manoa implemented 
with the Google Maps API key.

### Sign in and sign up

Click on the "Login" button in the upper right corner of the navbar, then select "Sign in" to go to the following page and login. 
You must have been previously registered with the system to use this option.
 
  
Alternatively, you can select "Sign up" to go to the following page and register as a new user.


## Community Feedback 

We are interested in your experience using Studious Manoa. We will provide a form in the near future that will help us understand 
how to better improve the system.

## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks. 

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, visit the Studious Manoa application github page, and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.  However you do it, download a copy of the repo to your local computer.
  
Third, cd into the studious-manoa/app directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000). 

### Application Design

Studious Manoa is based upon [meteor-application-template-react](https://ics-software-engineering.github.io/meteor-application-template-react/) and [meteor-example-form-react](https://ics-software-engineering.github.io/meteor-example-form-react/). Please use the videos and documentation at those sites to better acquaint yourself with the basic application design and form processing in Studious Manoa.

### Data model

To be implemented soon.

## Initialization

The config directory is intended to hold settings files.  The repository contains one file: [config/settings.development.json](https://github.com/bowfolios/bowfolios/blob/master/config/settings.development.json).

## Quality Assurance

### ESLint

Studious Manoa includes a .eslintrc file to define the coding style adhered to in this application. You can invoke ESLint from the command line as follows:

```
meteor npm run lint
```

ESLint should run without generating any errors.  

It's significantly easier to do development with ESLint integrated directly into your IDE (such as IntelliJ).

### From mockup to production

Studious Manoa is meant to illustrate the use of Meteor for developing an initial proof-of-concept prototype.  For a production application, several additional security-related changes must be implemented:

* Use of email-based password specification for users, and/or use of an alternative authentication mechanism.
* Use of https so that passwords are sent in encrypted format.
* Removal of the insecure package, and the addition of Meteor Methods to replace client-side DB updates. 

(Note that these changes do not need to be implemented for ICS 314, although they are relatively straightforward to accomplish.)

## Development History

The development process for Studious Manoa conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f19/modules/project-management/) practices. In a nutshell:
 
* Development consists of a sequence of Milestones. 
* Each Milestone is specified as a set of tasks.  
* Each task is described using a GitHub Issue, and is assigned to a single developer to complete. 
* Tasks should typically consist of work that can be completed in 2-4 days.  
* The work for each task is accomplished with a git branch named "issue-XX", where XX is replaced by the issue number. 
* When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master. 
* The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.

The following sections document the development history of Studious Manoa.

### Milestone 1: Mockup development

The goal of [Milestone 1](https://github.com/studious-manoa/studious-manoa/projects/1) is to create a set of HTML pages providing a mockup of the pages in the system. 


### Milestone 2: Data model development 

The goal of [Milestone 2](https://github.com/studious-manoa/studious-manoa/projects/2) is to implement the data model: the underlying set of Mongo Collections and the operations upon them that would support the BowFolio application.

### Milestone 3: Final touches

The goal of Milestone 3 is to clean up the code base and fix minor UI issues.

## Team Members

Listed below are the professional portfolios of the Sudious-Manoa team:

* [Jianna Orias](https://jlorias.github.io/)
* [Rebecca Vatnebryn](https://rebeccavatnebryn.github.io/)
* [Sahra Moseby](https://sahramoseby.github.io/)
* [Nathaniel Tomchak](https://ntomchak.github.io/)
* [Eric Botello](https://erbot.github.io/)


