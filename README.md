## 📌 Smart Query Routing System — n8n + LLM + Sentiment Analysis

This task is an **AI-driven automated query routing workflow** built using **n8n**, designed to streamline how student queries are handled at **Innomatics Research Labs**.
Instead of manually categorizing and forwarding queries, the workflow intelligently analyzes each entry and routes it to the appropriate department automatically.

## 🚀 Task Overview

The system performs the following tasks:

* **Collects student queries** via a Google Form
* Stores all submissions in **Google Sheets**
* Uses **Sentiment Analysis** to determine urgency
* Applies an **LLM classifier** to categorize the query
* Routes the query to the correct department using **Switch/IF logic**
* Sends a **structured email** to the respective HOD automatically


## 🧠 Tech Stack & Nodes Used

* **Google Sheets Node** – Input data source
* **Sentiment Analysis Node** – Urgent vs. Normal detection
* **LLM Node (Basic LLM Chain)** – Department classification
* **Switch / IF Node** – Routing logic
* **Email Node** – Automated email delivery

## 🏢 Supported Departments

Queries are classified into multiple categories, such as:

* Technical Doubts
* WiFi Issues
* LMS / Portal Access
* Certification
* Payment Issues
* Batch Change
* Assignments & Tasks
* Placement
* Room Allocation
* Resume Review
  …and more.

Each category is mapped to a department with a corresponding email address.

## 🔄 Workflow Summary

1. **Google Form Submission**
2. **Sheet Trigger Activates Workflow**
3. **Sentiment Evaluated (Urgent/Normal)**
4. **LLM Predicts Category**
5. **Switch Node Selects Department**
6. **Email Sent to Respective HOD**


## 📧 Sample Output Email

```
Subject: Urgent Query – LMS Access (HYD_JNTU)

Name: Vangapandu Lakshmi
Enrollment ID: DS2456
Branch: HYD_JNTU
Sentiment: Urgent
Query: “I can’t access my LMS account since yesterday.”

Please look into this issue at the earliest.
— Automated Query Routing System
```


This automation significantly improves the responsiveness and efficiency of the support workflow by ensuring queries are analyzed correctly and delivered instantly to the right team.

