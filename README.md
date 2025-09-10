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


<img width="1919" height="966" alt="Screenshot 2025-08-25 212810" src="https://github.com/user-attachments/assets/9d771e5c-712f-45bc-9fa4-d4b1cc4b8690" />
<img width="1919" height="962" alt="Screenshot 2025-08-25 212759" src="https://github.com/user-attachments/assets/7f999ea4-cf10-4dd7-8138-714942c5f8ff" />
<img width="1919" height="974" alt="Screenshot 2025-08-25 212750" src="https://github.com/user-attachments/assets/5c8f06cd-aae1-4806-ac51-ab2325f1a4dc" />
<img width="1916" height="968" alt="Screenshot 2025-08-25 212649" src="https://github.com/user-attachments/assets/bb5bed15-d329-480d-ad12-24fb2d0468e1" />
<img width="1919" height="961" alt="Screenshot 2025-08-25 212634" src="https://github.com/user-attachments/assets/d6abc17b-762d-4583-8476-d726138937ed" />
<img width="1920" height="1020" alt="Screenshot 2025-08-25 210620" src="https://github.com/user-attachments/assets/479a5176-142e-4d16-a075-d9f294ee4a3c" />
<img width="1920" height="1020" alt="Screenshot 2025-08-25 210602" src="https://github.com/user-attachments/assets/14bd5db9-a1ff-453f-89e3-68c540cb9031" />
<img width="1920" height="1020" alt="Screenshot 2025-08-25 210535" src="https://github.com/user-attachments/assets/8c14778f-88fb-4ded-a52d-3d4902aaf476" />
<img width="1920" height="1020" alt="Screenshot 2025-08-25 210504" src="https://github.com/user-attachments/assets/970a6224-510f-4139-9656-9d9ba5a3daca" />
<img width="1919" height="1019" alt="Screenshot 2025-08-26 004253" src="https://github.com/user-attachments/assets/be8be279-2a43-4ef6-b1e4-31b8c2696dff" />
<img width="1919" height="1022" alt="Screenshot 2025-08-26 003934" src="https://github.com/user-attachments/assets/01eeab3c-cb06-41d3-adb5-efc499c13e04" />
<img width="1917" height="997" alt="Screenshot 2025-08-26 001056" src="https://github.com/user-attachments/assets/c302ebc8-4612-40f1-9863-597e616d4587" />
<img width="1916" height="967" alt="Screenshot 2025-08-26 000127" src="https://github.com/user-attachments/assets/8873a629-32b1-4535-b3a9-966bbc50cb5c" />
<img width="1917" height="971" alt="Screenshot 2025-08-26 000115" src="https://github.com/user-attachments/assets/f2ef78b0-f773-4ad7-89b0-5a199cb1494c" />
<img width="1914" height="964" alt="Screenshot 2025-08-26 000057" src="https://github.com/user-attachments/assets/5f3128e1-3a50-4553-aa4c-1ba6df2e8044" />
<img width="1917" height="1017" alt="Screenshot 2025-08-25 232850" src="https://github.com/user-attachments/assets/ec4af933-b107-456b-bc02-a6a0c48e63a6" />
<img width="1914" height="956" alt="Screenshot 2025-08-25 232821" src="https://github.com/user-attachments/assets/9fa08f8f-289e-4e7c-befc-aca3d40f2449" />
<img width="1916" height="1018" alt="Screenshot 2025-08-25 232629" src="https://github.com/user-attachments/assets/1782dad9-cb10-45fc-9236-5d218323a255" />
<img width="1919" height="965" alt="Screenshot 2025-08-25 232612" src="https://github.com/user-attachments/assets/6b9eb576-1206-49d0-9220-d2cab00e2f1c" />
<img width="1911" height="971" alt="Screenshot 2025-08-25 220450" src="https://github.com/user-attachments/assets/d216c991-936a-4b7e-a9a2-e0fc5074c52a" />
<img width="1919" height="757" alt="Screenshot 2025-08-25 220437" src="https://github.com/user-attachments/assets/3d2b4dc7-0705-46d2-8b2a-f87f5a9aa24b" />
<img width="1919" height="962" alt="Screenshot 2025-08-25 220424" src="https://github.com/user-attachments/assets/a181a8f7-ad56-48b6-8b79-dd88e5ba3079" />
<img width="1919" height="971" alt="Screenshot 2025-08-25 215843" src="https://github.com/user-attachments/assets/46de82ae-c837-47c8-9f2f-589d8d9b377d" />
<img width="1916" height="959" alt="Screenshot 2025-08-25 214833" src="https://github.com/user-attachments/assets/cad9444c-9c11-4447-9cc2-c3c4c4d25c02" />
<img width="1916" height="968" alt="Screenshot 2025-08-25 214807" src="https://github.com/user-attachments/assets/92965919-74e3-49a2-aa21-4d1865d4bb97" />
<img width="1919" height="961" alt="Screenshot 2025-08-25 214402" src="https://github.com/user-attachments/assets/64c7c8f4-afb2-41b5-b549-84622c730a48" />
<img width="1919" height="962" alt="Screenshot 2025-08-25 213205" src="https://github.com/user-attachments/assets/bfc05e98-7ef9-4e0e-8e06-705c3e0f0dc0" />
<img width="1913" height="970" alt="Screenshot 2025-08-25 212843" src="https://github.com/user-attachments/assets/730155f5-4608-4d52-98b7-3c0baa496f1f" />

