# .NET Project Manager

## Description
Project and task management system that encompasses all the points outlined in the .NET Developer Roadmap 2024. The system will allow users to create, view, edit, and manage projects and tasks, applying best practices and technologies from the .NET ecosystem. 

The project covers various aspects of .NET development, including C#, ASP.NET Core, client-side .NET technologies, databases, ORM, communication, observability, containerization, cloud services, continuous integration & delivery, and .NET libraries.

## Credits
This project is inspired by the [.NET Developer Roadmap](https://github.com/milanm/DotNet-Developer-Roadmap) created by [milanm](https://github.com/milanm). The roadmap provides a structured guide for .NET developers to navigate through various technologies, libraries, and best practices in the .NET ecosystem.

## Features
### Authentication and Authorization
- Users must be able to register and log in to the system.
- Authentication must be secure and support different levels of access (e.g., administrator, regular user).

### Project Management
- Users can create new projects.
- Each project will have a name, description, and start/due date.
- Projects can be edited and deleted by administrators and users who created them.

### Task Management
- Users can add tasks to existing projects.
- Each task will have a name, description, deadline, and status (to do, in progress, completed, overdue).
- Tasks can be assigned to different team members.

### Integration with .NET Libraries
- Integration with `MediatR` for implementing mediator patterns.
- Use of `Polly` for fault handling and resilience policies.

### Observability with Logging and Monitoring
- Logging implementation using `Microsoft.Extensions.Logging` and `Serilog` to monitor and track system activities.
- Configuration of metrics and telemetry with Grafana and OpelTelemetry for monitoring system performance and behavior.

### Containerization and Orchestration
- Application containerization using `Docker`.
- Deployment of the application in a `Kubernetes` orchestration environment for scalability and simplified management.

### Cloud Integration with Azure and AWS
- Integration with `Azure` and `AWS` for cloud services such as storage, compute, and networking.
- Utilization of cloud-native features for scalability, reliability, and performance.

### Continuous Integration & Delivery with GitHub Actions and Azure Pipelines
- Implementation of CI/CD pipelines using GitHub Actions and Azure Pipelines.
- Automated testing, building, and deployment processes to ensure the reliability and consistency of the application.

## Acceptance Criteria
- Users should be able to register and log in successfully.
- Projects should be created and listed correctly in the user interface.
- Tasks should be added, edited, and deleted without issues.
- Authentication, creation, editing, and deletion operations should be protected by appropriate authorization.
- The system should integrate .NET libraries as specified.
- Logging records should be consistent and understandable.
- Monitoring with `Grafana` and `OpelTelemetry` should present relevant and accurate metrics.
- Cloud integration with `Azure` and `AWS` should provide seamless access to cloud services.
- Continuous integration & delivery with `GitHub Actions` and `Azure Pipelines` should ensure automated testing and deployment workflows.

## Test Scenarios

### Registration and Login
- **Positive Scenario:** A user can register successfully and log in using their credentials.
- **Negative Scenario:** Attempting to log in with invalid credentials should fail.

### Project Management
- **Positive Scenario:** A user can create a new project successfully.
- **Negative Scenario:** Attempting to create a project without filling in all mandatory fields should fail.

### Task Management
- **Positive Scenario:** A user can add a new task to an existing project successfully.
- **Negative Scenario:** Attempting to add a task without specifying a deadline should fail.

### Integration with .NET Libraries
- **Positive Scenario:** Functionalities implemented with MediatR and Polly work as expected.
- **Negative Scenario:** Unexpected failures should be handled correctly by policies defined with Polly.

### Observability
- **Positive Scenario:** Logging records are consistent and understandable.
- **Negative Scenario:** Critical failures are not being recorded properly.

### Containerization and Orchestration
- **Positive Scenario:** The application is successfully deployed in a Kubernetes cluster and can be scaled as needed.
- **Negative Scenario:** Configuration or deployment issues prevent the application from running in the Kubernetes environment.

## Installation and Setup
1. Clone the repository: `git clone https://github.com/renanfssilva/dotnet-project-manager.git`
2. Install dependencies: `dotnet restore`
3. Configure environment variables and database connection strings as needed.
4. Build and run the project: `dotnet run`

## Usage:
- Register and login to access the application.
- Create projects and add tasks to manage your workflow.
- Explore different features and functionalities aligned with the .NET Developer Roadmap.

## Contributing:
Contributions are welcome! Feel free to submit issues, feature requests, or pull requests.

## License:
This project is licensed under the [GPL-3.0 license](https://github.com/renanfssilva/dotnet-project-manager?tab=GPL-3.0-1-ov-file).

## Contact:
For any inquiries or feedback, please contact [Renan](mailto:renanfssilva@gmail.com).
