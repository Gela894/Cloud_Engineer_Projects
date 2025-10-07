# 🚀 Project Name – Cloud/DevOps Demo

A hands-on project to showcase Linux, Docker, Terraform, Ansible, and Kubernetes skills.
This repo provisions secure AWS infrastructure, configures hosts, deploys a containerized app,
and sets up monitoring & blue/green deployments.

## 🏗️ Architecture
![Architecture Diagram](diagrams/architecture.png)

- **Cloud:** AWS (VPC, EC2, ALB, S3, IAM)
- **Config Management:** Ansible
- **IaC:** Terraform (multi-env modules)
- **Container:** Docker
- **Orchestration:** Kubernetes (optional)
- **CI/CD:** GitHub Actions

## 🔧 Quick Start

```bash
# 1. Clone repo
git clone https://github.com/yourname/project-name.git
cd project-name

# 2. Deploy dev env
cd terraform/envs/dev
terraform init
terraform plan
terraform apply

# 3. Configure with Ansible
cd ../../ansible
ansible-playbook -i inventories/dev/hosts.ini site.yml

