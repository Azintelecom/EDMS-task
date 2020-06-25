# EDMS-task

EDMS (https://en.wikipedia.org/wiki/Document_management_system) system is a system for managing documents within an organisation.

The purpose of this task is to create EDMS system for Azintelecom adhering to our business flow.

### How to start
Fork this repository to your account. Work on these tasks and then make a pull request when you finish. We will then evaluate your results. You can work in teams, however we will take into account each member\`s contribution.

## Backend

### Auth
- Login - the user can login (email and password) and receive JWT token that will be set on the browser.
- Logout - the user\`s token is erased from the browser.
- Me - return the information about the current user, name, email, permissions

### Roles
Roles (CRUD) - an endpoint that adds/retrieves/updates/deletes a role. Each role has a name and unique id.
Only admin user has access to roles.

### Users
Users (CRUD) - an endpoint that adds/retrieves/updates/deletes a user. Each user has a name, email, roles.
Only admin user has access to users.

### Categories
Categories (CRUD) - an endpoint that adds/retrieves/updates/deletes a category. Each category has a name and a parent category (optional if the root one).
Only admin user has access to users.
Also, you can list the documents belonging to that category,

### Document
Documents (CRUD) - an endpoint that adds/retrieves/updates/deletes a document. Each document has a name, a file, and a category it belongs to.
Users with needed permissions can work with documents (AddDocument role, EditDocument role, ViewDocument role, DeleteDocument role).

### Workflow
Workflows (CRUD) - an endpoint that adds/retrieves/updates/deletes a workflow.
Only admin user has access to workflows.

#### Workflow states
Each workflow can have a number of states (finite state machine):
![EDMS](./EMDS.png)

## Databases

## Frontend
TODO: Requirements: Vue.Js, React

## Deployment

TODO: Requirements: Docker + Dockercompose
