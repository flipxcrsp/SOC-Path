# Wazuh SIEM Lab

This directory contains screenshots and notes from my hands-on work with the **Wazuh Security Information and Event Management (SIEM)** platform through Cybrary’s training labs.

## 🔍 Lab Topics Covered

- **Wazuh Interface Overview**
  - Modules: Security Information Management, Auditing, Threat Detection, Regulatory Compliance
- **Security Events Dashboard**
  - Navigating event logs and Lucene-based filtering
  - Sorting and expanding logs for deeper analysis

- **Apache Lucene Syntax**
  - Filtering logs with `key:value`, Boolean logic (AND, OR, NOT)
  - Examples:
    - `rule.description: "User account enabled or created."`
    - `manager.name: ubuntu AND data.win.eventdata.targetUserName: Pikachu`

- **Event Analysis with MITRE ATT&CK**
  - MITRE Technique `T1098`: Persistence via user account creation
  - Associated event logs using Event ID 4720 (Windows account creation)

- **Cross-platform Validation**
  - Viewed and correlated logs in both:
    - **Windows Event Viewer**
    - **Wazuh Web Interface**
  - Confirmed timestamps, usernames, domains, and IPs

- **Custom Filtering**
  - Filtered logs by:
    - Time range (e.g., `Jan 20, 2024 → Jan 23, 2024`)
    - Rule ID, rule.level, manager.name
    - Target usernames: `Hermit`, `Joker`, `Chariot`, `Pikachu`

## 🧠 Skills Practiced

- SIEM navigation and dashboard use
- Lucene/DQL search syntax for log queries
- Log correlation across systems
- MITRE mapping for detection and classification
- Agent service troubleshooting (Wazuh agent restarts, host file updates, IP validation)

## 📂 Related Screenshots

Screenshots inside this folder include:

- Dashboard views (`wazuh_main_dashboard.png`, `wazuh_concepts_overview.png`)
- Filtered search results (`wazuh_event_filter_user_created_t1098.png`)
- Event log deep dives (`wazuh_pikachu_event_details_t1098.png`, `wazuh_mitre_t1098_pikachu_details.png`)
- SIEM filter examples and visualizations

---

### ✅ Summary

This lab helped reinforce SIEM fundamentals while giving hands-on experience working with **Wazuh**, **log queries**, and **threat detection** using real-world security data.

