# Simulence/Team 34

## Product Details
 
#### Q1: What are you planning to build?

We’re planning to build a website focused on providing the tools necessary for small to mid scale indie game development companies to playtest their own games without having to enlist an outside company. The website will match willing playtesters with games similar to their other games, let developers record audio and video, and store data on the specific tests they conduct within the platform. For example, a solo dev that doesn't have the budget to pay a QA company to playtest their game can use our product to playtest it themself, with testers enlisted by Simulence. Similarly, a mid-size game company that wants creative control over their testing process may create their unique workflow within our website.

The website has different entry points for playtesters and developers, leading to separate workflows that connect in the process of testing. For playtesters, this includes filling an informational survey, being matched with a developer and playtesting the game on call or on video. For developers, this includes creating a page for their games, hosting a request for testers and receiving playtesting info such as video and transcripts from them. The website will keep the playtesting data available on its own database for devs to access when needed.


#### Q2: Who are your target users?

The target users of Simulence are indie game developers & playtesters. The game developers need easier access to a database of playtesters to do user research for their game while it is in development, such as collecting player surveys, audio/video recordings of their in game experience, and storing specific data depending on the type of tests they need for their game. The playtesters will be given access to a catalog of games matching their taste, and will have video/audio footage of their test run, whilst also completing surveys created by the developers. Since many smaller game developers do not have the resources to obtain substantial user testing, Simulance will provide quality testing at a much more affordable price. The platform will match developers and playtesters for different games. The service is targeting both small and mid scale indie game developers - not only will it help solo game developers find users to test their game, it will also be a scalable service for larger developers looking for much more data.

Simulance is also targeting video game players and playtesters interested in testing games from indie developers and want to gain more experience in the field, who want to have an impact on the development of games, who are interested in the process of finding bugs and glitches, and would like to support smaller game developers. 

**Target Users:**
* **Solo-devs for games**
    * An independent solo game developer who has limited access to any playtesters. 
* **Smaller game development companies**
    * A smaller game development company looking to expand their testing capabilities, to do user research at a more affordable price.
* **Playtesters**
    * A playtester who wants to gain more experience playtesting games to expand their portfolio.
* **Video game players** 
    * Video game player interested in supporting and contributing to indie games.

#### Q3: Why would your users choose your product? What are they using today to solve their problem/need?

The game development companies currently do not have a general platform which they can use to allow playtesters to playtest their games directly. Simulence offers this platform and streamlines the QA process for the game developers.

Smaller companies now typically go through an outside company to try and playtest their games. Or if they don’t have the budget to hire a QA , they can previously only rely on the people they know. This product will allow these companies or developers to have a scalable playtesting program by remote. The developers will have a large pool of playtesters to work with and with that, a large amount of feedback data which they want from this process. Surveys will be conducted on tests to obtain the opinion-based feedback. Questions regarding how the players felt during some specific part of the games, and game difficulty or mechanics may be included in such surveys to provide more informative feedback.

The program also allows for recordings done on the website, which will be saved into a cloud or database and be accessed by the developers. Testing, otherwise, is tedious for the playtesters and requires outside applications and/or onsite testing. This feature of remote testing saves time and money, which makes the QA process on both ends(developers and playtesters) to be more efficient. Simulence also wishes to make the whole playtesting process as easy as possible for the playtesters. They will fill out surveys or potentially have remote interviews and be matched by the program, or they can search and filter for ongoing playtests, which also saves the playtesters effort and time.

#### Q4: How will you build it?

For the front end we will continue using the framework used by the previous MVP which is Vue. We will also use JavaScript, HTML, and CSS to implement it. For the backend, we may need to handle the HTTP request sent from the user, eg. creating a new user, so the RESTful API may be used. The language we will use is C++, and we will use the docker service. For the database, Firestore and Google Cloud Storage will be used to store the data of recording videos. At last, we will use firebase for hosting.

The previous MVP was deployed on heroku, a container-based cloud Platform as a Service, so we will build on that. 

For the architecture, tester components will publish their services to the admin component . We will create a user component that sends requests to the admin component which handles requests and redirects the user component to the proper tester component.  We may incorporate a broker pattern, which has a broker that is responsible for coordinating communications and transmitting results between the client and servers.

We will test our front end and back end individually. We will create discrete automated testing cases for databases and APIs and manual ones that operate by our members for the front end.

We will also conduct code reviews to identify bugs and that would also help the team members learn about others source code. 


#### Q5: What are the user stories that make up the MVP?

Link to the trello board containing user stories: https://trello.com/b/y7N6joKg/sprint-board
* User stories have dark-green labels named ‘Story’

1. As a game developer I want to browse a list of game testers so that I can find testers for my game.
AC: 
    * Game tester DB exists and stores test user profiles.
    * Developer has a game tester browsing(add testers) tab.


2. As a game developer I want to send invitations to game testers so that I can add them to my project. 
AC:
    * Developer can send an invitation to a game tester.
    * Developer can revoke an invitation.
        
3. As a tester, I want to receive invitations to test games so I can begin the playtesting process.
AC:
    * Tester has an invitation tab.
    * Tester can accept an invitation to  join the project.
    * Tester can decline invitations


4. As a game tester I want to so create/edit my profile so that I can get relevant test invitations. 
AC:
    * Tester has a profile tab. 
    * Tester can edit the profile.
    * Schema for tester profile exist


5. As a game developer I want to watch video recordings recorded by my testers so that I can directly understand the user’s game experience. 
AC:
    * Developer has a playtest list tab. 
    * Developer can select and watch a playtest.
    * Developer can leave comments on the playtest.


6. As a game tester I want to record videos while I’m playtesting so that I can easily share my playtest with the developer. 
AC:
    * Tester has a video recording tab. 
    * Tester can edit the video recording.
    * Tester can leave comments on the video recording.

----
## Intellectual Property Confidentiality Agreement 
> Note this section is **not marked** but must be completed briefly if you have a partner. If you have any questions, please ask on Piazza.
>  
**By default, you own any work that you do as part of your coursework.** However, some partners may want you to keep the project confidential after the course is complete. As part of your first deliverable, you should discuss and agree upon an option with your partner. Examples include:
1. You can share the software and the code freely with anyone with or without a license, regardless of domain, for any use.
2. You can upload the code to GitHub or other similar publicly available domains.
3. You will only share the code under an open-source license with the partner but agree to not distribute it in any way to any other entity or individual. 
4. You will share the code under an open-source license and distribute it as you wish but only the partner can access the system deployed during the course.
5. You will only reference the work you did in your resume, interviews, etc. You agree to not share the code or software in any capacity with anyone unless your partner has agreed to it.

We will be using the MIT license, so we will be using option 2. The MIT license includes:

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. 

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

----

## Process Details

#### Q6: What are the roles & responsibilities on the team?

Describe the different roles on the team and the responsibilities associated with each role. 
 * Roles should reflect the structure of your team and be appropriate for your project. Not necessarily one role to one team member.  
 * Add role(s) to your Team-[Team_Number]-[Team_Name].csv file on the main folder

List each team member and:
 * A description of their role(s) and responsibilities including the components they'll work on and non-software related work
 * 3 technical strengths and weaknesses each (e.g. languages, frameworks, libraries, development methodologies, etc.)

For this project, we split ourselves into roles in which we each feel comfortable in, yet wish to grow in. There are currently 5 roles in our team, frontend, backend, data, scrum master, and product owner. Each role is vital in getting the team going, we have multiple people working on FE, BE, and data since those are the most pressing stacks to work on, while scrum master and product owner are more unique and relate more to team organization than getting work done, and that’s why those two unique roles will also have the students working on other stacks in their spare time. 
The scrum master essentially regulates the tempo of the team and ensures the team follows AGILE methodologies, while also encouraging teammates to give consistent updates about the tasks that need to be done. A product owner controls most of the product decisions and should be the most educated in the way the product should work, while also optimizing the user experience and encouraging proper design decisions. The product owner will be in constant communication with the client to ensure the client’s vision is fulfilled whilst also giving insight into the technical aspect and possibilities of the product. The data role is more focused on setting up the database that will be used throughout the product, and will be focused on setting up Machine Learning models, specifically the tester-developer matching system. The backend developers will be set on rehauling the entire backend of the current project, as there are some security vulnerabilities set by the previous CSC301 team and overall a non-expandable codebase. The frontend developers will salvage the current minimal FE that exists and aesthetically improve the current eye-sore, and overall improve the user flow for various features.

**Ramzi Dajani:** As the scrum master, Ramzi will lead the flow of any meetings going forward and ensure the team is as scrum as possible, this includes setting up a trello scrum board, setting up standup, retrospective, and backlog grooming meetings, and ensuring the meetings stay on topic to minimize the amount of time wasted in meetings, whilst also keeping track of the team’s productivity. Ramzi will also be in charge of setting up the ML classification/recommendation model for matching testers with games that match their taste, i.e. testers that like horror games are more likely to be matched with a horror game than a tester that likes shooter games.

* Strengths:
    * Machine Learning/AI (Various models, familiar with ML kits)
    * SQL (Data manipulation & writing queries)
    * OOO (General, SOLID design)
* Weaknesses:
    * Limited Frontend (Vue & JS unknown, basic knowledge of HTML/CSS)
    * Limited Backend (Hoping to pick up new skills & learn more)
    * CI/CD (Created one jenkins pipeline before, looking to improve in this area)

**Sonny Chen:** As a frontend developer, Sonny will mainly focus on the user interface and webpage design using Javascript, CSS and HTML. And ensure that users can successfully and comfortably interact with the program. Sonny will also manage the software workflow, fix bugs and tests for usability.

* Strengths:
    * Javascript
    * HTML
    * Python
* Weaknesses:
    * Frontend (need to know how exactly Vue and css works)
    * Database handling
    * Software architecture

**Caules Ge:** As a front-end developer, Caules will work on User Interface on websites with JavaScript, HTML, and CSS. In later phases, Caules will connect the front-end to the database.

* Strengths:
    * Front-end development: JavaScript, React, HTML/CSS
    * Back-end: NodeJS, Express 
    * Java, Python
* Weaknesses:
    * Database（limited knowledge on MongoDB）
    * C/C++
    * Software architecture, design paterns

**Ahmad Islah:** As a backend developer, Ahmad will focus on overhauling the security of 
the platform and improving the expandability of the codebase, using C++ and Docker. 
Ahmad will also assist with integrating/managing the database to ensure data is stored 
and accessed easily.

* Strengths:
    * C/C++
    * Python, Java
    * OOP, SOLID, design patterns
* Weaknesses:
    * Database (limited MongoDB experience)
    * Frontend (limited in HTML/CSS/JavaScript)
    * Android/iOS Development

**Gilbert Ye:** As a backend developer, Gilbert will help overhaul the security system of the platform using C++ and docker. This includes the password and accounts and such information’s storage. Gilbert will also integrate the databases and manage such databases of the product to make sure the video/sound data, as well as the data for the playtesters’ profile and feedback data are stored properly and can be accessed easily.

* Strengths:
    * OOP, design patterns
    * SQL
    * C/C++, Python
* Weaknesses: 
    * Frontend(basic knowledge of HTML/CSS only)
    * Web design
    * Mobile development
    * Limited knowledge of software architecture, CI/CD
    
**Ali Gencoglu:** As a frontend developer, Ali will use design principles to develop the UI and maintain connections with the back end and database using the Vue.js framework.

* Strengths:
    * Design patterns
    * Java
    * SQL
    * C/C++
* Weaknesses:
    * Limited knowledge of HTML/CSS and Javascript
    * Limited web design experience
    * Mid-scale software architecture

**Taehwan Park:** As a backend developer, Taehwan will expand his knowledge in SQL to build the database for both test users and developers. Taehwan will also use CI/CD to automatize parts of the development process. As a product owner, Taehwan will write User Stories and attend weekly meetings with the partner. 

* Strengths:
    * SQL
    * C/C++
    * Systems Programming
* Weaknesses:
    * Limited knowledge of CI/CD 
    * Limited knowledge of Frontend
    * Limited knowledge of Firestore and Google Cloud Storage

#### Q7: What operational events will you have as a team?

We will have a meeting on each Thursday with our partner online for 1 hour using Google Meet.
The purpose of each meeting is reporting our working process to the partner. Besides, we may also have weekly sync meetings in our discord voice channel. 

**Summary for the meeting minutes for our September 27, 2022 meeting with the partner:**
* Quick introduction of other teams members(team 23), they previously had a meeting with the partner
* Some overview of the product direction
    * Figma/mock up of the product
    * General direction of work of team 23
    * Information regarding some features the partner want the product to have
* Workflow of the other team working on the same product
    * Discussion of video recordings/remote testing
    * Discussion of database storage and options
**The outcomes of this meeting:** received contact information and started contact with the other team, access to previous code and mockup. 

**Summary for the meeting minutes for our September 29, 2022 meeting with the partner:**
* Company background information
    * Product introduction
    * MVP introduction
* Resource
    * Previous MVP repository
    * Google drive folder with relevant information
    * Airtable to connect team workflows
* Working with the other team in parallel
* In-game play recording
* Playtester database and playtester assignment
* A regular meeting on Thursday afternoon
* Reading through the code of previous MVP
**The outcomes of this meeting:** agreeing upon the license, agreeing to discord and google meet and focus on the playtesters database first and then the interaction part.

**Summary for the meeting minutes for our September 30, 2022 meeting with Team 23:**
* Technology stacks for front end and back end
    * Hosting: Firebase 
    * Frontend: Vue + JavaScript
    * Backend: CPP + Docker 
    * Database: Firestore + Google Cloud Storage
* Future collaboration
* Cross-team organization
    * Created cross-team Trello board to organize
    * Clarified points of intersection between the workload of both teams    
**The outcomes of this meeting:** agreeing upon the technology stack that we will use for frontend backend and database.

Regarding future meetings, we wish to set a consistent agile meeting schedule that follows scrum methodologies. We wish to have recurring standup meetings that are short & sweet, aiming to give small updates to the team about what each member is currently working on. We will also have longer weekly meetings dedicated to sprint retrospective and planning, and backlog grooming. Each of these meetings are aimed less towards what each team member is doing, but rather looking back on our performance and reflecting, whilst also prioritizing and ranking future work. Code reviews and QA will be conducted separately between the reviewer & the coder as they see fit.
  
#### Q8: What artifacts will you use to self-organize?

We use Trello boards across the two teams working on this project to maintain to-do lists and organize our SCRUM framework. We assign team members their tasks by structuring the to-do list on the sprint board, with each column reflecting a different state (i.e. to do, in progress, done, etc…). We prioritize tasks by ordering them by importance on the board during backlog grooming & sprint planning meetings. Our team members will decide among themselves which tickets they’d like to take on by selecting high priority tickets from the backlog and placing them into the “To Do” sprint column with their name assigned to the ticket. Finally, to track progress, the person(s) working on a ticket will update its status on their board as not started, in progress, or done. At the end of each sprint period, we will go over our performance and see how many sprint points are completed during the sprint retrospective.


#### Q9: What are the rules regarding how your team works?

Along with daily standup and weekly meetings from our SCRUM framework, we agreed to meet bi-weekly with our partner to give updates. This would align with our sprint period of two weeks, so that we can present our work from the previous sprint to the partner and inquire more about the partner’s goals/wishes for the next sprint. Key stakeholders will participate in the partner meeting along with the product owner, for example, if the backend was completely overhauled during the sprint, the backend developer responsible for that overhaul is expected to attend. 

In terms of accountability, the daily standup is no big issue, missing 1 or 2 of these meetings per week isn’t much as these standup meetings are only meant to give quick updates, as long as the team member missing standup sends an adequate update regarding their own tickets to the group chat. Failure to provide proper updates will cause a decline in participation points. As for the larger meetings, i.e. grooming & sprint planning, all members are expected to attend these meetings. We aim to be flexible in planning our meeting times, and if a member notifies the team about their unavailability beforehand, then we will try to accommodate said member. With regards to productivity, the scrum master will ensure every developer does an adequate amount of work using story points, if the developer is lacking points & doesn’t make up for it in non-technical projects, then participation points will be deducted.

----
## Highlights

1. **Overhauling the previous team’s backend code**
We reviewed the existing backend code and found three major problems. First of all, sensitive user information was dealt poorly (ex. Unhashed passwords were being passed around the backend as raw strings). Second, the existing code was written by two separate teams including irrelevant directories. Lastly, we realized that most of the database needed repairments. With team 23, we’ve discussed a variety of backend technologies to find the most feasible one for each team’s MVP and the scalability of the project. As a result, we decided to start the backend from scratch instead of making use of the existing code. 

2. **Organizing as two different teams working on a single project**
    We were advised that we should divide work such that one team’s workflow won’t have to rely on the other team's workflow. Therefore, we decided to work on different features of the product (video recording & test user DB) instead of dividing it into developers and testers. Each team will work on both the frontend and the backend of the feature they’ve chosen. At the same time, we could’ve made decisions such as rebuilding the backend as two teams will be working on the same product. 
    
3. **Frontend consistency with other team and previous work on the project**
    Talking along with the other team working on the Simulence project, we agreed to build on the existing frontend done on Vure are significant color clashes (i.e. red text on orange buttons). Therefore, the front end members of both teams need to remain in constant communication throughout the project to ense.js. We also agreed that in many parts the website UI needs overhauls, as for example, theure baseline design uniformity across the project.

4. **Database as the first priority**
    In our meeting with the partner, they mentioned how they’d also like our team to focus on setting up the database. Afterall, the database is used all throughout the project, so it makes sense to make this a top priority. We decided to use Firestore and Google Cloud Storage for our DB as it makes the most sense considering we are using Firebase for hosting. Plus firebase has an excellent ML kit, so the more compatibility the better.

5. **Decision to work on the playtester workflow as second priority**
For our team, we thought that the database was most important, and we believed that the playtester workflow is next on the list of what we should prioritize. The current version of the mockup does not establish this workflow very well, and we wish to finish this part of the application. This will help finish establishing the relationship between the playtesters, developers, and the administrators. We would like to use this workflow to aid in the design of the UI in the frontend as well as providing a structure for how the playtester would behave when using the application. Since this workflow should come before the UI part, we believe that it should be our second priority.
