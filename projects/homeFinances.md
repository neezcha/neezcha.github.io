---
layout: project
type: project
image: images/HF_pie.png
title: Home Finances  
permalink: projects/homeFinances
# All dates must be YYYY-MM-DD format!
date: 2020-08-17
labels:
  - Data Analysis
  - Data Visualization 
  - Python
  - Jupyter Notebooks
  - Bokeh Library 
  - SQL
  - Finances

Summary: I am working on creating informative graphs of my family’s financial situation using the skills I learned from  UH’s Data Analysis class. 

---
While job hunting after graduation I have been working on a personal project to practice my **Data Analysis and SQL skills on my family’s home finances**. Due to the nature of the numbers, I am working with, the numbers and categories are going to block out. From this project, I hope to give my family a better sense of our financial situation and all the good things that can come from that. I plan to create an interactive dashboard, that is clear, intuitive, and informative for my family. To do this I am using SQL to parse the CSV sheet I created in Excel while digitizing my family’s records, along with Python on Jupyter Notebooks using the libraries Pandas and Numpy to interact with the information and the Python library Bokeh to create the interactive dashboard. 

### Data Wrangling
After digitizing my family’s records from their analog origins, I charted some basic graphs to check for any errors or outliers. What I noticed from the bar graph is that one field was significantly larger than the rest. So much so that the other field’s amounts were too small to be seen, this seemed odd considering the average payment amount was small in comparison with other payments. Along with that, the Pie graph confirmed this anomaly and show two others, smaller but still much larger than they should have been.  Using the SQL statement shown bellow I isolated the anomalies. These numbers turned out to be a recording error and was fixed on the CSV sheet. 


<div class="ui medium rounded images">
  <img class="ui image" src="../images/HF_dataWrangling.png">
  <img class="ui image" src="../images/HF_Bar Graph Outlyers Consored.jpg"> 
  <img class="ui image" src="../images/HF_SQL Find Typo Censored.jpg">
  <img class="ui image" src="../images/HF_Pie Chart Glitch Censored.jpg">
  
</div>
 
### Data Visualization

This project is still in progress. 


