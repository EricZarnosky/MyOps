# ⚙️ MyOps: Learn it. Build it. Automate everything.

**MyOps** is my personal automation and infrastructure framework — built for experimentation, repeatable deployments, and managing infrastructure-as-code across Kubernetes clusters, Docker platforms, virtualization stacks, and cloud environments.

> ⚠️ **Work In Progress**  
> This repository is a continuous work in progress. Initial commits may be slow as I actively learn new tools and refine how automation is applied across various technologies and environments.  
> Contributions, suggestions, and feedback are welcome as I grow this into a robust, reusable infrastructure framework.

---

## 📦 Features

- 🧠 **FluxCD-based GitOps** for managing multiple Kubernetes clusters:
  - Home lab
  - VPS (Cloud)
  - Business/Client Deployments
  - Learning environments

- 🛠️ **Infrastructure as Code** using:
  - Terraform (cloud, VPS, Proxmox, vSphere, etc.)
  - Azure Bicep (Azure + Azure HCI)
  - Ansible (bare-metal, cloud VMs, Active Directory, etc.)

- 🐳 **Docker Environments**:
  - Compose-based services
  - Single-node and Swarm mode setups
  - Helm charts and Kubernetes manifests

- 🖥️ **Virtualization & Orchestration**:
  - **Proxmox VE** and **LXC** containers
  - **VMware vSphere**, vCenter, Horizon VDI
  - **SUSE Harvester** (experimental)

- 🔐 **Secrets & Access**:
  - OpenBao (Vault) for secret management
  - Secure credentials for automation pipelines

- ⚙️ **CI/CD and Workflow Automation**:
  - Jenkins pipelines
  - Kestra orchestrations
  - GitOps-first workflows with FluxCD

---

## 🗂️ Repository Structure

```text
.
├── k8s/               # GitOps & Flux-managed Kubernetes deployments
│   ├── apps/
│   ├── clusters/
│   └── base/
├── ansible/           # Ansible playbooks and roles
├── docker/            # Docker Compose and Swarm configs
├── terraform/         # IAC for cloud, Proxmox, vSphere, etc.
├── azure/             # Bicep templates and Azure-specific deployments
├── vmware/            # vSphere, vCenter, Horizon automation
├── proxmox/           # LXC/VM provisioning and config
├── ci-cd/             # Jenkins and Kestra automation
├── docs/              # Planning, architecture, notes
└── README.md
```

---

## 🧪 Clusters
| Cluster         | Purpose                         | Location         |
| --------------- | ------------------------------- | ---------------- |
| `MediaStack`    | Home media + storage automation | Home Lab         |
| `Lab`           | R\&D, new app testing           | Local / Cloud    |
| `LearningLab`   | Used for learning in Kubecraft  | Home Lab         |
| *(more coming)* | Dev, staging, and production    | Various          |

---

## 🤝 Acknowledgements & Attribution
MyOps is built on the foundation of amazing open-source tools, guides, repositories, and community knowledge.

I strive to credit all original authors or sources whenever their code, patterns, or ideas are used. This project is a culmination of shared knowledge, shaped by tutorials, blog posts, forums, GitHub repos, and documentation from countless contributors in the open-source world.

If you believe I’ve used something without proper credit, please open an issue or PR so I can correct it.

---

## 💡 Goals
Build repeatable, scalable, declarative infrastructure

Centralize infrastructure management using GitOps

Apply automation from bare metal to production

Maintain a modular, documented IaC library

Serve as both a production toolkit and learning environment

---

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
