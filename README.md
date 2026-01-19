# Workout Project – Infrastructure (Terraform CDK)

This repository contains **all infrastructure-as-code (IaC)** for the **Workout Project**, implemented using **Terraform CDK (CDKTF)** with **TypeScript**.

The infrastructure is designed to be **scalable, reproducible, and secure**, and supports **commercial white-label deployments**.

---

## 🧱 Technology Stack

- **Terraform CDK (CDKTF)**
- **TypeScript**
- **Terraform**
- Cloud Provider: *AWS* (adaptable)
- Node.js ≥ 18

---

## 📦 Repository Purpose

This repository is responsible for:

- Defining and provisioning cloud infrastructure
- Managing isolated environments (`staging` and `production`)
- Ensuring consistent deployments across customers
- Supporting white-label and multi-tenant use cases

> **Note:** This repository contains *infrastructure only*. Application code lives in separate repositories.

---

## 📁 Project Structure

```text
.
├── cdktf.json
├── package.json
├── tsconfig.json
├── src/
│   ├── main.ts              # CDKTF application entry point
│   ├── stacks/              # Terraform stacks
│   ├── constructs/          # Reusable infrastructure components
│   └── config/              # Environment configuration
├── environments/
│   ├── staging/
│   └── production/
├── scripts/                 # Helper and automation scripts
├── LICENSE
└── README.md
