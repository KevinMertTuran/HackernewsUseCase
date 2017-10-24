#3.usecaseModel

## A fully dressed use case description

## Login

### Login succeed

Actor
Arnold – User (interacts with the subject)
Scenario

1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters username and password and clicks on the “Login” button
4. Arnold is redirected to the front page and has access to authorized functionality
5. Use case ends with Success


### Login - Validation Failed

Arnold – User (interacts with the subject)
Scenario
1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold doesn’t enter either username or password and clicks on the “Login” button
4. Arnold receives an Error Message that says “Please fill out required fields”
5. Use case ends with Failure

###Login – Credential Failed

Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters a username and a wrong password, and clicks on the “Login” button
4. Arnold receives an Error Message that says “Username or Password incorrect, please try again”
5. Use case ends with Failure



##Signup

###Signup – Succeed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters a username and password, and clicks on the “Create Account” button
4. Arnold is redirected to the front page and has access to authorized functionality
5. Use case ends with Success

###Signup – Validation Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters a username but doesn’t enter a password, and clicks on the “Create Account” button
4. Arnold receives an Error Message, that he needs to fill out the required fields.
5. Use case ends with Failure

###Signup – Validation Failed (Password required length)
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters a username and enters a password less than 8 characters, and clicks on the “Create
Account” button
4. Arnold receives an Error Message, that the password must be minimum 8 characters’ long
5. Use case ends with Failure

###Signup – Existing User

Actor
Arnold – User (interacts with the subject)
Scenario

1. Arnold browses through the site and wants to be able to interact with other posts 2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters a username and password, and clicks on the “Create Account” button 4. Arnold receives a Message, that Arnold already has an account
5. Use case ends with Failure

###Signup – Username Taken
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold browses through the site and wants to be able to interact with other posts
2. Arnold clicks on the “Login” button in the navigation bar
3. Arnold enters a username and password, and clicks on the “Create Account” button
4. Arnold receives an Error Message, that the username is already taken
5. Use case ends with Failure


##Comment

###Comment Post - Validation succeed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to comment on a post
2. Arnold navigates to the post and clicks on the “comment” button
3. Arnold enters texts and clicks on the “Add Comment” button
4. Use case ends with Success

###Comment Post – Validation Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to comment on a post
2. Arnold navigates to the post and clicks on the “comment” button
3. Arnold doesn’t enter any text, and clicks on the “Add Comment” button
4. Use case ends with Failure

###Comment Post – Authorization Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to comment on a post
2. Arnold navigates to the post and clicks on the “comment” button
3. Arnold enters text, and clicks on the “Add Comment” button
4. Arnold is not authorized
5. Use case ends with Failure


##Up-vote Comment – Succeed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to up-vote a comment that he likes
2. Arnold navigates to the specific comment and clicks on the “Up-vote” button
3. Arnold is informed that he has up-voted a comment
4. Use case ends with Success

###Up-vote Comment – Authorization Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to up-vote a comment that he likes
2. Arnold navigates to the specific comment and clicks on the “Up-vote” button
3. Arnold is prompted to sign up or login
4. Use case ends with Failure

###Down-vote Comment – Succeed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to down-vote a comment that he dislikes
2. Arnold navigates to the specific comment and clicks on the “Down-vote” button
3. Arnold is informed that he has down-voted a comment
4. Use case ends with Success

###Down-vote Comment – Authorization Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to down-vote a comment that he dislikes
2. Arnold navigates to the specific comment and clicks on the “Down-vote” button
3. Arnold is prompted to sign up or login
4. Use case ends with Failure

##Post

###Create Post – Validation Succeed
Actor
Arnold – User (interacts with the subject)
Scenario
6. Arnold wants to create a post
7. Arnold clicks on the “submit” button on the front page
8. Arnold enters a title, url and text
9. Arnold clicks on the “submit” button to make his post public
10. Use case ends with Success

###Create Post - Validation Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to create a post
2. Arnold clicks on the “submit” button on the front page
3. Arnold does not enter required fields
4. Arnold click on the “submit” button
5. Arnold receive an Error (“Please try again”), required fields cannot be empty
6. Use case ends with Failure

###Create Post - Authentication Failed
Actor
Arnold – User (interacts with the subject)
Scenario
1. Arnold wants to create a post
2. Arnold clicks on the “submit” button on the front page
3. Arnold is prompted to log in or create a new user
4. Use case ends with Failure
