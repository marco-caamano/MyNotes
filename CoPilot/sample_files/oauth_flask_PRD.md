# Project Requirements Document: OauthSample

## Outline
The website will start with a home page that will:
- Provide a Login button if the user is not logged in
- Provide a Welcome Screen with the User's name and other public account information. Also add a logout button

## Technologies used
- Frontend will use HTML, CSS, Javascript and Bootstrap 5
- Backend with use Flask
- Frontend and backend code will be under different folders
- User Authentication will be done with OAuth2 using Github.com

## Requirements

The following table outlines the detailed functional requirements of The OauthSample website.

| Requirement ID | Description | User Story | Expected Behavior/Outcome |
|----------------|-------------|------------|---------------------------|
| TP001 | HomePage | As a user, the initial homepage will provide me with a welcome message and instruct me to click on the login button to login using Github |
| TP002 | Log in to Account | As a user, I want to be able to log into the website by Clicking on the Login Button and authentication with Github using oauth2 | The system will use Github oauth2 to authenticate the user and create a session |
| TP003 | Log Out | As a user, I want to be able to close my connection and log out of the site | The system will provide a log out button that will terminate the user session |
| TP004 | Welcome Screen | As a user when I log in I want to see a welcome screen with my name and other public github account information details |
| TP005 | Already Logged In | As a user, I don't want to be asked to log in again if I already logged in | The system will redirect the user to the welcome screen if he accesses the main page and is already logged in |

