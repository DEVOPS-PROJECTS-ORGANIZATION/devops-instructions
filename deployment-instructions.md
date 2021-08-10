# Deployment Instructions
## Heroku Cloud
### How to set up a free PostgreSQL database on Heroku
In order to create a new database on Heroku, you first need to create an **Heroku app** in your personal dashboard. Then you can attach a **Heroku Postgres** instance to it as a **resource**.
#### Step 1: Log into Heroku
Navigate your browser to https://id.heroku.com/login and log in. If you don't have an account yet, you can sign up via the **Sign Up** button below the login form:
![log_into_heroku](https://github.com/DEVOPS-PROJECTS-ORGANIZATION/devops-instructions/blob/main/images/deployment-instructions/log_into_heroku.png)
#### Step 2: Create a new Heroku app
Once you see your personal app dashboard, you can create a new app. If your dashboard is currently empty, you can click the **Create new app button**. Otherwise click the **New** button in the top-right corner and select **Create new app**:
![create_new_heroku_app1](https://github.com/DEVOPS-PROJECTS-ORGANIZATION/devops-instructions/blob/main/images/deployment-instructions/create_new_heroku_app1.png)

If you want, you can also change the **Region** so that the database is hosted closer to where you are located. Once you've provided the **App name**, you can click the **Create app** button.
![create_new_heroku_app2](https://github.com/DEVOPS-PROJECTS-ORGANIZATION/devops-instructions/blob/main/images/deployment-instructions/create_new_heroku_app2.png)
#### Step 3: Add a PostgreSQL database
To attach a **PostgreSQL database** to the Heroku app you just created, you need to navigate to the **Resources** tab in the header of your newly created Heroku app's dahsboard. Then type Heroku Postgres into the **Add-ons** search field. When shown, select the suggested **Heroku Postgres** add-on from the dropdown:
![add_postresql_database1](https://github.com/DEVOPS-PROJECTS-ORGANIZATION/devops-instructions/blob/main/images/deployment-instructions/add_postresql_database1.png)

The next popup asks you to choose a pricing plan for the database. Select the **Hobby Dev - Free plan** and click **Provision**:
![add_postresql_database2](https://github.com/DEVOPS-PROJECTS-ORGANIZATION/devops-instructions/blob/main/images/deployment-instructions/add_postresql_database2.png)
