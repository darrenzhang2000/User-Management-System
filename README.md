# User-Management-System
Note: since this code is proprietary, I'm cannot to disclose the source code. 

However, I am happy to share the experience I've had while building this project as well as images of the completed product.
## Images of the User Management System can found at [UMS.js](https://github.com/darrenzhang2000/User-Management-System/blob/master/UMS.pdf). 

### Stack
I used React, Redux and Material UI for the user interface and .Net Core and C# for the microservice.

### Motivation
Because New York City Department of Transportation is a huge company with many teams and employees, managing the permissions of each employee can be a daunting task, especially if you have to manually create SQL queries to add/remove a user to/from a user group, give him permission to certain API endpoints, keep track of all function groups a user group has as well as each function and each route in a function group. This user management system streamlines this process in addition to giving user managers access to a specific user / user group's details as well as filter users and user groups based on user/user group id, loginId, name, department, last login, status, and source system. The current User Management System manages 147 users and 25 user groups for the PRISM  team.

### Project Planning
After receiving the user stories, I had to come up with a design for the UI. I took out my notespad, and sketched several prototypes and laying out each component before confirming with my mentor and choosing a design. Since I knew that I would be working with React for the frontend it easy for me to visualize the general code structure. Of course, this is after understanding DOT's coding conventions and structures and comforming to these styles.

As for the backend, I learned about the MVC and MVVM design patterns, and the trade offs between the two. I understood the reasoning behind why DOT choose to follow MVVM, which I followed for the UMS microservice. 

### Features
User features include the following:  User Filter, User Search, and User Details (includes a user's Info, Functions, Function Groups, Features, and Last Logins). 
User Group features including the following:  User Group Filter, User Group Search, and User Group Details (Users and Function Group Cards). Each Function Group Card has a source description, status, and a list of functions and a list of routes belonging to that function group.
Login, logout and user session expiry. 

### Thoughts
I really enjoy creating the project from scratch and seeing how the workflow between the user management frontend and microservice backend. Scaffolding the database models, creating complex sql / link joins, and writing the controllers using a technology and language I haven't used before (.Net Core and C#) to create a whole project in a month and a half is an extremely gratifying feeling. 

As for the frontend, while I've used React before, I never used React hooks. This project showed me the benefits of React hooks (including more modular code and reduced syntax). I also became much more familiarized with organizing code and using Redux and thunks. 

### Reusability
Following the software engineering principle of code reuse, I integrated the already existing Authenication microservice for user login and login session expiry. I also reused the custom sort function, which sorts a table depending on the table headers, ascending or descending, the page number, and the number of rows per page.



