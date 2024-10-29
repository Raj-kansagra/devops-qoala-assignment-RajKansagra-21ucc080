# DevOps Assignment: Debugging and Running a Dockerized Application

Welcome to your DevOps assignment! Your goal is to debug and deploy a Dockerized application. The steps below outline the tasks you’ll complete, including setup, debugging, running, testing, and submitting your work.

## Assignment Overview

In this assignment, you’ll:
1. Set up Docker and Docker Compose.
2. Build Docker images and launch containers.
3. Debug and resolve intentional errors in the code to ensure the application runs correctly.
4. Verify the application in your browser.
5. Document your process and submit your work.

---

## Requirements

**Tools Needed:**
- **System:** Use any laptop, PC, or cloud server.
- **Tools:** Docker and Docker Compose must be installed and configured.

---

## Steps

### 1. Initial Setup
1. **Clone the GitHub Repository:**
   - Start by cloning the provided GitHub repository, which contains the `Dockerfiles`, `docker-compose.yml` file, and the application code.
   
2. **Build Docker Images:**
   - Build each Docker image locally using the provided Dockerfiles.
   - Tag each image appropriately to be referenced by the `docker-compose.yml` file.

### 2. Running the Docker Compose File
1. **Start the Containers:**
   - Use the provided `docker-compose.yml` file to launch all containers.
   - **Note:** There are intentional errors in the code. Part of your assignment is to identify and fix these errors so the application runs correctly.

### 3. Debugging and Testing
1. **Identify Issues:**
   - Check the logs for any errors while building and running containers.
   - Examine the application code, Dockerfiles, and `docker-compose.yml` file to identify intentional errors.

2. **Resolve Errors:**
   - Document the issues and explain your debugging steps.
   - Apply necessary changes to the code, Dockerfiles, or configuration to resolve these errors.

3. **Verify Website Access:**
   - Open a web browser and access the application on `http://localhost` (or `http://<server-IP>` if hosted on a cloud server) to confirm it is running correctly.
   - Check Nginx or other web server logs to confirm requests are being logged as expected.

### 4. Submitting the Assignment
1. **GitHub Repository:**
   - Create a new GitHub repository and name it in this format: `devops-qoala-assignment-<name>-<rollnumber>`.
   - Upload all relevant files (including the modified code, Dockerfiles, `docker-compose.yml`, and other configurations) to this repository.
   - Grant access to `devops@qoala.id`. **Note:** Submissions without access granted will not be considered.

2. **Screenshots:**
   - Take a screenshot of the application running in the browser.
   - Include a screenshot showing Nginx (or web server) access logs that confirm a successful request.

3. **Report:**
   - Write a concise, one-page report that includes:
     - **Issues Identified:** Summarize any errors encountered during image building, container setup, or application testing.
     - **Resolution Steps:** Describe each action taken to resolve the issues and ensure the application runs correctly.

---

## Bonus Points

### Cloud Deployment
- For extra credit, deploy the application on a cloud server (AWS, GCP, or Azure) and provide an accessible endpoint, such as an IP address or DNS record.
- This will allow your work to be verified through the shared endpoint.

---

## Summary Checklist
- Set up Docker and Docker Compose.
- Clone and build Docker images.
- Debug and fix issues in code, Dockerfiles, or `docker-compose.yml`.
- Start containers and verify application accessibility on port 80.
- Upload files to a new GitHub repository and grant access to `devops@qoala.id`.
- Submit screenshots and a concise report of issues and solutions.
- (Bonus) Deploy on a cloud provider and share endpoint details.

---

Good luck, and happy debugging!
