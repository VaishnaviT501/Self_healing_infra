# 🛠️ Self-Healing Infrastructure with Prometheus, Alertmanager & Ansible

This project demonstrates a **self-healing infrastructure** setup using **Nginx, Prometheus, Node Exporter, Alertmanager, Webhooks, and Ansible**.  
When Nginx or system resources go down, Prometheus detects the issue, triggers an alert via Alertmanager, and automatically remediates it using Ansible.

---

## 🚀 Features
- **Monitoring**
  - Nginx health monitoring using `/stub_status`
  - System-level metrics via Node Exporter
- **Alerting**
  - Prometheus rules for:
    - `NginxDown`
    - `HighCPUUsage`
  - Alerts routed through Alertmanager
- **Self-Healing**
  - Alerts trigger a **Webhook**
  - Ansible playbooks restart failed services automatically
- **Automation**
  - Complete infrastructure orchestrated using **Docker Compose**

---

## 📊 Alerts Implemented

NginxDown – Fires when Nginx is unreachable

HighCPUUsage – Fires when CPU load exceeds threshold

---

## 📸 Screenshots


