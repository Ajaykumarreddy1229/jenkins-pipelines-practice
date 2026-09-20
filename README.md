# jenkins-pipelines-practice
Jenkins Pipeline as Code 
This project demonstrates my learning and practice with Jenkins Pipeline as Code as part of my DevOps learning journey.

**📌 Overview**
The project focuses on creating Jenkins pipelines using a Jenkinsfile to automate different stages of the CI/CD workflow.
Instead of performing build, testing, code-quality analysis, and deployment manually, Jenkins can execute these tasks through an automated pipeline.


**🔄 Pipeline Workflow**
GitHub
   ↓
Checkout Code
   ↓
Maven Build
   ↓
Testing
   ↓
SonarQube Code Quality
   ↓
Deployment

**🛠️ Technologies Used**
1.Jenkins
2.Jenkins Pipeline
3.Git / GitHub
4.Maven
5.Java
6.SonarQube
7.Apache Tomcat
8.Docker


**📋 Pipeline Stages Practiced**
1. Checkout Code
The pipeline can retrieve the project source code from GitHub.
2. Build
Maven is used to clean and package the application:
mvn clean package
3. Test
Automated tests can be executed using:
mvn test
4. Code Quality
SonarQube analysis can be integrated into the pipeline:
mvn sonar:sonar
5. Deployment
The generated WAR file can be copied to the Tomcat deployment directory.
6. Docker Deployment
I also practiced building a Docker image, pushing it to a registry, and running the application using Docker.
7. Parallel Testing
The pipeline can execute different testing activities in parallel to organize the testing workflow.
8. Notifications
Post-build actions can be used to report whether the pipeline completed successfully or failed.

**🎯 Key Learning**
Through this practice, I learned how Jenkins Pipeline as Code can be used to define and automate a CI/CD workflow.
This makes the pipeline easier to manage, repeat, and integrate with source-control repositories.
