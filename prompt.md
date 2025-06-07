# QuickShelf - PROMPT


Goal: QuickShelf is a Java Spring Boot RESTful API server allowing users to perform CRUD (Create, Read, Update, Delete) operations on product entries.  Each product will have the following attributes:
* id (string, auto-generated unique identifier)
* name (string)
* description (string)
* price (float, non-negative)
* category (string)
* stock_quantity (integer, non-negative)

Endpoints will include:
* POST /products - Create a new product.
* GET /products - Retrieve a list of all products.
* GET /products/{product_id} - Retrieve a specific product by its ID.
* PUT /products/{product_id} - Update an existing product.
* DELETE /products/{product_id} - Delete a product.

Important Technical Considerations!
1. Must offer local run configuration so that app/server can be tested running locally!
2. Must be written in Java 23
3. Must use Gradle as the build management tool
4. Must use Spring Boot (latest version)

We will split this project in 5 main phases - Planning, Implementation, Validation, Documentation, Release

Now, let’s start with the first phase 
Phase I: Planning

1. This project should be tracked and managed in JIRA. In order to integrate via its API, use the jira.properties file jira.py script available in the jira/ folder.
2. As first step, document separate an Epic and respective Stories for code design & implementation in markdown files under jira/docs/ folder. 
       2.1 Each Epic/Story must contain sufficient description (gherkin language) as well as Acceptance Criteria for development.       
3. These epic/stories should be created under my JIRA project. API URL as well as the API Token can be found in jira/jira.properties file - make sure all JIRA tickets (epic/stories) are created successfully.
4. After all tickets (epic/stories) created in JIRA, return a summary of all tasks completion including a summary of tickets (ID and Title) for each.

——

Excellent! Now, let's proceed to next phase

**Phase II**: Implementation

Create a .gitignore file and include IntelliJ, build, and jira/ folders to be ignored by git 
Now, for each JIRA ticket created during Planning:
1. Set its status to In Progress
2. Implement the code changes to complete the task
3. Write tests to validate the changes
4. Once code implementation and tests are done, set ticket to In Review (or similar review status)
5. Commit and push changes to the repository

——

Excellent! Now, let's proceed to next phase

**Phase III**: Validation

1. Create local configuration is available to run the app/server in localhost via simple shell script - example: start.sh script at the root of repository
2. Create/Adjust integration tests to run against locally running app/server (localhost)
3. Make sure all unit and integration tests are passed successfully
4. For each JIRA ticket implemented, add comment to the ticket about tests used to validate its implementation and set JIRA ticket status to DONE


——

Excellent! Now, let's proceed to next phase

**Phase IV**: Documentation 

1. Add Java docs documentation to code base classes and methods
2. Create README.md documentation for users on app/server as well as how to run server locally

——

Excellent! Now, let's proceed to next phase

**Phase V**: Release
1. Make sure all changes are pushed to the repository
2. Adjust README.md to have a professional project repository (include badges and catchy elements) 
3. Make sure project is building and packaged properly
4. Create a tag for release
5. Create release notes (docs) 
6. Push the first release












