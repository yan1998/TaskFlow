# TaskFlow project requirements

## General
1. System contains the following user roles: Administrator, Project administrator, User, Guest.
2. The system allows to create projects and boards within.
3. The board consist of several columns.
4. Tickets can be created and placed to boards. User can move tickets between columns
5. Notifications are sent for ticket if user is subscribed on it.
6. Reports and diagrams could be created for board/projects

## Roles definition
1. Guest - the basic role which doesn’t require registration and authorization.
    * Guests can see public projects and boards

2. User - extends guest role and requires registration and authorization.
    * Can see private projects and boards in case of access is allowed
    * Can create tasks and edit the existing ones
    * Can move tasks between columns and left comments
    * Can edit user information data and credentials
    * Can subscribe/unsubscribe on events related to the ticket (status changed/description is added, etc)

3. Project administrator - extends user role and allows to configure project/s
    * Can create boards in project/s
    * Can manage an access to project/projects
    * Can invite new users to the project/s
    * Can remove comments/tasks/boards

4. Administrator - extends project administrator and allows to configure all projects in system
    * Can create projects
    * Can manage an access to projects
    * Can invite new project administrators to the project/s
    * Can manage user management (remove/reset credentials) for users

## Technical stack
1. .NET 8, C#, ASP.NET Core
2. MS SQL
3. RabbitMQ
4. Docker, Kubernetes, Helm, Istio