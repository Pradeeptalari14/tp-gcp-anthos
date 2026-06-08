# GCP Anthos Service Mesh Studio

This repository contains the target configuration and SRE runtime files compiled by the **GCP Anthos Service Mesh Studio** dashboard module.

## 🚀 Description
Orchestrate multi-cluster service mesh across hybrid clouds. Generate mesh configs, mTLS egress/ingress rules, and telemetry log dashboards configurations.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/deploy/asm/asm_policy.yaml`
- **Execution Command**: `kubectl apply -f asm_policy.yaml`
- **Validation Command**: `kubectl get peerauthentication`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-gcp-anthos.git
   cd tp-gcp-anthos
   ```

2. **Run Execution Target:**
   ```bash
   kubectl apply -f asm_policy.yaml
   ```

3. **Verify Runtime Stability:**
   ```bash
   kubectl get peerauthentication
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
