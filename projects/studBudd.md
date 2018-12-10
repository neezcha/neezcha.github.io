---
layout: project
type: project
image: images/StudBudd3-transperent-book.png
title:  StudBudd
permalink: projects/MWE
# All dates must be YYYY-MM-DD format!
date: 2018-12-09
labels:
  - Meteor
  - Semantic UI
  - Software Engineering
  - React
  - Project Management 
  - Web Development
  - Website  
summary: A website developed for UH students to connect with fellow students who are proficient in a subject field and peers studying similar topics. 

---

[StudBudd](https://studbudd.github.io/)is a website developed for ICS 314 Software Engineering, using  Meteor, React and Semantic UI. For our final project we were grouped into teams of three or four to work on building a functioning website that can benefit the local student community. StudBudd’s goal is to help students connect with fellow students who are proficient in a subject field and peers studying similar topics.

The final project was partitioned into three milestones.  **Milestone one** was focused on a functional aesthetic landing page that users would first be created with, along with a few non functional mockup pages. I was incharge of the navigation bar at the top,  and the mockup pages - some with restricted access depending on the role the user is signed in as. 

**Milestone two** only really specified the need for increased functionality, so we constructed collections and focused on being able to add to those collections. For this milestone I filled out the mockup pages, such as Class List, Instructions, and the now deleted Mentors page that was mainly a tester to show that the collections worked. 

For **milestone three** we shifted gears, working on pulling from our working collections, and designing an intuitive usable website. This milestone I implemented a working Class List page using a nested underscore function to pull from our collection, cleaned up the landing page, and worked on a various of bug issues.

Bellow is some **example code** of the nested underscore fucntion I used to *_.filter* out mentors who have the specified *subject* in their *class* feild and then *_. map* those mentors using their card component, *MentorCard*, onto the page.  

```js
{this.props.mentors.filter(
                  mentor => (this.state.subject && (this.state.subject.includes((mentor.class)))),
              ).map(
                  (mentor, index) => <MentorCard key={index} mentor={mentor} />,
              )}
```

This was one of the largest projects I have worked on from the ground up and I have learned a lot about project management and features I can use on github. At first creating Issues was difficult for our group, we would assign easy task as a whole issue and large task with multiple parts as another issue, but by milestone two I had a much better sense of how to break up large tasks into reasonable sizes. That way everyone can regularly to check off progress for updates and moral boost. 
<div class="ui small rounded images">
<img src="https://raw.githubusercontent.com/studbudd/studbudd.github.io/master/doc/StudBudd3-transperent.png">
</div>
<div class="ui medium rounded images">
  <img class="ui image" src="../images/MS3-LP.png">
  <img class="ui image" src="https://raw.githubusercontent.com/studbudd/studbudd.github.io/master/doc/MS3-SIGNUP.png">
  <img class="ui image" src="https://raw.githubusercontent.com/studbudd/studbudd.github.io/master/doc/MS3-CLASS.png">
  <img class="ui image" src="../images/MS3-INSTRUCTIONS (2).png">
</div>
