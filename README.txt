I. Tools used: 

    - npm (node package manager), automatically installed 
    with NodeJs

    - $ npm install: look through all your packages and update
    them

    - $ npm install nodemon --save-dev: automatically update
    the server while running if there is any changes in the code
        NOTE THIS: 
        $ npm install nodemon --save-dev: applied the dependency
        on this project only. So when you run $ nodemon app.js, 
        the terminal won't recognize the command. We can run 
        $ npm start, see package.json under "start" to see why 
        (5th Commit)

        $ npm install -g nodemon: will install the dependency
        globally so you can use it for any projects, and when you run
        $ nodemon app.js, terminal will recognize


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

    2. Types of Errors: 
        - Syntax Errors: 
            +, Shown when compiled
        - Runtime Errors: 
            +, Some code break when it runs
            +, You'll see the message in the terminal 
            if the code run into any issue
        - Logical Errors: 
            + Hard to find since no editor 
              recognize it so you get no 
              error message
            +, You can use the VS code debugging
               tool for these kind of errors
    
    3. Using VS Code Debuggin Tool For NodeJs: 
        - Stop the Server > Debug (On the top bar) 
        > Start Debugging > Debug w NodeJs

        - Put a red dot on any line (2:45 video 50)
        to run the program up until that point. Any 
        code down below won't be executed

        - After run the program, hit View (On the top bar)
        > Debugging > This will show the whole code info
        on VS Code

        - More on it: 
            +, Video 50 - 52, 54
            +, Documentation: 
            https://code.visualstudio.com/docs/nodejs/nodejs-debugging

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

        NOTE: Changed scripts in package.json 
        in 5th commit so we can just run 
        $ npm start 
        nodemon will be automatically applied

IV. Note: 
    - This module contain 2 main contents: 
        +, Understanding npm and 3rd Party packages
        +, Learning the VSCode debugging tool for NodeJS
    
    - VS Code debugging is a skill, need to revised and 
    practice overtime to really get it.

    - Here are some resources for the Debugging Tools: 
        +, Video 50 - 52, 54
        +, Documentation: 
        https://code.visualstudio.com/docs/nodejs/nodejs-debugging
