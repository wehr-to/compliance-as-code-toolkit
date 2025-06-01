# 🛡️ compliance-toolkit

This repository contains automation resources for implementing **Compliance as Code** — using Terraform, Ansible, and shell scripts to enforce security benchmarks and regulatory controls such as **CIS**, **NIST 800-53**, and **SOC 2**.

It’s designed to simulate how cloud and infrastructure teams can **build compliance into their provisioning pipelines** instead of relying on manual audits or checklists.

## 🎯 Why This Repo Exists

Security frameworks are only useful if they're enforceable. This project turns compliance into executable infrastructure, aligning technical controls with regulatory standards through automation.

This repo helps you:

- Apply CIS benchmarks to cloud and Linux resources
- Enforce NIST-aligned IAM and logging policies via Terraform
- Harden systems with reusable Ansible roles
- Integrate compliance into CI/CD pipelines

## 🧱 What's Included

| Folder                     | Description |
|----------------------------|-------------|
| `terraform-modules/`       | Infrastructure modules with CIS/NIST-aligned controls (AWS, Azure, GCP) |
| `ansible-playbooks/`       | OS hardening and compliance enforcement (Ubuntu, CentOS, Amazon Linux) |
| `scripts/`                 | Shell scripts for auditing and remediating compliance gaps |
| `controls-mapping/`        | Maps Terraform/Ansible actions to CIS/NIST/SOC 2 controls |
| `ci-cd-integrations/`      | GitHub Actions / GitLab pipelines for compliance checks pre-deploy |
| `audit-output-samples/`    | Output examples from OpenSCAP, Lynis, and AWS Config |
| `docs/`                    | Compliance checklists, references, and reporting templates |

## 📋 Compliance Frameworks Covered
- CIS Benchmarks (AWS, Linux, Azure)
- NIST 800-53 (access control, auditing, baseline hardening)
- SOC 2 Security Trust Principles
- HIPAA-inspired logging and access constraints

Each module or playbook includes a control-mapping.md file explaining what standards it enforces.

## 🚀 CI/CD Integrations
- terraform-fmt and tfsec runs in pre-commit hooks
- Ansible playbook dry-run before deploy
- OpenSCAP or custom shell check after cloud resource creation

## 👥 Who Should Use This
- Cloud and security engineers responsible for compliance posture
- Blue teamers aligning policy with cloud or Linux enforcement
- Security architects evaluating “compliance as code” maturity
- Students and job seekers looking to prove practical GRC automation skills

