# TaskFlow
Pet-project to learn Docker/Kubernetes to build microservice architecture

**Project Idea:** Real-time Task Manager with Microservices Architecture

**Description:**
Create a real-time task manager application where users can create, update, and track tasks. The application will consist of multiple microservices, each responsible for specific functionalities. The use of Docker containers and Kubernetes will enable easy scaling and management of these microservices.

**Key Components:**
1. Web API (.NET): Develop a RESTful API using .NET that handles user authentication, task creation, updating, and retrieval. Ensure that the API supports real-time communication.
2. Database Microservice (MSSQL): Create a microservice responsible for managing the database (MSSQL) and handling data storage and retrieval.
3. Notification Microservice (RabbitMQ): Implement a microservice that utilizes RabbitMQ for handling real-time notifications. Whenever a task is created or updated, a notification is sent to users who are involved in that task.
4. Containerization (Docker): Containerize each microservice using Docker, making it easier to deploy and manage them across different environments.
5. Orchestration (Kubernetes): Use Kubernetes for orchestrating and managing the deployment of your Docker containers. This will allow you to scale, update, and monitor your microservices efficiently.
6. Helm Chart: Create Helm charts for each microservice to simplify the deployment and configuration process. Helm charts make it easy to package and deploy applications on Kubernetes.
7. Azure Integration (Future Enhancement): As a future enhancement, integrate your application with Azure services such as Azure Active Directory for enhanced authentication and authorization. You can also explore Azure Kubernetes Service (AKS) for managed Kubernetes clusters.

**Additional Features:**
* User authentication and authorization.
* Real-time updates using SignalR for the web interface.
* Task categorization and priority management.
* User dashboard for task tracking.
* Support for attachments and comments on tasks.
