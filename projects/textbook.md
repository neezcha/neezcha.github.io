---
layout: project
type: project
image: images/textbook_gradient.png
title: Textbook Reader  
permalink: projects/textbook
# All dates must be YYYY-MM-DD format!
date: 2019-12-10
labels:
  - Website 
  - Bootstrap
  - HTML
  - CSS
  - JavaScript  
  - PDF.js
summary: Website designed to load and display a pdf document.
---
For my final project in ICS 415 Intro to Programming for the Web, I designed a [website](http://www2.hawaii.edu/~neezcha/textbook/landing.html) that *loads and displays a pdf file hosted on the user’s computer*. The prompt for this project was to redesign a preexisting website we have found to be poor in user experience and or functionality. I chose to redesign the textbook reader for ICS 469 Cognitive Science textbook, which I was also taking that semester. The site made good use of the screen retail space with a vertical left-aligned menu and the preexisting expectation that reading text off a computer screen will not require a user to drastically scan their eyes from one end to the other but maintain a comfortable center column span. The general layout was decently planned for functionality and catering to the user’s expectations. Preserving these positive qualities, I focused on *improving the website’s shortcomings*; a noncollapsable sub-menu, which would shift the main content to right align on the screen, which throws off the ‘status-quo’ that large bodies of text are left-aligned and or centered. The site also included many icons and a half working features. While many of these features have been improved upon since, while I was in the class and building the website, the extra icons and notifications were all clutter interfering with my reading. 

<img class="ui medium right floated rounded image" src="../images/homeTextbook.png">
A surprising amount of time was spent on the fluidity and design of the side menu. The main menu, far left, would always be visible and submenus would toggle to display while shifting the content of the page over so that the pdf will always be centered. Below is an example of the JavaScript code I used to create the sidebar toggle functionality. 

```js
$(function() {
	$('#close').on('click', function() {
		$('.active').toggleClass('active');
	});
});	


$(function() {
	//link on main sidebar
	$('#indexSidebar).on('click', function() { 
		//vertical-nav index
		if('!#subIndex.active’){ 
			$('.active').toggleClass('active');
			$('#subIndex, #content').toggleClass('active');
		} else {
			$('.active').toggleClass('active');
		}
	});
});
```

The largest milestone during this project was accessing the pdf. There are many tutorials online and the platform`PDF.js` to help with reading a displaying a document, however, the project is hosted on `UHUnix`, a Linux based environment available to UHM students. `UHUnix` has a max space limit for students so storing PDFs on my website would max out the storage which I also needed for other classes at the time. I was unable to load documents from another host website due to `Cross-origin resource sharing (CORS)` policies, so I did not have access to those documents (even if I hosted them to my account).  There is a possible workaround to this issue using a proxy server request, however, based on the intended demographic for this website I found another solution. The original purpose of the website was to be a textbook reader for students who are tired of the clutter and right alignment of the other site. These types of students are often tech-savvy enough to have a downloaded version of these textbooks or know how to acquire one. 

PDFs would be uploaded by the students to read on the website. This solves the hosting space issue and the access issue discovered earlier, it would also open up options for students to review other types of PDFs, such as their own essays or online articles, in addition to textbooks. You can see a video demonstration for this website [ICS 415 Final](https://www.youtube.com/watch?v=oRuVnwbr8Ao&feature=youtu.be) or explore the site at [Textbook Reader](http://www2.hawaii.edu/~neezcha/textbook/landing.html). Other asspects of the website were made using Bootstrap.

[View Textbook Reader](http://www2.hawaii.edu/~neezcha/textbook/landing.html)

[View Demo Vido](https://www.youtube.com/watch?v=oRuVnwbr8Ao&feature=youtu.be)


