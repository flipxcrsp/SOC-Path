# 🛡️ Wazuh SIEM Labs – Search Expressions & Event Correlation

This section contains hands-on labs using the **Wazuh SIEM** interface to analyze Windows security logs, filter events using Lucene syntax, and correlate real-time alerts with MITRE ATT&CK TTPs.

---

## 📊 Wazuh Main Dashboard

Explore event levels, MITRE correlations, and alert timelines.

![Main Dashboard](wazuh_main_dashboard.png)

---

## 🔍 Using Lucene Filters for Precision Search

Filtering specific logs using `rule.description`, `manager.name`, `eventID`, and usernames with DQL syntax.

![User Creation Filter](wazuh_event_filter_user_created_t1098.png)

---

## 📎 MITRE Technique T1098 - User Account Creation

Wazuh detected the creation of the `Pikachu` account and mapped it to MITRE ATT&CK T1098 (Persistence).

![Pikachu Event](wazuh_pikachu_event_details_t1098.png)

---

## 📄 Correlating Alerts & Viewing Event Details

In-depth alert breakdown including rule IDs, agent info, and timestamps.

![Event Detail](wazuh_event_apparmor_denied_details.png)

---

## ✅ SIEM Challenge Completion

Completed challenge by identifying correct users, filters, and answering correlation questions in Wazuh.

![Challenge Result](wazuh_challenge_results.png)

---

## 🔗 Other Notable Screens

- [ ] `wazuh_interface_breakdown.png`
- [ ] `wazuh_data_visualization.png`
- [ ] `wazuh_events_sorting_multiple_alerts.png`
- [ ] `wazuh_filter_rule_5710.png`
- [ ] `wazuh_elastic_modules_view.png`

---

### 📚 Skills Practiced

- SIEM log correlation
- Lucene/DQL search syntax
- Event Viewer + Wazuh side-by-side analysis
- MITRE ATT&CK mapping
- Real-world alert triage & filtering

---
