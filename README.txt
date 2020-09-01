I. Tools used: 

    - npm (node package manager), automatically installed 
    with NodeJs

    - $ npm install: look through all your packages and update
    them

    - $ npm install nodemon --save-dev: automatically update
    the server while running if there is any changes in the code

II. Core Concepts: 
    1. npm & Packages: 
        - Your Local Project usually includes: 
            +, Your Code
            +, Core Node Packages 
            (like 'http' and 'fs' we 
            already used)
            +, Dependecies Packages
            (such as express, etc...)

        - Dependecies Packages: 
            +, Are packages that help us to 
            do things faster with pre-written
            code. 
            +, Stored on npm Repository, which 
            is a cloud Repository

III. Commits Logs: 

    1. Using configuration file: 
        - Files in 2nd Commit

        - $ npm init > release package.json file is a
        configuration file for your project. 

        - Can edit scripts in configuration file. 
        For example, we can type $npm start and 
        project would run the same as command: 
        $ node app.js (1st commit)

        - Note that for any other scripts different than 
        "start", we have to include run. For example: 
        $ npm run start-server > would work
        $ npm start-server > won't work

        (HAVE TO LOOK INTO package.json 
        under "script" to understand)
    
    2. Installing Dependecies packages with npm: 
        - 3rd Commit
        - In NodeJS, whenever there is a change 
        in code, we have to save the code, stop 
        the server and rerun it for it to be updated

        - In this commit, we install this to solve the problem: 
        $ npm install nodemon --save-dev

        - This will produce a package-lock.json, 
        write its version in package.json and 
        create node_modules file