
# NextWork Web Project

A Java web application deployed on an AWS EC2 instance and version-controlled using Git and GitHub. This project is part of the **7 Day DevOps Challenge** and demonstrates how to set up a local Git repository, connect it to GitHub, and manage version control in the cloud.

---

## 📌 Project Overview

This project involved:

- Setting up a Java web app on an EC2 instance.
- Installing Git on the instance.
- Creating and configuring a GitHub repository.
- Initializing a local Git repository in the project folder.
- Connecting the local repo to GitHub and pushing project files.
- Making and pushing updates to track version history.
- Securing GitHub authentication using personal access tokens (PAT).

---

## ⚙️ Services Used

- **Amazon EC2 (Amazon Linux 2023)**  
  For hosting and developing the Java web app.

- **Git**  
  For local version control and change tracking.

- **GitHub**  
  For cloud-based storage of the project code and remote version control.

---

## 🧠 Key Concepts Learned

- Version control with Git
- GitHub repository creation and management
- Setting up a local and remote Git connection
- Using Git commands: `init`, `add`, `commit`, `push`
- Creating and using GitHub personal access tokens (PATs)
- Staging, committing, and pushing code changes
- Understanding local vs. remote repositories

---

## 🛠️ Setup Instructions

1. **Launch EC2 Instance**  
   - OS: Amazon Linux 2023  
   - Tools installed: Maven, Java (Corretto 8), Git

2. **Install Git**  
   ```bash
   sudo dnf update -y
   sudo dnf install git -y
   git --version
   ```

3. **Create GitHub Repository**  
   - Repo name: `nextwork-web-project`  
   - Description: Java web app set up on an EC2 instance  
   - Visibility: Public  
   - Include a README

4. **Connect Local Repo to GitHub**
   ```bash
   git init
   git remote add origin https://github.com/your-username/nextwork-web-project.git
   git add .
   git commit -m "Initial commit"
   git push -u origin master
   ```

5. **Set Up GitHub Token (for HTTPS Auth)**
   - Generated classic PAT with `repo` scope
   - Used token instead of password when prompted by Git

6. **Configure Git Identity**
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your@email.com"
   ```

7. **Push Updates**
   ```bash
   git add .
   git commit -m "Add new line to index.jsp"
   git push
   ```

---

## 🖥️ What the Project Does

This is a basic Java web application using JSP deployed on an EC2 server. The main index page was updated to include a message confirming successful sync to GitHub.

---

## ⏳ Time Spent

This project took me approximately **2 hours** to complete.  
The most challenging part was **configuring GitHub authentication using a personal access token**.  
It was most rewarding to **see my web app files pushed and live in my GitHub repository**.

---

## 📄 Author

**[Your Name]**  
DevOps Engineer | Participant in the NextWork 7 Day DevOps Challenge

---

## 🔐 Important Notes

- Don’t forget to delete your EC2 instance and key pair after completing this project to avoid AWS charges.
- Use GitHub tokens instead of passwords for secure access.

---

## 🏁 Next Steps

Up next in the 7 Day DevOps Challenge:  
**Secure and manage packages with AWS CodeArtifact**

---


