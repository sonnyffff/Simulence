# Simulence/Team 34

## Description 
 Simulence is a website focused on providing the tools necessary for small to mid scale indie game development companies to playtest their own games without having to enlist an outside company. The website will match willing playtesters with games similar to their own games, let developers record audio and video, and store data on the specific tests they conduct within the platform. 

Our product is unique in the market due to the fact that the necessary functions of a good playtesting environment do not come at an affordable price for our client base. Simulence tries to change this by offering a playtesting environment where any games from any companies can be professionally tested at a reasonable price. Solo developers will no longer have to manually search for target testers. Indie game companies can easily see and hear their testers’ feedback. 


## Key Features
 **Common Features**
  - Sign up and log in
    - Authentication is now properly handled with Firebase
    - Sign up
      - Choose a user type. This cannot be changed later
      - Remember the email and password to log in
    - Log in
      - Use the email and password to log in 
  - Navigation Bar 
    - Once logged in, the user can see the navigation bar 
    - All the buttons on the navigation bar route the user to the correct page
    - Common Buttons
      - Log out
        - Log out is properly handled with Firebase
        - Once logged out, the user is routed back to the login page
      - Account
        - The button displays the user type 
        - On the account page the user can see their profile and contact info
    - Different user types have different navigation bar buttons
  - Logo
    - Clicking the logo will route you to the dashboard page if you are logged in
    - Clicking the logo will route you to the login page if you are logged out
    
    
**Features for Game Testers** 
  - Navigation Bar
    - Dashboard: The dashboard page shows projects assigned to the tester
    - Survey: The survey page shows the surveys assigned to the tester
    - Calendar: The calendar page shows daily project schedules
 
 
**Features for Game Developers**
  - Navigation Bar
    - Dashboard
      - The dashboard page shows projects created by the developer
      - Developers can add a new game project with the  + Add New Project button
      - Developers can view their game project with the View Details button on each project card      
      - Developers can remove their game project with the Remove button on each project card
    - Survey: The survey page shows the surveys made by the developer
    - Calendar: The calendar page shows daily project schedules


**Features for Admin** 
  - Navigation Bar
    - Templates: The templates page shows all templates in the database
    - Users: The user page shows all users in the database
    - Surveys: The survey page shows all surveys in the database


## Instructions
To access our product, you can use our URL (https://simulence-e7915.web.app/#/). You can register as a new user or log in using the following accounts

| Type of User | Email | Password | 
| --- | --- | --- |
| Developer | super@uoft.ca    | 123123 |
| Tester | dog@bahen.ca  | 123123 |
| Admin | adminsimulence@gmail.com | 123123 |

 
 ## Development requirements
 Requires windows (MacOS/Linux may work, but are not supported)
1. The code is here https://github.com/joshuaanastasakis/Simulence2.0
2. Clone the repo locally
3. Open VS Code on the project
4. Open terminal in Simulence2.0-main directory and type in the following two commands

```powershell
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev
```

5. Go to localhost at this URL: http://localhost:8080/ 

 
 ## Deployment and Github Workflow

 We have two teams working on this product together. Therefore, our github is structured in a way where we have a main branch, which includes the currently working product, and two QA branches for each team named qa-23 and qa-34.

Individuals trying to work on extending features create their own branch from their team‘s QA branch, with the naming convention of whatever the feature they are currently working on. For example, when we wanted to port over the product from V1 of last year, we used porting-insertstudentname. The individuals then test locally on their own machine, if they are able to, the extended features that they wrote code for. 

After local testing, individuals create pull-requests to their team’s QA branch, which are reviewed by Ramzi for our team, and when approved, can be merged. Our team then tests the newly combined code in the qa-34 branch and merges to the main QA branch for both teams after going through a similar pull request process. The final staging and build, as well as manual testing, occurs in the big qa branch. After approval of both teams, the branch is then merged into the main branch as a new release. 

We chose this workflow because we needed to manage the code from each team separately. Therefore we created two QA branches to test the features that each team is implementing separately, and have a big QA branch where we put the code together and stage for a new release.


 ## Licenses 

 We are using the MIT license, which most importantly absolves us of any liability arising from any misuse/connection to our software, and it also allows us to freely distribute our software as we wish. This allows us to showcase any tricks we’ve learned over the years since we can use this project on our resume when applying for jobs. Ultimately we made this choice because we all understand that as students it's important for us to get our work out there, and since we’re not developing anything new or revolutionary, there’s not much of an advantage of hiding the source code behind obscenely strict copyright rules.
