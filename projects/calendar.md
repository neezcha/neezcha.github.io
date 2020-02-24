---
layout: project
type: project
image: images/months.jpg
title: Calandaring Interface 
permalink: projects/calendar 
# All dates must be YYYY-MM-DD format!
date: 2019-08-08
labels:
  - Python
  - JupyterNotebook
  - Calendar 
  - Calendaring System
  - RFC 5545 
summary: Python app designed to generate.ics calendar files that conform to RFC standards. Content is based on user input. 
---

ICS 414 Software Engineering 2 is a project-based class. The goal is to collaborate on something that would require external interaction. Over the course of a semester, my partner and I created the interface for a calendaring system. Conforming to [RFC 5545](https://tools.ietf.org/html/rfc5545) standards we built up the features and error checking to create valid .ics files that will be readable by other applications. 

<img class="ui large left floated rounded image" src="../images/UI.png"> This calendaring system is programmed in Python using Jupyter Notebooks and the `tkinter` library to create the vintage look. To the left is an empty version of our user interface. Final versions of this project offered reoccurrence options and auto-filled the time and date selection based on the user’s computer’s information. The program also checked for valid entries, such as the save file name including a .ics modifier and validating times. For example, ff an events end-time was before the start-time an informative error explaining what is wrong would appear at the bottom of the window. 


[View Project Github](https://github.com/ics414-teamorzo/TeamOrzo)
