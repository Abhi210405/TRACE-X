# TRACE-X

### Transaction Risk Analysis & Circular Evidence Explorer

> **One transaction may look normal. The pattern tells the truth.**

TRACE-X is an **AI-inspired financial crime intelligence prototype** designed to demonstrate how suspicious transaction networks can be identified, visualized, scored, explained, and investigated.

Instead of looking at transactions individually, TRACE-X focuses on the **relationships and patterns between accounts** to uncover potentially suspicious financial activity.

---

## 🚨 Problem Statement

Financial crime is often not visible in a single transaction.

Suspicious activity can be distributed across multiple accounts through:

* Small and repeated transfers
* Rapid movement of funds
* Circular money flows
* Layered transactions
* Connected account networks
* Fan-in and fan-out transaction structures
* Repeated movement between accounts

Traditional transaction monitoring systems can generate large numbers of alerts while providing limited context for investigators.

**TRACE-X approaches the problem from a network perspective.**

---

## 💡 Our Solution

TRACE-X transforms transaction data into a connected network and analyzes it for suspicious behavioral patterns.

### Core Flow

```text
Transaction Data
       ↓
Data Processing
       ↓
Transaction Network
       ↓
Pattern Detection
       ↓
Risk Analysis
       ↓
Explainable Alert
       ↓
Human Investigation
```

The platform is designed to help investigators move from:

**"This transaction looks suspicious."**

to:

**"This network shows a suspicious pattern, and here is the evidence explaining why."**

---

## ✨ Key Features

### 📊 Investigator Dashboard

Provides a high-level view of:

* Total transactions
* Connected accounts
* Suspicious networks
* High-risk cases
* Detected patterns

---

### 📁 Transaction Data Ingestion

TRACE-X supports:

* Synthetic demo transaction data
* CSV transaction upload
* Transaction table visualization
* Basic client-side data processing

Example transaction structure:

```text
Transaction ID
Sender
Receiver
Amount
Timestamp
```

---

### 🕸️ Transaction Network Visualization

Transactions are represented as relationships between accounts.

Example:

```text
A → B → C → D → E
↑               ↓
└───────────────┘
```

This makes hidden relationships and suspicious movement easier to understand.

---

### 🔍 Pattern Detection

TRACE-X demonstrates detection of multiple suspicious network patterns:

| Pattern            | Description                                                   |
| ------------------ | ------------------------------------------------------------- |
| Circular Flow      | Funds move through multiple accounts and return to the origin |
| Layering           | Funds move through several intermediary accounts              |
| Fan-In             | Multiple accounts send funds to a common account              |
| Fan-Out            | One account distributes funds to multiple accounts            |
| Rapid Transfer     | Funds move between accounts within short time intervals       |
| Connected Accounts | Multiple accounts form a suspicious transaction cluster       |

---

### 🎯 Risk Scoring

Detected patterns are assigned a risk score from:

**0 → 100**

Example:

```text
91 / 100
HIGH RISK
```

Risk levels:

```text
0–39    LOW
40–69   MEDIUM
70–100  HIGH
```

The score is intended to help investigators prioritize cases.

---

### 🧠 Explainable Alerts

Instead of showing only a risk score, TRACE-X provides evidence explaining why a network was flagged.

Example:

```text
Risk Score: 91/100

Alert:
Circular + Layered Fund Flow

Evidence:
✓ 5 connected accounts
✓ Repeated movement
✓ Circular transaction path
✓ Similar transaction amounts
✓ Short transaction intervals
✓ Unusual network structure
```

This supports a **human-in-the-loop investigation workflow**.

---

### 🕵️ Investigation Workspace

Investigators can inspect:

* Suspicious transaction networks
* Detected patterns
* Risk scores
* Evidence
* Transaction timeline
* Investigation notes
* Case status

---

## 🧪 Synthetic Demo

TRACE-X includes synthetic transaction scenarios for demonstration purposes.

One example is:

```text
A → B → C → D → E → A
```

This creates a circular transaction network that can be identified by the prototype.

### Demo Flow

```text
1. Open Dashboard
        ↓
2. Load Demo Data
        ↓
3. Analyze Transactions
        ↓
4. Detect Suspicious Patterns
        ↓
5. Generate Risk Scores
        ↓
6. Review Explainable Alert
        ↓
7. Open Investigation
```

---

## 🖥️ Prototype Screens

The prototype includes:

* Login
* Investigator Dashboard
* Transaction Management
* Network Visualization
* Pattern Detection
* Risk Alerts
* Investigation Workspace
* Evidence Timeline
* Investigator Notes

---

## 🛠️ Technology Stack

The current prototype is intentionally lightweight and runs entirely in the browser.

### Frontend

* HTML5
* CSS3
* Vanilla JavaScript

### Data Processing

* JavaScript-based transaction processing
* Synthetic transaction datasets
* Client-side CSV parsing

### Visualization

* Custom HTML/CSS/JavaScript network visualization
* Interactive transaction and investigation views

### Current Architecture

```text
┌──────────────────────────────┐
│        TRACE-X UI            │
│                              │
│ HTML + CSS + JavaScript      │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│ Client-Side Data Processing  │
│                              │
│ Transactions + Pattern Logic │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│ Network & Risk Analysis      │
│                              │
│ Pattern Detection            │
│ Risk Scoring                 │
│ Explainable Alerts           │
└──────────────────────────────┘
```

---

## 📂 Project Structure

The current prototype is a single-file application:

```text
TRACE-X/
│
├── index.html
└── README.md
```

All CSS and JavaScript required by the prototype are contained inside:

```text
index.html
```

Therefore, no package installation or backend setup is required.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/TRACE-X.git
```

### 2. Open the Project

```bash
cd TRACE-X
```

### 3. Run the Prototype

Simply open:

```text
index.html
```

in a modern web browser.

No:

* Node.js
* npm
* Python
* Database
* Backend server

is required for the current prototype.

---

## 🔐 Demo Login

Use the following credentials for the prototype:

```text
Email:
investigator@trace-x.demo

Password:
TraceX@123
```

> These credentials are for the local demonstration prototype only.

---

## 🎬 Recommended Hackathon Demo

For the best live demonstration, use this sequence:

### Step 1 — Dashboard

Start with the investigator dashboard and explain the overall situation.

### Step 2 — Load Demo Data

Load the synthetic transaction dataset.

### Step 3 — Show the Network

Display how individual transactions form a connected network.

### Step 4 — Detect Patterns

Show patterns such as:

```text
Circular Flow
Layering
Fan-In
Fan-Out
Rapid Transfer
```

### Step 5 — Risk Score

Highlight the highest-risk network.

Example:

```text
91 / 100
HIGH RISK
```

### Step 6 — Explain the Alert

Show the evidence behind the score.

### Step 7 — Investigation

Open the investigation workspace and demonstrate:

* Network evidence
* Timeline
* Notes
* Case status

---

## 🏦 Target Users

TRACE-X is designed as a conceptual solution for:

* Banks
* FinTech companies
* Payment platforms
* Risk & compliance teams
* Financial crime investigators

---

## 🎯 Benefits

TRACE-X aims to provide:

### Network Visibility

Understand relationships between accounts instead of viewing transactions in isolation.

### Faster Investigation

Help investigators focus on high-risk networks first.

### Better Alert Prioritization

Use risk scoring to identify potentially important cases.

### Explainable Detection

Show evidence supporting why a network was flagged.

### Human-in-the-Loop Analysis

The system supports investigators rather than replacing human judgment.

---

## 🔮 Future Roadmap

The current version is a hackathon prototype. Future versions can extend the architecture with:

### Real-Time Transaction Monitoring

```text
Live Transaction Stream
        ↓
Real-Time Graph
        ↓
Continuous Analysis
        ↓
Instant Risk Alert
```

### Advanced Graph Analytics

Use large-scale graph processing to analyze millions of connected accounts and transactions.

### Machine Learning

Future versions can integrate:

* Anomaly detection
* Behavioral profiling
* Graph-based machine learning
* Graph Neural Networks
* Adaptive risk models

### Cross-Network Intelligence

Connect transaction networks across multiple platforms and financial institutions.

### Automated Investigation Workflows

Future versions could support:

* Case assignment
* Evidence collection
* Investigation workflow
* Investigator collaboration
* Case reporting

---

## ⚠️ Prototype Disclaimer

TRACE-X is a **hackathon demonstration prototype** using synthetic/demo transaction data.

It is not intended to:

* Determine whether a person has committed financial crime
* Replace compliance professionals
* Make autonomous enforcement decisions
* Provide legal conclusions
* Process real financial accounts

Risk scores and alerts shown by the prototype are demonstrative.

---

## 🧩 Vision

Financial crime is rarely about one transaction.

It is about the **network behind the transactions**.

TRACE-X aims to make those hidden relationships visible by combining:

```text
Transaction Data
       +
Network Analysis
       +
Pattern Detection
       +
Risk Scoring
       +
Explainable Evidence
       +
Human Investigation
```

### TRACE-X

> **One transaction may look normal. The pattern tells the truth.**

---

## 👥 Team

### TRACE-X Team

* **Lovekush Goyal**
* **Abhinandan Pandey**
* **Om Aditya**
* **Ruchi Yadav**

---

## ⭐ Project Status

```text
Prototype Status: Hackathon Demo Ready

Frontend:        ✅
Dashboard:       ✅
Transaction Data: ✅
CSV Upload:      ✅
Network View:    ✅
Pattern Detection: ✅
Risk Scoring:    ✅
Explainable Alerts: ✅
Investigation View: ✅
Synthetic Demo:  ✅
```

---

## 📜 License

This project is intended for educational, research, and hackathon demonstration purposes.
