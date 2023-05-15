# Application Dependencies

This document lists the dependencies required to run the application, along with the installation instructions for each dependency.
# Backend Dependencies

    - Node.js 14.17.0: The backend is built using Node.js and requires version 14.17.0 or higher to run. If you don't have Node.js installed, you can download it from the official website.
    - Express 4.17.1: Express is a lightweight web framework used to build the backend of the application. To install Express, run npm install express.
    - pg 8.7.1: pg is a PostgreSQL client for Node.js, used to connect to the database from the backend. To install pg, run npm install pg.

# Frontend Dependencies

    - Node.js 14.17.0: The frontend is built using Node.js and requires version 14.17.0 or higher to run. If you don't have Node.js installed, you can download it from the official website.
    - Ionic 5.5.2: Ionic is a hybrid mobile app development framework used to build the frontend of the application. To install Ionic, run npm install -g @ionic/cli.
    - Angular 12.2.3: Angular is a JavaScript framework used to build the frontend of the application. To install Angular, run npm install -g @angular/cli.

# Database Dependencies

    - PostgreSQL 13.3: The database used by the application is PostgreSQL, version 13.3. If you don't have PostgreSQL installed, you can download it from the official website.

# Installation Instructions

To install all the dependencies required to run the application, follow these steps:

    1. Install Node.js 14.17.0 and PostgreSQL 13.3.
    2. Clone the repository to your local machine: git clone https://github.com/ntn1999/nd0067-c4-deployment-process-project-starter.git.
    3. Change to the project directory: cd nd0067-c4-deployment-process-project-starter/udagram.
    4. Install the Node.js dependencies for the backend: 
        source set_env.sh
        cd udagram-api/
        rm -rf node_modules/
        rm -rf package-lock.json  
        npm install .
        npx tsc
        
    5. Install the Node.js dependencies for the frontend: 
        source set_env.sh
        cd udagram-frontend/ 
        rm -rf node_modules/
        rm -rf package-lock.json 
        npm install -f
        ionic build
        ionic serve
    6. Create the database tables by running the SQL scripts located in the database directory.
    7. Start the backend server: 
        npm run start
        npm run dev.
    8. Start the frontend server: ionic serve.

Once you have installed all the dependencies and started the servers, you should be able to access the application by navigating to http://localhost:8100 in your web browser.