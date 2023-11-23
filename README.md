# Backend_Bank_Service
- This project lab dives into advanced backend development using Go (Golang). It covers Golang, database management, asynchronous processing, infrastructure deployment, and security measures.

## Section 1: Database [Go & SQL]
### Languages: 
#### Golang
- Concurrency: Golang's built-in concurrency primitives like goroutines and channels facilitate efficient parallelism, enabling multiple tasks to run concurrently.
- Performance: Golang offers excellent performance due to its compiled nature and efficient memory management, making it suitable for high-performance applications.
- Strong Typing: Golang's static typing ensures type safety and reduces runtime errors, enhancing code reliability.
- Standard Library: Go boasts a comprehensive standard library, offering powerful tools and functionalities for various tasks without external dependencies.
- Simplicity: Golang emphasizes simplicity and readability, allowing developers to write clean, concise, and maintainable code.
- Cross-Platform Compatibility: Golang's compiler generates platform-independent binaries, facilitating seamless deployment across different operating systems.
#### SQL
- Data Integrity: SQL ensures data integrity through constraints (e.g., unique, not null) and transactions, maintaining the accuracy and consistency of stored data.
- Scalability: SQL databases are scalable, allowing efficient handling of increased workloads by scaling vertically or horizontally.
- Query Optimization: SQL databases utilize query optimization techniques to enhance query performance and execution efficiency.
- ACID Properties: SQL databases adhere to ACID (Atomicity, Consistency, Isolation, Durability) properties, ensuring reliable and robust transactions.
- Data Manipulation: SQL provides powerful data manipulation capabilities through operations like SELECT, INSERT, UPDATE, and DELETE, enabling efficient data retrieval and modification.
- Standardization: Being a standardized language, SQL ensures uniformity across different database platforms, promoting interoperability and ease of use.
### Tools:
- dbdiagram.io (Schema Design): Crafting and visualizing database structures.
- WSL2 (Development Environment): Windows Subsystem for Linux 2, facilitating Linux functionalities within Windows for seamless development.
- Visual Studio Code (IDE): Integrated Development Environment for coding and project management.
- Docker (Containerization): Platform for containerizing applications and database instances.
- Make (Build Automation): Tool for automating build processes.
- SQLc (SQL Compiler): Compiler generating Golang code from SQL queries.
- Postgres (Database Management): Relational Database Management System (RDBMS) for data storage.
- TablePlus (Database GUI): Graphical User Interface for managing databases.
- GitHub Actions (Automated Testing): CI/CD platform automating code testing and deployment.
### Technical Conceptts:
- Schema Design: Defining database structures, relationships, and constraints.
- Database Migration: Managing and applying changes to the database schema over time.
- CRUD Operations: Create, Read, Update, Delete actions on database records.
- ORMs (Object-Relational Mapping): gorm, sqlx - Tools for mapping database entities to objects in code.
- Unit Testing: Testing individual units of code, including database functions, in isolation.
- Transactions (DB Transactions): Bundling database operations into atomic units for consistency.
- Deadlock Handling: Strategies to prevent and resolve conflicts in concurrent transactions.
- Isolation Levels: Different levels of data visibility and consistency in transactions.
- Read Phenomena: Anomalies arising due to concurrent database access.

## Section 2: RESTful API (http json) [Gin Framework, Viper Configuration Library, PostgresSQL, Bcrypt, Gomock, JWT/Paseto]
### Tools:
- Gin Framework: Efficient routing and middleware capabilities for building performant APIs in Golang.
- Viper Configuration Library: Simplifies the loading of configurations from various sources.
- PostgreSQL: Relational Database Management System for data storage.
- Bcrypt: Encryption library for password hashing.
- Gomock: Enhances unit testing with custom matchers.
- PASETO & JWT: Token-based authentication mechanisms.
### Technical Concepts:
#### Golang:
- RESTful Design: Principles for API structuring and scalability.
- Middleware Implementation: Enforcing authentication and authorization rules.
- Custom Validation: Ensuring data integrity in API endpoints.
- Effective Error Handling: Managing database-related errors effectively.
#### SQL & Database Concepts:
- Database Constraints: Including unique and foreign key constraints for data integrity.
- Token-Based Authentication: Comparing PASETO and JWT for secure authentication.
- Password Security Measures: Securely storing passwords using Bcrypt encryption.
- Testing Strategies: Achieving 100% coverage by using mocks and custom matchers in unit tests.

## Section 3: Infrastructure & Deployment [Docker -> Kubernetes -> AWS]
### Tools:
- Docker: For containerization and image creation.
- docker-compose: For defining and managing multi-container Docker applications.
- AWS Services: ECR (Elastic Container Registry), RDS (Relational Database Service), Secrets Manager, Route53, EKS (Elastic Kubernetes Service).
- GitHub Actions: For automating build, testing, and deployment processes.
- Kubernetes (kubectl, k9s): For container orchestration and management.
### Technical Concepts:
#### Docker and Containerization:
- Multistage Dockerfile: Building small Golang Docker images using multistage builds.
- Docker Networking: Connecting standalone containers using Docker networks.
- docker-compose File: Configuring and managing service startup orders using docker-compose.
#### AWS Services and Cloud Deployment:
- AWS Account Setup: Creating a free-tier AWS account for cloud services.
- AWS ECR & GitHub Actions: Automating Docker image builds and pushes to AWS ECR with GitHub Actions.
- AWS RDS & Secrets Manager: Creating and managing a production database on AWS RDS, storing and retrieving secrets using AWS Secrets Manager.
#### Kubernetes and Deployment Orchestration:
- Kubernetes Architecture: Understanding Kubernetes architecture and creating EKS clusters on AWS.
- kubectl & k9s: Tools for connecting and managing Kubernetes clusters on AWS EKS.
- Deployment to Kubernetes: Deploying a web application to a Kubernetes cluster on AWS EKS.
- Ingress and Traffic Routing: Using Ingress to route traffic to different services within Kubernetes.
- TLS Certificate Management: Automatically issuing and renewing TLS certificates with cert-manager and Let's Encrypt.
- GitHub Action for Kubernetes: Automating deployment to Kubernetes with GitHub Actions.

## Section 4: Advanced Backend Develpment
### Tools:
- gRPC: For high-performance and language-agnostic API communication.
- protobuf: Protocol Buffers for defining gRPC APIs and generating Go code.
- Swagger: Tool for API documentation.
- SQLC: SQL compiler for generating Go code from SQL queries.
- Docker: For containerization.
- GitHub Actions: For automated workflows.
- HTTP Middleware: For handling HTTP requests.
- Front-end Embedding: To include static front-end files within the Golang server binary.
### Technical Concepts:
#### gRPC and API Development:
- Session Management: Handling user sessions using refresh tokens.
- gRPC Introduction: Understanding gRPC for efficient API communication.
- gRPC API Definition: Defining gRPC APIs and generating Go code with protobuf.
- gRPC Server Operations: Running a gRPC server and calling its APIs.
- gRPC Implementation: Creating and managing user-related gRPC APIs in Go.
- gRPC Gateway: Writing code to serve both gRPC and HTTP requests.
- gRPC Metadata: Extracting information from gRPC metadata.
#### Documentation and Code Structure:
- Database Documentation: Generating DB documentation and SQL schema dump from DBML.
- Swagger Documentation: Generating and serving Swagger documentation from a Go server.
- Front-end Embedding: Embedding static front-end files within the Golang backend server's binary.
#### Advanced Database Operations:
- gRPC Parameter Validation: Validating gRPC parameters for human and machine-friendly responses.
- DB Migrations: Running database migrations directly inside Golang code.
- Partial Record Update: Updating database records partially with SQLC nullable arguments.
- Optional Parameter API: Building gRPC update APIs with optional parameters.
- Authorization: Adding authorization to protect gRPC APIs.
#### Logging and Middleware:
- Structured Logs: Writing structured logs for gRPC APIs.
- HTTP Logger Middleware: Implementing HTTP logger middleware in Go for handling HTTP requests.

## Section 5: Asynchronous Processing & Email Handling in Go
### Tools:
- Redis: For task queuing and asynchronous processing.
- Gmail SMTP: For sending emails.
- Visual Studio Code: IDE configuration for testing in Go.
- Mocking: For unit testing with mock DB and Redis.
### Technical Concepts:
#### Asynchronous Processing:
- Background Worker: Implementing background workers using Redis task queues.
- Async Integration: Integrating async workers into a Go web server.
- Async Task Handling: Sending async tasks to Redis within a DB transaction.
- Error Handling: Managing errors and logging for async workers.
- Task Delay: Understanding the benefits of introducing delays in async tasks.
#### Email Handling:
- Email Sending: Sending emails in Go via Gmail SMTP.
- Email Verification Feature: Designing database schema and sending email for email verification.
- Email Verification API: Implementing email verification APIs in Go.
#### Testing and Unit Testing:
- Test Configuration: Configuring test flags in Visual Studio Code for Go.
- Skipping Tests: Understanding how to skip tests in Go.
- Unit Testing: Unit testing gRPC APIs with mock DB and Redis.
- Authenticated API Testing: Strategies for testing gRPC APIs that require authentication.

## Section 6: Server Security & Stability
### Tools:
- sqlc: SQL compiler with version 2 syntax for database operations.
- pgx: Database driver for PostgreSQL with enhanced features.
- Docker Compose: For managing port and volume mappings.
- Binary Packages in Go: Managing and using binary packages.
- AWS EKS Security Group: Managing access permissions for AWS services.
### Technical Concepts:
#### Database Management:
- sqlc Upgrade and Configuration: Upgrading and configuring sqlc with version 2 syntax.
- DB Driver Switch: Switching from lib/pq to pgx database driver.
- DB Error Handling: Properly handling database errors with the pgx driver.
#### Deployment and Infrastructure:
- Docker Compose Setup: Mapping ports and volumes using Docker Compose.
- Binary Package Management: Installing and using binary packages efficiently in Go.
#### Access Control and AWS Configuration:
- Role-Based Access Control (RBAC): Implementing RBAC in Go for access management.
- AWS EKS Cluster Access: Granting AWS EKS cluster access to Postgres and Redis using security groups.
- AWS EKS Deployment: Deploying gRPC and HTTP servers to an AWS EKS cluster.
