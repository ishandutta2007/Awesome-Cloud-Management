# Awesome-Cloud-Management

# Top Cloud Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Multi-Cloud Orchestration, FinOps & Infrastructure Governance*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Management**. These tools enable organizations to provision, orchestrate, govern, and optimize resources across public, private, and hybrid cloud environments—controlling costs, enforcing policies, and maintaining visibility over distributed infrastructure.

**Examples** include ServiceNow Cloud Management (now Cloud Provisioning and Governance), Flexera, CloudHealth by Broadcom, Morpheus Data (HPE), Spot by NetApp, Apptio Cloudability, Nutanix Beam (NCM Cost Governance), Turbonomic, Scalr, and CloudBolt (the category leaders).

**Open-source emphasis**: This section is expanded with active projects for self-hosted FinOps, Infrastructure-as-Code management, and cloud cost optimization—ideal for platform teams and FinOps practitioners building sovereign cloud management infrastructure without per-resource or per-workload licensing lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[ServiceNow Cloud Management](https://www.servicenow.com/)**  
  Now branded as **Cloud Provisioning and Governance (CPG)**, this module on the Now Platform provides cloud user and admin portals, resource profiles, Terraform integration, policy enforcement, and multi-cloud support for AWS, Azure, and VMware; positioned as an integrated CMP for organizations already on ServiceNow, though some users note it lags behind dedicated CMP tools in feature depth .

- **[Flexera](https://www.flexera.com/)**  
  Hybrid IT management platform with cloud management capabilities including orchestration, automation, provisioning, and inventory across multi-vendor environments; Gartner reviewers note a smooth UI and accurate information, though support resolution can be slow . Flexera's Snow Commander offers self-service hybrid cloud provisioning with automated lifecycle management and policy-driven resource decommissioning .

- **[CloudHealth by Broadcom](https://www.broadcom.com/)**  
  FinOps and cloud spend management platform (VMware Tanzu CloudHealth) with a new AI-powered experience featuring Intelligent Assist (natural language FinOps co-pilot) and Smart Summary (cost change analysis); recently GA'd under Broadcom with Arrow Electronics as sole global provider; users report strong multi-cloud visibility but note intermittent data gaps and a steep learning curve .

- **[Morpheus Data (HPE)](https://morpheusdata.com/)**  
  Infrastructure-agnostic multi-cloud management platform for hybrid IT and DevOps automation; provides unified orchestration across VMs, containers, and bare metal with FinOps-focused cost tracking and optimization; now part of HPE as HPE Morpheus Enterprise Software; users note licensing can be complex but cost-effective compared to competitors .

- **[Spot by NetApp](https://www.netapp.com/)**  
  Cloud optimization suite that continuously analyzes and automates cloud operations to improve efficiency and reduce costs across compute, storage, and security resources .

- **[Apptio Cloudability](https://www.apptio.com/)**  
  FinOps platform (IBM company) used as a single source of truth for cloud costs; Apptio's own P&E team used Cloudability to optimize unit costs by 30% and automated 1,400+ actions per month with no human touch, ranging from RI conversions to dynamic resource parking .

- **[Nutanix Beam (NCM Cost Governance)](https://www.nutanix.com/)**  
  Multi-cloud cost governance platform (formerly Beam) providing visibility, optimization, and control across AWS, Azure, GCP, and Nutanix private cloud; claims 35%+ savings through automated rightsizing, reserved instance purchasing, and showback/chargeback .

- **[Turbonomic (IBM)](https://www.ibm.com/)**  
  Application Resource Management platform that continuously analyzes and automates resource allocation across on-premises and cloud environments; 8.19 adds AWS Aurora DB cluster parking, expanded Azure region and VM instance support, and billed cost discovery for Azure VM Scale Sets .

- **[Scalr](https://scalr.io/)**  
  Terraform/OpenTofu automation and collaboration platform positioned as a cost-effective drop-in replacement for Terraform Cloud; provides remote operations backend, GitOps workflows, OPA policy enforcement, drift detection, and AI tooling including an MCP Server for querying workspaces from AI assistants .

- **[CloudBolt](https://www.cloudbolt.io/)**  
  Hybrid cloud management platform with a May 2026 release adding MCP support for governed AI agent interaction, fine-grained RBAC, custom day-two actions, and expanded VMware alternative support (OpenShift Virtualization, Oracle Linux Virtualization Manager, Hyper-V, OCI, Azure Local) .

## Open-Source GitHub Projects

- **[OptScale](https://github.com/hystax/optscale)**  
  Open-source multi-cloud FinOps platform (Apache 2.0) with support for AI/ML-heavy workloads where GPU and experimentation costs can spike; ingests billing and usage data from cloud APIs, combining cost visibility, optimization recommendations, budget tracking, anomaly detection, and policy-based alerts aligned to teams or business structures; Thoughtworks notes it covers broader non-Kubernetes FinOps use cases than OpenCost with less vendor lock-in than Cloudability/CloudHealth, though deployment complexity is higher .

- **[Terrakube](https://github.com/terrakube-io/terrakube)**  
  Open-source collaboration platform for remote Infrastructure-as-Code operations using Terraform or OpenTofu (Apache 2.0); positioned as a complete replacement for Terraform Enterprise, Scalr, or Env0; features private Terraform module and provider registries, organization-based workspace management, VCS integration (GitHub, GitLab, Azure DevOps, Bitbucket), custom flows with approvals, and plugin support; deployable on Kubernetes .

- **[Fulcrum Core](https://github.com/fulcrumproject/core)**  
  Comprehensive open-source cloud infrastructure management system (Go) designed to orchestrate and monitor distributed cloud resources across multiple providers; serves as a centralized control plane for managing cloud service providers, deployed agents, and provisioned services (VMs, containers, Kubernetes clusters); supported by CISPE.cloud for open, sovereign, and interoperable cloud solutions in Europe; active development with Docker Compose deployment .

### Additional Strong Open-Source Options

- **OpenCost** — Open-source Kubernetes cost monitoring tool; provides real-time cost visibility for container workloads, useful as a complement to broader FinOps platforms.
- **Infracost** — Open-source cloud cost estimator for pull requests; shows cost impact of infrastructure changes before merge, integrating FinOps into IaC workflows .
- **Terracost** — European open-source cloud cost estimation tool (France, score 94/100 in EU sovereignty ranking); self-hostable for cost estimation of Terraform plans .
- **kube-green** — Open-source tool (Italy) for automatically shutting down idle Kubernetes resources outside business hours to reduce cloud costs .
- **BoaviztAPI** — Open-source API (France) for assessing the environmental impact of cloud resources; useful for sustainability-aware cloud management .

**Frameworks for building custom systems**: Combine **OptScale** for multi-cloud FinOps with GPU/ML workload cost visibility, **Terrakube** for self-hosted Terraform/OpenTofu operations with policy enforcement, **Fulcrum Core** for distributed cloud resource orchestration, and **Infracost** for shift-left cost visibility in IaC pipelines in a fully self-hosted cloud management stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cloud management platforms handling infrastructure credentials and cost data must comply with applicable security policies and financial governance requirements; access to cloud provisioning capabilities requires strict RBAC and audit trails.
- Self-hosted open-source solutions vary significantly in scope—OptScale provides broad FinOps coverage, Terrakube focuses on IaC operations, and Fulcrum Core targets distributed resource orchestration; full enterprise CMP with provisioning, governance, and multi-cloud orchestration typically requires commercial platforms or assembly of multiple tools.
- Verify license terms for commercial use; OptScale uses Apache 2.0, Terrakube uses Apache 2.0, and Fulcrum Core is under active development (check repository for license) .

---

**Made for cloud platform engineers, FinOps practitioners, infrastructure architects, and IT operations leaders.**  
Let's make cloud management more open, cost-aware, and operationally sovereign.
