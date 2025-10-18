Assignemnt_(mod 10) Integrate SonarQube with GitHub
Assignment: Integrate SonarQube with GitHub Actions for Code Quality Analysis

Objective:

Set up SonarQube with a sample project and configure GitHub Actions to automatically analyze code quality on every push. At the end, a SonarQube report should be generated and viewable through the dashboard.

 

Project Requirements:

A sample project in Java, Python, or JavaScript (your choice).

GitHub repository for version control and CI setup.

Steps to Follow:

1. Prepare the Environment

Install or access a SonarQube server (can be local via Docker or on a shared remote instance).

Set up a SonarQube Token for authentication.

2. Create a Sample Project

Initialize a Git repository with a basic Java/Python/JS project.

Add at least one class/module with simple logic.

Include minimal test cases if possible.

3. Configure SonarQube

Create a new project in the SonarQube dashboard.

Configure the project settings to get the projectKey and token.

4. Add SonarQube Scanner Configuration

Add a configuration file (sonar-project.properties) in the root of your project.

Fill it with necessary fields like sonar.projectKey, sonar.host.url, and sonar.login.

 

 

5. Set Up GitHub Actions Workflow

Create a .github/workflows/sonarqube.yml file.

Configure it to:

Checkout the code

Set up the environment (Java or Python depending on your project)

Install required dependencies

Run the SonarQube scanner using the token and project key

6. Run the Workflow

Push your changes to GitHub to trigger the workflow.

Verify that GitHub Actions runs and connects with SonarQube.