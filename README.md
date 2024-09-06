Overview
This repository contains a Maven-based Java web application that is integrated with Jenkins for Continuous Integration (CI) and Continuous Deployment (CD). The project is structured into two Jenkins pipelines that automate the build and deployment stages, streamlining the software development lifecycle.

Pipeline Structure
1. Build Pipeline
Purpose: Automates the compilation and packaging of the Java web application.
Steps:
Jenkins triggers the pipeline upon code commit.
Maven is used to clean, compile, and package the application into a deployable artifact (e.g., WAR or JAR file).
The build artifact is archived for the deployment stage.

2. Deploy Pipeline
Purpose: Automates the deployment of the built artifact to a staging or production environment.
Steps:
Deploys the artifact to a web server (e.g., Apache Tomcat) or a cloud-based environment.
Notifies stakeholders upon successful deployment.
Optionally includes steps for basic post-deployment checks to verify that the application is running correctly.
