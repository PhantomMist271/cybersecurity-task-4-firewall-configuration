
# 🔥 Windows Firewall Configuration – Cybersecurity Internship Task 4

## 🎯 Task Objective
Understand how a firewall filters traffic, create and manage rules, and simulate real-world use cases by blocking a common insecure port.

---

## 💻 System Used
- **Operating System:** Windows 10
- **Tool:** Windows Defender Firewall with Advanced Security

---

## 🔧 Task Performed

### ✅ Step 1: Viewed Existing Inbound Rules
Accessed the firewall and reviewed current inbound rules.
- 📸 Screenshot: `firewall_rules_list.png`

### ✅ Step 2: Created New Rule to Block Port 23 (Telnet)
Telnet uses port 23 and is known for being insecure. Blocking this port is a standard security practice.

- Created a new **Inbound Rule** using the following settings:
  - **Rule Type:** Port
  - **Protocol:** TCP
  - **Port Number:** 23
  - **Action:** Block the connection
  - **Profiles:** Domain, Private, Public
  - **Name:** `Block Telnet Port 23`
  - **Description:** This rule blocks inbound traffic to port 23 (Telnet) for better security.

- 📸 Screenshot: `block_port_23_rule_creation.png`
- 📸 Screenshot: `block_port_23_rule_added.png`

---

## 🧠 Key Learnings

- Windows Firewall allows fine-grained control over network traffic.
- Blocking known vulnerable ports helps prevent unauthorized access.
- Port 23 (Telnet) is outdated and should always be disabled.
- Creating and removing firewall rules is simple through the Windows GUI.

---

## 📁 Repository Structure

```
cybersecurity-task-4-firewall-configuration/
│
├── README.md
└── screenshots/
    ├── firewall_rules_list.png
    ├── block_port_23_rule_creation.png
    ├── block_port_23_rule_added.png
    
```

---
*This task demonstrates how firewalls can be configured to secure a system from vulnerable or outdated protocols like Telnet.*
.
