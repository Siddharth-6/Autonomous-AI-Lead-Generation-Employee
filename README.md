# Autonomous-AI-Lead-Generation-Employee

An autonomous multi-agent lead generation system built using **MachinaOS** that continuously discovers, qualifies, prioritizes, and nurtures high-intent business leads from Reddit.

The system automatically monitors Reddit communities, identifies founders and business owners seeking automation solutions, evaluates whether **Zeenie AI Employees** can solve their problems, generates personalized outreach messages, and delivers actionable sales intelligence reports to the executive team.

---

## 🚀 Features

* Automated Reddit lead discovery
* Multi-agent orchestration
* Lead qualification & scoring
* Zeenie solution recommendation
* Personalized outreach generation
* Lead deduplication & storage
* Telegram notifications
* Daily scheduled execution
* Executive sales intelligence reports

---

## 🏗️ Workflow Architecture

```text
Cron Scheduler (9:00 AM Daily)
            │
            ▼
   Lead Generation Manager
            │
    ┌───────┼────────┐
    ▼       ▼        ▼
Reddit   Lead     Outreach
Hunter   Analyst   Writer
    │       │        │
    └───────┴────────┘
            │
            ▼
    Executive Report
            │
     ┌──────┴──────┐
     ▼             ▼
Lead Storage   Telegram Alert
```

---

## 🤖 Agents

### 1. Reddit Hunter

Responsible for discovering potential opportunities from Reddit.

#### Tasks

* Monitor relevant subreddits
* Find recent posts (last 7 days)
* Identify automation-related discussions
* Return structured lead data

#### Output

```json
{
  "title": "",
  "url": "",
  "subreddit": "",
  "author": "",
  "summary": ""
}
```

---

### 2. Lead Analyst

Responsible for evaluating and qualifying discovered leads.

#### Tasks

* Identify pain points
* Understand business context
* Measure buying intent
* Calculate lead scores
* Determine automation fit
* Recommend Zeenie solutions

#### Lead Scoring

| Metric                 | Weight |
| ---------------------- | ------ |
| Buying Intent          | 40     |
| Pain Severity          | 25     |
| Automation Fit         | 20     |
| Engagement & Freshness | 15     |

#### Priority Levels

| Score    | Priority |
| -------- | -------- |
| 90 - 100 | Critical |
| 80 - 89  | High     |
| 60 - 79  | Medium   |
| < 60     | Low      |

---

### 3. Outreach Writer

Responsible for generating personalized outreach messages.

#### Tasks

* Reference Reddit discussions
* Understand prospect pain points
* Explain why Zeenie fits
* Generate personalized CTAs

#### Output

* Personalized Opening Line
* Outreach Message
* Why Zeenie Fits
* Call To Action

---

### 4. Lead Generation Manager

Responsible for coordinating the entire workflow.

#### Workflow

1. Request opportunities from Reddit Hunter
2. Send candidate leads to Lead Analyst
3. Send qualified leads to Outreach Writer
4. Collect outputs from all agents
5. Generate executive report
6. Store qualified leads
7. Send Telegram notification

---

## 📊 Example Output

The system generates:

* Executive summaries
* Lead priority matrices
* Detailed lead analysis
* Zeenie solution recommendations
* Personalized outreach messages
* Action items for the sales team

Example report sections:

```text
Executive Summary

Lead Priority Matrix

Detailed Lead Analysis

Outreach Recommendations

Action Items
```

---

## 💾 Lead Storage

Qualified leads are stored in:

```text
data/leads.json
```

Stored fields:

* Date
* Title
* URL
* Subreddit
* Lead Score
* Pain Point
* Recommended Zeenie Solution

Duplicate leads are automatically ignored.

---

## ⏰ Automation

The workflow runs automatically every day at:

```text
09:00 AM
```

using the built-in Cron Scheduler.

Manual execution is also supported through the chat trigger.

---

## 📲 Notifications

After each execution:

* Executive report is generated
* High-priority opportunities are summarized
* Results are delivered through Telegram

This enables the Zeenie team to review opportunities immediately and take action.

---

## 🛠️ Tech Stack

* MachinaOS
* Gemini Flash
* Multi-Agent AI Workflows
* Reddit Data Collection
* Telegram Bot Integration
* JSON Database Storage

---

## 🎯 Use Cases

This system can identify businesses looking for:

* Workflow automation
* CRM automation
* Lead generation automation
* Customer support automation
* Browser automation
* Task automation
* AI employees
* Business process automation

---

## 🔮 Future Improvements

* LinkedIn lead discovery
* CRM integrations
* Automated email outreach
* Lead enrichment
* Analytics dashboard
* Multi-platform lead monitoring

---

## 📸 Workflow

<img width="1231" height="733" alt="Screenshot 2026-06-12 141943" src="https://github.com/user-attachments/assets/7031e45e-a96c-4743-8131-e32996234bfd" />

---

## Author

Built as an autonomous lead generation system for **Zeenie AI Employees**.

