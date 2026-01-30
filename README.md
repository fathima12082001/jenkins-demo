📘 Jenkins CI Project – GitHub Webhook Automation

🔹 Project Overview

This project demonstrates a fully automated Continuous Integration (CI) pipeline using Jenkins, GitHub Webhooks, and ngrok.

Every time code is pushed to GitHub, Jenkins automatically pulls the code and runs the build without manual intervention.

🔹 Tools & Technologies

- Jenkins

- Git & GitHub

- GitHub Webhooks

- ngrok

- Ubuntu (WSL)

- Shell scripting

🔹 CI Workflow

Developer → GitHub Push → Webhook → ngrok → Jenkins → Build

🔹 Jenkins Configuration

- Jenkins running on Ubuntu (WSL)

- Jenkins Port: 8080

- Job Type: Freestyle Project

- SCM: Git

- Branch: main


🔹 GitHub Webhook Setup

- Payload URL:
 https://<ngrok-url>/github-webhook/

- Content Type: application/json

- Event Trigger: Push

🔹 Jenkins Build Steps
echo "Hello Pathu"
echo "Jenkins is working"
whoami
hostname
date


🔹 GitHub Authentication
GitHub Personal Access Token (PAT) is used instead of passwords for secure Git operations.

🔹 Key Challenges Solved
DNS issues in WSL environment

Git branch mismatch (master vs main)

GitHub authentication using PAT

Exposing Jenkins to the internet using ngrok

Webhook debugging and delivery verification

verification

🔹 Outcome

Jenkins builds triggered automatically on every git push

Zero manual intervention

Fully functional CI pipeline

🔹 Learning Outcomes

Jenkins fundamentals

GitHub webhook automation

CI debugging and troubleshooting

Real-world DevOps workflow

🔹 Future Enhancements

Jenkins Pipelines (Jenkinsfile)

Docker-based builds

Deployment automation

Secure Jenkins with HTTPS


🔹 Author

Fathima Nasar
DevOps & Cloud Enthusiast 🌱
