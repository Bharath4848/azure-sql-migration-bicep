# azure-sql-migration-bicep
# 🚀 Azure SQL Server Migration – Bicep Templates

This repository contains **modular, production-ready Azure Bicep templates** designed to automate the infrastructure deployment for SQL Server migration projects. It provides everything needed to create and manage resources like Virtual Networks, SQL Managed Instances, Private DNS Zones, Private Endpoints, and Storage Accounts using CI/CD pipelines.

> 💡 It supports both **Dev** and **Prod** environments with separate parameter files and flexible deployments via Azure CLI or DevOps pipelines.

---

## 📂 Repository Structure

```text
azure-sql-migration-bicep/
├── bicep/
│   ├── main.bicep                      # Entry point for deployments
│   └── modules/                        # Modular, reusable Bicep templates
│       ├── Vnet.bicep
│       ├── sqlmi.bicep
│       ├── dnsZones.bicep
|       ├── storageAccount.bicep
│       └── privateEndpoints.bicep
├── variables/                          # Parameter files per environment
│   ├── dev-config.yml
│   └── prod-config.yml
├── pipelines/                          # Azure DevOps pipeline definition
│   └── azure-pipelines.yml
├── .github/                            # (Optional) GitHub Actions workflows
│   └── workflows/
│       └── deploy.yml
├── .gitignore
├── LICENSE
├── CONTRIBUTING.md
└── README.md
```

---

