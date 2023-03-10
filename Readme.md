# Serene
## Site Description
### Purpose:
Nowadays, around 20% of adults are suffering from mental illness. It affects a person a lot which shows on a person’s act.  This app is a platform which helps a user to track his mental health condition. There are some other purposes of this app which are given below-  
* Serene is a mental health journaling platform that gives users – and other users they authorise – the ability to log and track changes in their emotional state through time.
* Serene was built to solve the problem people face in recounting discrete changes in their mental health and disclosing these changes to those closest to them.
* Most of the time, people don’t want to disclose their mental state to others. But for special purposes such as monitoring (e.g. data can be monitored by the psychologists), users can grant access to other users.
* This app will help to understand a user’s mood so that he/she can manage them and feel better faster. Also, it’s easier to make decisions related to health which can provide a better quality of life.
* It is beneficial for a person to manage low moods and triggering situations if he/she tracks his/her mood daily through this app.
* Serene does this by allowing users to log their mental state each day via journal entries and a weekly wellbeing questionnaire, with select data summarized by a weekly/daily graphical snapshot. Users can grant other users access to this snapshot for remote monitoring. 
* This app plays a great role to reduce the stigma as in most of the communities, mental illness isn’t widely talked about.

### Features/Functionality:   
+ A homepage includes a hero component and a Sign-in/Sign-up button for direct user auth access
+ Profile handler: greeting message, inspirational quote on reload
+ Ability for users to add short journal entries with accompanying ‘emotion’ tags
+ A simple mental wellbeing questionnaire – optionally answered weekly 
+ Ability for users to view a weekly summary, that displays emotions and questionnaire scores from the past week, plus a daily emotions % (pie chart)
+ Ability for users to grant access to their weekly summary to select users


### Target audience:
Although all demographics are welcomed to user Serene, it is initially targeted at therapists/social workers by providing a way to remotely track the mental health of the people under their duty of care.  

### Tech Stack:
1. **Front End Technologies:** React.JS, Bootstrap
2. **Back End Technologies:** Express.JS, Node.JS
3. **Database Technologies:** MongoDB, Mongoose
4. **Testing:** JEST
5. **Deployment:** Railway

## Data Flow Diagram
![data-flow](https://user-images.githubusercontent.com/105357829/213894108-2cb605c3-1e5a-4b00-ac46-0b56619519d6.jpg)

## Application Architecture Diagram 
![image1](https://user-images.githubusercontent.com/105357829/213894470-0634c0aa-f71d-4706-b334-778142d28a85.png)

## User Stories:
+ **Homepage** 
  1. User must be able to register and sign in to their profile
  2. User should be given a summary of what the app does 
+ **Profile**
  1. User should have constant access to navigation via a navbar
  2. User should be able to see their username, welcome message and inspirational quote
+ **Journal [profile component child]**
  1. User should be able to post a journal entry with text, an ‘emotion’ tag and timestamp at any time
  2. User should be able to see a list of previous journal entries
  3. User should be able to delete posts
+ **Calendar [profile component child]**
  1. User should be able to see a summary of the past 30 days, that for each day shows (1) date (2) questionnaire score/colour (3) tags posted 
+ **Questionnaire [profile component child]**
  1. Each sunday a user should have the opportunity to answer a 10 question questionnaire that gives them a score out of 10-50 
  2. User should have this score stored with a timestamp in the db
  3. User should be blocked for completing the questionnaire more than one time per week
+ **Grant Access [within profile/profile component child]**
  1. User should be able to see a list of usernames that have given them access to view their calendar (trackers) 
  2. Users should be able to search and add usernames to a list of people who can view THEIR calendar (populate ‘tracking’ field in db collection)
+ **Settings**
  1. User must be able to delete their account
  
## Trello ScreenShots
[Trello Link](https://trello.com/b/MMurIsLO/mern-frontend-kanban)

![image5](https://user-images.githubusercontent.com/105357829/213894657-884ff87a-1496-4c08-b32b-7352dbbc3a7a.png)
![image2](https://user-images.githubusercontent.com/105357829/213894659-c9436b7e-b687-4498-bf8b-c2b85364f3e4.png)
![image4](https://user-images.githubusercontent.com/105357829/213894681-e5f3aae4-81bf-4e5e-8f90-0f978fc3b3fd.png)
![image3](https://user-images.githubusercontent.com/105357829/213894685-d3e6d9ee-b080-4719-b770-a9735af11007.png)
