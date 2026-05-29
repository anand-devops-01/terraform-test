````md id="g7m2x5"
# ☁️ Terraform Azure Storage Account Project

![Terraform](https://img.shields.io/badge/Terraform-IaC-blueviolet?style=for-the-badge&logo=terraform)
![Azure](https://img.shields.io/badge/Azure-Cloud-blue?style=for-the-badge&logo=microsoftazure)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)

---

# 📌 Project Overview

This project demonstrates how to create an Azure Storage Account using Terraform Infrastructure as Code (IaC).

Terraform automates cloud resource deployment using configuration files.

Using this project, we can:
- Create Azure Storage Account
- Create Blob Container
- Upload Blob/File
- Manage Azure Resources Automatically

---

# 🚀 Technologies Used

| Technology | Purpose |
|------------|---------|
| Terraform | Infrastructure as Code |
| Microsoft Azure | Cloud Platform |
| VS Code | Code Editor |
| Git & GitHub | Version Control |

---

# 📂 Project Structure

```text
terraform-storage-project/
│
├── main.tf
├── README.md
├── .gitignore
````

---

# ⚙️ Terraform Configuration

## 📄 main.tf

```hcl id="ql08fh"
provider "azurerm" {
  features {}
  subscription_id = "YOUR_SUBSCRIPTION_ID"
}

resource "azurerm_resource_group" "rg" {
  name     = "storage-rg"
  location = "Central India"
}

resource "azurerm_storage_account" "storage" {
  name                     = "prodstrdemo"
  resource_group_name      = azurerm_resource_group.rg.name
  location                 = azurerm_resource_group.rg.location
  account_tier             = "Standard"
  account_replication_type = "LRS"
}

resource "azurerm_storage_container" "container" {
  name                  = "prodcontainer"
  storage_account_name  = azurerm_storage_account.storage.name
  container_access_type = "private"
}
```

---

# 🔥 Resources Created

✅ Azure Resource Group
✅ Azure Storage Account
✅ Azure Storage Container

---

# 🚀 Terraform Workflow

## 1️⃣ Initialize Terraform

```bash id="n42a9e"
terraform init
```

Downloads Terraform providers.

---

## 2️⃣ Validate Configuration

```bash id="ycv8yw"
terraform validate
```

Checks syntax and configuration.

---

## 3️⃣ Generate Execution Plan

```bash id="tck6zj"
terraform plan
```

Shows resources Terraform will create.

---

## 4️⃣ Apply Infrastructure

```bash id="ub0z44"
terraform apply
```

Deploys Azure infrastructure.

---

## 5️⃣ Destroy Infrastructure

```bash id="75hvx6"
terraform destroy
```

Deletes all created resources.

---

# ☁️ Azure Resources Details

| Resource        | Description   |
| --------------- | ------------- |
| Resource Group  | storage-rg    |
| Storage Account | prodstrdemo   |
| Storage Tier    | Standard      |
| Replication     | LRS           |
| Container       | prodcontainer |

---

# 📷 Deployment Screenshots

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

# 🛡️ .gitignore

```gitignore id="80llyi"
.terraform/
*.tfstate
*.tfstate.backup
```

---

# 💡 DevOps Concepts Used

* Infrastructure as Code (IaC)
* Cloud Automation
* Azure Resource Management
* Terraform Providers
* Storage Services
* GitHub Version Control

---

# 📈 Future Improvements

* Add Blob Upload Automation
* Add Virtual Network
* Add Azure VM
* Use Terraform Variables
* Create Reusable Terraform Modules

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
* Linux
* Git & GitHub
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
* Azure Automation
* GitHub Portfolio

---

# 🙌 Thank You

If you like this project, give it a ⭐ on GitHub.

```
```
