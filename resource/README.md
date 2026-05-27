````md
# 🚀 Terraform Azure Resource Group Project

![Terraform](https://img.shields.io/badge/Terraform-IaC-blueviolet?style=for-the-badge&logo=terraform)
![Azure](https://img.shields.io/badge/Azure-Cloud-blue?style=for-the-badge&logo=microsoftazure)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)

---

# 📌 Project Overview

This project demonstrates how to create and manage an Azure Resource Group using **Terraform Infrastructure as Code (IaC)**.

Terraform automates cloud infrastructure deployment using simple configuration files.

Using this project, we can:
- Create Azure Resource Group
- Automate Infrastructure
- Manage Cloud Resources
- Learn DevOps Practices

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Terraform | Infrastructure as Code |
| Microsoft Azure | Cloud Platform |
| VS Code | Code Editor |
| Git & GitHub | Version Control |

---

# 📂 Project Structure

```text
terraform-test/
│
├── main.tf
├── README.md
├── .gitignore
````

---

# ⚙ Terraform Configuration

## 📄 main.tf

```hcl
provider "azurerm" {
  features {}
  subscription_id = "YOUR_SUBSCRIPTION_ID"
}

resource "azurerm_resource_group" "rg" {
  name     = "demo-resource-group"
  location = "Central India"
}
```

---

# 🚀 Terraform Workflow

## 1️⃣ Initialize Terraform

```bash
terraform init
```

Downloads required providers and initializes Terraform.

---

## 2️⃣ Validate Configuration

```bash
terraform validate
```

Checks whether configuration is correct.

---

## 3️⃣ Generate Execution Plan

```bash
terraform plan
```

Shows what Terraform will create before deployment.

---

## 4️⃣ Apply Infrastructure

```bash
terraform apply
```

Creates Azure Resource Group in Azure Cloud.

---

## 5️⃣ Destroy Infrastructure

```bash
terraform destroy
```

Deletes created resources.

---

# ☁ Azure Resource Group Details

| Property      | Value                |
| ------------- | -------------------- |
| Resource Type | Azure Resource Group |
| Location      | Central India        |
| Provider      | AzureRM              |
| IaC Tool      | Terraform            |

---

# 📷 Deployment Screenshot

Add your screenshots here:

## Terraform Init

![Terraform Init](./screenshots/init.png)

---

## Terraform Plan

![Terraform Plan](./screenshots/plan.png)

---

## Terraform Apply

![Terraform Apply](./screenshots/apply.png)

---

## Azure Portal Output

![Azure Portal](./screenshots/azure-portal.png)

---

# 🛡 .gitignore File

```gitignore
.terraform/
*.tfstate
*.tfstate.backup
```

---

# 🔥 DevOps Concepts Used

* Infrastructure as Code (IaC)
* Cloud Automation
* Azure Cloud Deployment
* Terraform Providers
* Resource Management
* GitHub Version Control

---

# 📈 Future Improvements

* Add Azure Virtual Machine
* Add Storage Account
* Add Virtual Network
* Use Terraform Variables
* Create Terraform Modules

---

# 👨‍💻 Author

## Anand Janke

🎓 BCA Student (2026)
🏫 Makhanlal Chaturvedi University, Bhopal

### Skills

* Terraform
* AWS
* Azure
* Docker
* Kubernetes
* Git & GitHub
* Linux
* CI/CD

📧 Email: [anandjanke2112@gmail.com](mailto:anandjanke2112@gmail.com)

🌐 GitHub:
[https://github.com/anand-devops-01](https://github.com/anand-devops-01)

---

# ⭐ Project Purpose

This project is created for:

* DevOps Learning
* Cloud Practice
* Terraform Practice
* GitHub Portfolio
* College Submission

---

# 🙌 Thank You

If you like this project, give it a ⭐ on GitHub.

```
```
