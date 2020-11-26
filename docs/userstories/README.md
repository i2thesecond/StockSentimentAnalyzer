# User Stories

Below are the Stock Sentiment Analyzer's User Stories. Each User Story has an Acceptance criteria, Mis-user stories, and Mitigation Criteria.

Acceptance criteria: defines the set of requirements present when done with the user story.

Mis-user stories: ways which users can mis-use the app. The user, goal, and rationale are malicious.

Mitigation Criteria: For each mis-user story identify at least one mitigation criteria. The mitigation criteria define the set of requirements that tell you when you are done protecting against the mis-user story.

User stories follow the format: 

As a **user/role**, I want to **goal** so I can **rationale**.


## Story 1

User Story: As a **user**, I want to **Add Stock Tickers** so I can **Predict Stock Trends**.

Acceptance criteria: The stock tickers the user adds allows the user to view the stock prediction results. 

Mis-user story: As a **malicious user**, I want to **Remove Other User's Stock Tickers** so I can **prevent other user's from using the application**. 

Mitigation criteria: 

* Role-permissions allow only administrator roles from modifying app data. 
* Django's web application security features prevent web application attacks.

# Story 2

As a **user**, I want to **View Stock Predictions** so I can **make smarter trades**.

Acceptance criteria: Users are able to use the application to help predict stock market trends by viewing the stock market trends based on emotional sentiment. 

Mis-user story: As a **malicious user**, I want to **Modify Other User's Stock Tickers** so I can **prevent other user's from using the application**. 

Mitigation criteria: 

* Role-permissions allow only administrator roles from modifying app data. 
* Django's web application security features prevent web application attacks, such as 

Mis-user story: As a **malicious user**, I want to **Disrupt web services** so I can **prevent other user's from using the application**. 

Mitigation criteria: 

* Server DDoS protection
* Password protect services and implement 2f authentication, such as Twitter Developer credentials. 

## Story 3

As an **administer**, I want to **Add/Edit Users** so I can **Manage access to the application**.

Acceptance criteria: Administrator account can add, edit, and delete users to use the application. 

Mis-user story: As a **malicious user**, I want to **Modify Other User's Stock Tickers** so I can **prevent other user's from using the application**. 

Mitigation criteria: 

* Role-permissi

Mis-user story: As a **malicious user**, I want to **log into the administrator account** so I can **prevent other user's from using the application**. 

Mitigation criteria: 

* Password protects administrator 
* Django's web application security features prevent web application attacks.
