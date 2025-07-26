# techeasy_DEVOPS_swaraj

# DevOps Assignment – EC2 + S3 Simulation (No AWS)

This assignment simulates AWS DevOps tasks entirely on a local machine.

## Features

- EC2 Setup simulated with Bash scripts (deploy.sh)
- Java + Maven installation
- App cloned from: https://github.com/Trainings-TechEazy/test-repo-for-devops
- App deployed to port 80
- /hello endpoint tested and functional
- Logs archived using stop.sh
- Logs uploaded to simulated S3 folder
- Lifecycle rule deletes logs older than 7 days
- Dev/Prod config support via .env files
- No AWS account used; fully local setup

## To Run

```bash
./deploy.sh dev
curl http://localhost/hello
./stop.sh
python upload_logs.py
python delete_old_logs.py