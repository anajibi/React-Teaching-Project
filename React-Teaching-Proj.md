# <h1 style="text-align: center;">The Course Adder Project <br/>System Group</p>

In this project we want you to learn React by building a simple web application.
In the first phase you will only build the frontend part of the application with a
mocked backend. In the second phase you will build the backend and connect it to the frontend.

As the purpose of this project is to make you ready for the next phase which is to
use React to develop azure devops extensions, you should use the respective packages and the UI system of
Azure Devops as much as possible in your application. You can find samples of different
components of the specified library in the [Formula Design](https://developer.microsoft.com/en-us/azure-devops/)
website.
Steps and guidelines for using the UI system of Azure Devops can be found in this website.

#### Note: Don't forget to ask questions regarding different parts of the project and the technologies used in it.

#### Note: You should use Typescript for both front-end and back-end parts of the project.

#### Note: The responsibility of designing the UI and the back-end models for this project is on you.


## Phase 1

In this phase you will build the frontend part of the application. In most cases, building a React application
involves creating a global state using [Redux](https://redux.js.org/) which helps us handle the data flow in
the application. In this project since we are going to have only one page, there is no need to use redux in the first
phase.

### Overview

This project is a similar version of [Sharif's course selection system](https://my.edu.sharif.edu). You are required to
implement the add course page to this system. In this page, students can add courses to their schedule.

### Requirements

- The page should have a header and a footer. The header should contain the name of the system and the name of the
  student.
- The page should have a sidebar which contains the list of courses that the student has added to his/her schedule.
- The page should have a main section which contains the list of all the courses that the student can add to his/her
  schedule.
- Each course in the main section should have a button which adds the course to the student's schedule.
- Each course in the sidebar should have a button which removes the course from the student's schedule.

### Mocked Backend

In this phase you should use a mocked backend. You can use
[json-server](https://github.com/typicode/json-server) which is an NPM package that helps you create a mocked backend
using a json file. You can find 3 json files which are the mocked data for three departments of Sharif University (CE,
MATH, PHYS)
in the `mocked-backend` folder. You can use these files to create your mocked backend.

### UI System

You should use the UI system of Azure Devops as much as possible in your application. You can find samples of different
components of the specified library in the [Formula Design](https://developer.microsoft.com/en-us/azure-devops/)
website.
You can also find samples of using such components in
the [GitHub repository](https://github.com/microsoft/azure-devops-extension-sample)
of the Azure Devops extension sample.

### Non-Functional Requirements

- You should use Webpack to bundle and host your application.
- You should use scss to style your application.
- You should use eslint to lint your code.
- You should use prettier to format your code.
- You should use webpack-dev-server to host your application.
- You should use typescript for your application.

## Phase 2

In this phase you will build the backend part of the application. You should use [Express](https://expressjs.com/)
to build your backend. For the database part, you should use [Knex](https://knexjs.org/) which is a query builder for
SQL databases, thus, there is no need to write raw SQL queries in your code. The database engine that
you should use is of your choice. You can use [PostgreSQL](https://www.postgresql.org/) or
[SQLServer](https://www.microsoft.com/en-us/sql-server/sql-server-2019) or any other SQL database engine; however,
my suggestion is to use SQLServer as it is the database engine that is used in Azure Devops.

### Overview

In this phase you have to implement some APIs to connect your front-end application to a back-end
server. The mocked backend will be replaced by the real backend in this phase. In this part,
you are required to implement an authentication system for the students to be able to distinguish
between different students.

### Requirements

You should implement the following APIs:

- Adding and removing courses from the student's schedule.
- Getting the list of courses that the student can add to his/her schedule.
- Getting the list of courses that the student has added to his/her schedule.
- Getting the list of all the courses.
- Getting the list of all the departments.
- Getting the list of all the courses of a specific department.
- Users should have an id which is unique for each user and generated by the server as `uuid`.

### Authentication

There is no need to implement a real authentication system. We only need users to be able to log into the system,
in fact, you can even ignore user passwords and log them in using only the username.

### Non-Functional Requirements

- You should use eslint to lint your code.
- You should use prettier to format your code.
- You should use typescript for your application.
- You should use knex to connect to your database.
- You should use express to build your backend.

#### Note: I suggest creating the back-end project using [express-generator-typescript](https://github.com/seanpmaxwell/express-generator-typescript).

## Phase 3

In this phase, you will integrate your front-end application with the azure devops and change it to an azure devops
extension.
To get yourself more familiar with the azure devops extension development, you can read
the [documentation](https://docs.microsoft.com/en-us/azure/devops/extend/overview?view=azure-devops)
and the [samples](https://github.com/microsoft/azure-devops-extension-sample) provided by Microsoft.

### Requirements

- Your course adder application should be integrated with the azure devops.
- Your application should be viewed as an additional tab to the work item form.
- You should not ask for user login anymore, you should use different libraries provided by azure devops to get the
  user's information.
  specifically, the user-id which is also `uuid` and is unique for each user.

## Submission

The estimated time for each phase taking into account the time for learning the technologies is as follows:

- Phase 1: 50-60 hours
- Phase 2: 35-45 hours
- Phase 3: 20-30 hours

#### Note: Create a private github repository with 3 folders and a README file, the folders are named as follows:

- course-adder-frontend
- course-adder-backend
- course-adder-extension

#### Note: Add your mentor [Ali Najibi](https://github.com/anajibi) as a collaborator to your repository.

#### Note: After finishing each phase, schedule a meeting with your mentor to discuss your code and to review and get feedback on your code.
