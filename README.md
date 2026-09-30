# Missed Classes & Attendance Automation

An **n8n-based automation workflow** that processes lecture attendance data, identifies students who missed classes, sends automated WhatsApp reminders, and generates daily attendance reports.

<img width="770" height="344" alt="image" src="https://github.com/user-attachments/assets/1caefbe5-ef87-4576-bd7e-5861ea7ec301" />


## 🚀 Overview

The workflow automates the process of:

* Fetching attendance and enrollment data
* Identifying students who missed lectures
* Applying reminder eligibility rules
* Sending automated WhatsApp reminders
* Generating batch-wise attendance summaries
* Updating attendance records in Google Sheets

## ⚙️ Workflow

```text
Scheduled Trigger
       ↓
Fetch Attendance & Enrollment Data
       ↓
Process & Match Student Records
       ↓
Identify Absent Students
       ↓
Apply Reminder Rules
       ↓
 ┌───────────────┐
 ↓               ↓
WhatsApp      Attendance
Reminder       Summary
 ↓               ↓
DoubleTick    Google Sheets
```

## 🛠️ Tech Stack

* **n8n** — Workflow automation
* **REST APIs** — Attendance & enrollment data
* **JavaScript** — Business logic and data processing
* **Google Sheets API** — Reporting and record management
* **WhatsApp API / DoubleTick** — Automated notifications

## 🔑 Key Features

### Attendance Processing

Fetches attendance records and matches them with enrolled students and course information.

### Absentee Detection

Uses custom JavaScript logic to identify students who missed specific lectures while handling duplicate records and course eligibility.

### Automated Reminders

Eligible students receive personalized WhatsApp reminders through the DoubleTick API.

### Attendance Reporting

Generates batch-wise and student-level attendance summaries, including attendance percentages.

### Scheduled Execution

The workflow can run automatically on a daily schedule, reducing manual attendance tracking and follow-ups.

## 📁 Workflow File

The repository contains the exported **n8n workflow JSON**, which can be imported into an n8n instance for further configuration.

> **Note:** API keys, tokens, credentials, and other sensitive configuration values should be removed or replaced before sharing the workflow publicly.

## 🎯 Purpose

The project was built to reduce manual effort in **attendance operations, student follow-ups, and daily reporting** by connecting multiple systems through an automated workflow.
