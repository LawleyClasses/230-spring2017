# IGME-230 Web Design &amp; Implementation, Spring 2017: Schedule of Topics

## Contents
- [Week 1 (Jan 24/26): Overview: Syllabus, Expectations, Tools](#week1)
- [Week 2 (Jan 31/Feb 2): HTML & CSS, beyond the basics](#week2)
- [Week 3 (Feb 7/9): Web Design & Accessibility](#week3)
- [Week 4 (Feb 14/16): Online Portfolios & Web Workflow](#week4)
- [Week 5 (Feb 21/23): Responsive Design & CSS Media Queries](#week5)
- [Week 6 (Feb 28/Mar 2): Web Development Frameworks](#week6)
- [Week 7 (Mar 7/9): CSS Animation & Transitions](#week7)
- [Week 8 (Mar 21/23): Javascript Intro: Syntax, DOM, and Debuggers](#week8)
- [Week 9 (Mar 28/30): Javacript Cont'd: Events/Listeners, CSS](#week9)
- [Week 10 (Apr 4/6): JQuery](#week10)
- [Week 11 (Apr 11/13): Client-Side Data Access & Site Security](#week11)
- [Week 12 (Apr 18/20): Web Server Basics & .htaccess Files](#week12)
- [Week 13 (Apr 25/27): LAMP Concepts & WordPress Install](#week13)
- [Week 14 (May 2/4): PHP & MySQL Basics](#week14)
- [Week 15 (May 9/11): WordPress Themes & Final Practical](#week15)
- [Finals Week: Practical Exam Makeup](#finals)

## <a name="week1"></a>Week 1 (Jan 24/26): Overview: Syllabus, Expectations, Tools
I will review the syllabus, goals, and requirements for class. We will discuss the tools and technologies we'll be using for communication, collaboration, and content creation. 

- **Tuesday Readings**
  - [Course Syllabus](README.md)
  - [Slack Guides: Getting Started for New Users](https://get.slack.help/hc/en-us/articles/218080037-Getting-started-for-new-users)

- **[Tuesday Exercise](weekly_materials/week1/tuesdayExercise.md)**
  - In this exercise, you'll sign up for the (free) Github Student Developer Pack,  set up an account on the class Slack, and configure Visual Studio Code for use in class. 

- **Thursday Readings**
  - [Why Validate?](https://validator.w3.org/docs/why.html) from w3.org 
  - [The Basics of Visual Studio Code](https://code.visualstudio.com/docs/editor/codebasics)
  - [HTML Programming in VS Code](https://code.visualstudio.com/docs/languages/html)
  - [Save Time and Keystrokes with Emmet in Visual Studio Code](https://devhammer.net/blog/save-time-and-keystrokes-with-emmet-in-visual-studio-code/)

- **[Thursday Exercise](./weekly_materials/week1/thursdayExercise.md)**
  - We will review the functionality of VS Code in class, working together in class to take a text file and mark it up as valid HTML. We will also add a configuration file to your banjo.rit.edu account to change its default behavior with web pages. 

## <a name="week2"></a>Week 2 (Jan 31/Feb 2): HTML & CSS, beyond the basics
A deeper dive into aspects of HTML and CSS that aren't covered in the prereq classes: validation, semantic markup, CSS positioning, complex CSS selector types, and more.

- **Tuesday Readings**
  - Review the content in [Lynda.com HTML Essential Training, Lessons 1-6](https://www.lynda.com/HTML-tutorials/HTML-Essential-Training/170427-2.html?org=rit.edu). Some of it will be familiar (like basic HTML formatting). Other parts will be new (like structuring content with semantic tags, linking to regions inside a page, and creating complex lists). 

- **[Tuesday Exercise](./weekly_materials/week2/tuesdayExercise.md)**
  - We will revisit the file we worked on last week, adding semantic markup, and internal and external links.
 
- **Thursday Readings**
  - [Lynda.com: CSS Fundamentals, Sections 1-3](https://www.lynda.com/CSS-tutorials/CSS-Fundamentals/417645-2.html?org=rit.edu) (this replaces the CSS Positioning tutorial I had originally assigned; if you have already completed that course, you don't need to do this one)
  - Not required, but useful references: [CSS Selector Reference](http://www.w3schools.com/cssref/css_selectors.asp) and [CSS Box Model](http://www.w3schools.com/css/css_boxmodel.asp)
  
- **[Thursday Exercise](./weekly_materials/week2/thursdayExercise.md)**
  - We will use CSS positioning to modify the layout of an HTML file 

[Project 1](projects/project1.md) (a personal page) is due at the end of this week (11:59pm on Saturday, February 4th)
  
## <a name="week3"></a>Week 3 (Feb 7/9): Web Design & Accessibility
When we talk about "web design," we're actually talking about a much wider range of concepts than graphic design--we're also talking about interaction design, usability, and accessibility. This week we'll talk about the range of design issues related to the web. On Tuesday we'll talk about the intersection of graphic design and interaction design, including Jesse James Garrett's excellent diagram showing the various elements of user experience. In class, I'll have you break into groups to look at and critique a number of websites.

On Thursday we'll talk about accessibility for the web, and I'll have you assess the usability of some pages, and then edit a page to correct accessibility errors. 

- **Tuesday Readings**
  - [Interaction Design Basics](https://www.usability.gov/what-and-why/interaction-design.html)
  - [The Elements of User Experience](http://www.jjg.net/elements/pdf/elements.pdf)

- **Tuesday Lecture Links**
  - [Slides from Tuesday's Lecture](weekly_materials/week3/230-Week3-UX&IA.pdf)
  - Flow Chart Tools
    - [Draw.io](http://draw.io/) - Free, web-based flowcharting tool
    - Google Drawings and Microsoft Word and PowerPoint have flowcharting symbols available
    - Microsoft Visio is available on lab computers
    - Many of the wireframing tools linked below also have flowcharting stencils & tools

  - Wireframing Tools
    - Downloadable paper templates: [Sneakpeekit](http://sneakpeekit.com/), [Smashing Magazine List](https://www.smashingmagazine.com/2010/03/free-printable-sketching-wireframing-and-note-taking-pdf-templates/)
    - [UI Stencils (Analog)](http://www.uistencils.com/collections/stencils) (Amazon has other options)
    - [Yahoo UI Stencil Kit](https://developer.yahoo.com/ypatterns/about/stencils/) - Available in multiple formats
    - [Cacoo](https://cacoo.com/lang/en/tour) - Web-based. Free for ≤6 diagrams, I've requested an edu license for the class
    - [Balsamiq](https://balsamiq.com/) - Desktop for Mac and Windows. Free for 30 days. [License good until 20 May 2017 has been posted in our myCourses shell.](https://mycourses.rit.edu/d2l/le/news/633310/449029/view)

  - Prototyping and Comp Tools
    - [Style Tiles Approach](http://styletil.es/) - Alternative to graphics-heavy comps
    - [Axure](https://www.axure.com/edu) - Available on IGM lab computers, free license for students
    - [Invision](https://www.invisionapp.com/) - Free web-based tool
    - [Design the Web: Layer Comps](https://www.lynda.com/Photoshop-tutorials/Using-Layer-Comps-Show-Interactive-States/114904-2.html?org=rit.edu) - Lynda.com tutorial on using Photoshop for comps
   

- **Thursday Readings**
  - [Web Accessibility Initiative: Diversity of Web Users](https://www.w3.org/WAI/intro/people-use-web/diversity)
  - [Web Content Accessiblity Guidelines (WCAG) At-A-Glance](https://www.w3.org/WAI/WCAG20/glance/Overview)

- **[Thursday Exercise (Accessibility Writeup)](weekly_materials/week3/thursdayExercise.md)**


## <a name="week4"></a>Week 4 (Feb 14/16): Online Portfolios & Web Workflow 
Your second project is a portfolio site about yourself and your work. This week we'll look at a variety of approaches to online portfolios, and talk about content, organization, and design. We'll also begin to talk about workflow for websites, particularly version control and collaborative work, and you'll be introduced to Git and Github for tracking and maintaining your HTML and CSS files.  

- **Tuesday Readings**
  - [Breaking Into Game Design, Part 2: Build Your Portfolio](http://www.gamasutra.com/blogs/EthanLevy/20130621/194830/Breaking_into_game_design_Part_2__build_your_portfolio.php)
  - [Graphic Design Portfolios: The New Online Resume](http://www.howdesign.com/design-career/resume-portfolio/graphic-design-portfolios-new-online-resume-design/)

- **[Tuesday Exercise](weekly_materials/week4/tuesdayExercise.md)**
  - In today's exercise, you'll create an initial design document for your next project, a personal portfolio site. 

- **Thursday Readings**
Do one of the following tutorials *before* class on Thursday. I recommend the first one, but either one is acceptable. Make sure you block off time to do this; while the courses are listed as taking 3-4 hours, it can take longer since you'll frequently need to stop, try something on your computer, and then restart. 
  - [Lynda.com: GitHub for Web Designers, Chapters 1-3](https://www.lynda.com/GitHub-tutorials/GitHub-Web-Designers/162276-2.html?org=rit.edu)
  - [Lynda.com: Version Control for Everyone](https://www.lynda.com/GitHub-tutorials/Version-Control-Everyone/378045-2.html?org=rit.edu)

## <a name="week5"></a>Week 5 (Feb 21/23): Responsive Design & CSS Media Queries
Mobile devices now make up more than half of the traffic to major websites. That means web designers need to make sure their pages work on a variety of screens, not just high-resolution computer monitors. The process of creating HTML and CSS that will adapt to a variety of devices is called responsive design. CSS Media Queries allow responsive design to work more effectively by determining what environment the page will be displayed in. 

- **Tuesday Readings**
On Tuesday we'll look specifically at using CSS to create different versions of a page for different media types. This was covered in the CSS Fundamentals tutorial from week 2, but for review, you should look at the portion of that tutorial dealing with the topic. 
  - [Lynda.com CSS Fundamentals: Media Types & Queries](https://www.lynda.com/CSS-tutorials/Media-types-media-queries/417645/484795-4.html?org=rit.edu)

- **Thursday Readings**
On Thursday we'll dive more deeply into responsive design concepts.
  - [Lynda.com: Responsive Design Fundamentals](https://www.lynda.com/Web-Responsive-Design-tutorials/Responsive-Design-Fundamentals/104969-2.html?org=rit.edu) - Like the "CSS Fundamentals" tutorial from week 2, this is not a hands-on tutorial--instead, it is an overview of what responsive design is, why it's important, and how it's typically implemented. In class, we'll have a hands-on exercise applying these concepts. 
 
## <a name="week6"></a>Week 6 (Feb 28/Mar 2): Web Development Frameworks
Many responsive websites are built using a pre-existing framework of CSS and Javscript that enable the developer to focus on content and design rather than the underlying code necessary for effective responsive functionality. We'll be working with one of the most widely used frameworks, Bootstrap. 

Because I will be in San Francisco for GDC this week, you will work through these tutorials and then implement exercises on your own. 

- **Week 6 Tutorials**
  - [Lynda.com: Bootstrap 3 Fundamentals](https://www.lynda.com/Bootstrap-tutorials/Bootstrap-3-Essential-Training/417641-2.html?org=rit.edu) -- Even though Bootstrap is now up to version 4, this tutorial covers the basics of how Bootstrap works, and how you can use it to create responsive designs. 
  - [Lynda.com: Bootstrap 4: First Look](https://www.lynda.com/Bootstrap-tutorials/Bootstrap-4-First-Look/372547-2.html?org=rit.edu) - This shorter tutorial looks at the differences between Bootstrap 3 and 4.

- **Week 6 Exercise**
  - TBA 

## <a name="week7"></a>Week 7 (Mar 7/9): CSS Animation & Transitions
Modern CSS can control more than just the static presentation of web pages; it can also be used for motion graphics. This week we'll look at CSS animation and transition effects.

- **Tuesday Readings**
  - [Lynda.com CSS:Animation](https://www.lynda.com/CSS-tutorials/CSS-Animation/439683-2.html?org=rit.edu)


## SPRING BREAK
[Project 2](./projects/project2.md) (a personal portfolio site using responsive design) is due at the end of spring break. 

## <a name="week8"></a>Week 8 (Mar 21/23): Javascript Intro: Syntax, DOM, and Debuggers
We'll begin looking at Javascript this week, and its importance in building interactivity into websites. This week will be the basics--syntax, the Document Object Model, and basic debugging using both VS Code and Chrome's developer tools. 

## <a name="week9"></a>Week 9 (Mar 28/30): Javacript Cont'd: Events/Listeners, CSS
This week is a continuation of basic Javascript programming, with a focus on HTML events and event listenters, as well as the interaction between Javascript and CSS.

## <a name="week10"></a>Week 10 (Apr 4/6): JQuery
A great deal of the Javascript on the web uses a freely-available library of code called JQuery (which, in fact, was originally written by an RIT student!). We'll be looking at JQuery and how to use it this week. 

## <a name="week11"></a>Week 11 (Apr 11/13): Client-Side Data Access & Site Security
Most modern websites don't use completely static data--they dynamically generate content from databases or other inputs. This week we'll look at data access on the client (browser) side, and also will talk about the security implications of client-side data access.

Your third project is due at the end of this week.

## <a name="week12"></a>Week 12 (Apr 18/20): Web Server Basics & .htaccess Files 
Understanding the basics of how a web server works can make your work as a designer and/or developer much easier. We'll look at basic web server operation, as well as the use of .htaccess files to modify how the server works with your pages. 

## <a name="week13"></a>Week 13 (Apr 25/27): LAMP Concepts & WordPress Install
The majority of web servers on the Internet use Apache software running on a Linux operating system. Many also use mySQL databases, and the PHP server-side scripting language. The combination of these four technologies is referred to as "LAMP." This week we'll install a copy of WordPress onto a LAMP server, and talk about dynamic database-driven websites. 

## <a name="week14"></a>Week 14 (Apr 2/4): PHP & MySQL Basics
Under the hood, WordPress uses both PHP and MySQL. We'll talk about both technologies this week, and look at how the WordPress database is organized. 

## <a name="week15"></a>Week 15 (Apr 9/11): WordPress Themes & Practical Exam
Once you understand CSS, PHP, and MySQL, it becomes much easier to modify WordPress themes and even create your own. On Tuesday, we'll look at what goes into a WordPress theme. And on Thursday, you'll take the final practical exam for the class. 

## <a name="finals"></a>Finals Week: Practical Exam Makeup
In addition to the makeup practical exam, your group project will be due this week. 
