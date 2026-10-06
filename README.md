# 🛠️ IT Service Desk Analytics

An IT service desk analytics project that uses **PostgreSQL**, **SQL**, and **Power BI** to analyze support ticket activity, SLA performance, resolution times, agent workload, and service trends.

---

## 📌 Project Overview

The goal of this project is to analyze an IT service desk dataset and turn raw ticket data into useful operational insights.

The project follows an end-to-end analytics workflow:

```
CSV Data → PostgreSQL → SQL Analysis → Power BI → Business Insights
```

The analysis focuses on questions such as:

- How many tickets are being created?
- Which priorities generate the most support requests?
- Which categories have the highest ticket volume?
- How long does it take to resolve tickets?
- How often are resolution SLAs breached?
- How are tickets distributed across support agents?
- Which merchants generate the most support requests?

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **PostgreSQL** | Data storage and querying |
| **pgAdmin 4** | Database management |
| **SQL** | Data analysis and transformation |
| **Power BI** | Data visualization and dashboard development |
| **Power Query** | Data preparation |
| **DAX** | KPI and dashboard calculations |
| **Git/GitHub** | Project version control |

---

## 🗂️ Dataset

The dataset contains IT service/support ticket information along with agent and merchant information.

### Main Tables

**Tickets**
- Ticket ID
- Merchant ID
- Category
- Sub-category
- Priority
- Created date
- First response time
- Resolution time
- Response SLA status
- Resolution SLA status
- Reopened status
- CSAT score

**Agents**
- Agent ID
- Agent name
- Support tier
- Primary category
- Shift region
- Efficiency multiplier

**Merchants**
- Merchant ID
- Merchant name
- Sector
- Merchant tier
- Region

---

## 🔍 SQL Analysis

The SQL analysis is organized into practical questions that become progressively more advanced.

### Analysis Covered

- Ticket volume by priority
- Ticket volume by category
- Average resolution time by priority
- Resolution SLA breach analysis
- Tickets handled by each agent
- Average resolution time by category
- Monthly ticket volume
- Top merchants by ticket volume
- Ranking categories within each priority
- Tickets requiring further investigation

### SQL Features Used

- `GROUP BY`
- Aggregate functions
- `JOIN`
- `WHERE`
- `FILTER`
- `DATE_TRUNC`
- CTEs
- Window functions

---

## 📊 Power BI Dashboard

The Power BI dashboard provides an overview of service desk performance and lets users investigate operational trends.

### Dashboard Pages

#### 1. Executive Overview
- Total tickets
- Open tickets
- SLA performance
- Average resolution time
- Ticket trends
- Priority distribution
- Category distribution

#### 2. SLA & Resolution
- Response SLA performance
- Resolution SLA performance
- SLA breaches by priority
- Resolution time by category
- Monthly SLA trends

#### 3. Agent Performance
- Tickets handled by agent
- Average resolution time
- Average response time
- SLA performance
- Reopened tickets

#### 4. Merchant Analysis
- Tickets by merchant
- Tickets by sector
- Tickets by region
- Top support categories
- High-volume merchants
- Reopened tickets

---

## 💡 Key Business Questions

The analysis is intended to help answer operational questions such as:

- Where is the service desk experiencing the most demand?
- Which ticket priorities take the longest to resolve?
- Which categories contribute most to SLA breaches?
- Are some agents handling significantly more tickets than others?
- Which merchants generate the highest support volume?
- Are there recurring areas that may require process improvements?

---

## 📁 Suggested Repository Structure

```
it-service-desk-analytics/
│
├── data/                 # Raw CSV files
├── sql/                  # SQL scripts (schema, analysis queries)
├── powerbi/              # Power BI (.pbix) file
├── screenshots/          # Dashboard screenshots
└── README.md
```

---

## 🚀 How to Run

1. Create a PostgreSQL database and import the CSV files into the tables using pgAdmin 4.
2. Run the scripts in the `sql/` folder to reproduce the analysis.
3. Open the `.pbix` file in Power BI Desktop and connect it to your PostgreSQL database (or refresh the data source).
4. Explore the dashboard pages.

---

## 👤 Author

**Your Name**
[LinkedIn](https://linkedin.com/in/your-profile) | [GitHub](https://github.com/your-username)

A few things to customize before publishing:

Replace the Author section with your name and links.
Add dashboard screenshots to a screenshots/ folder and embed them with ![Executive Overview](screenshots/executive-overview.png).
Adjust the repository structure and "How to Run" steps if your folder names differ.

i will add csv files as well agents.csv , merchants.csv, tickets.csv , i imported dataset wrote queries

Updating the README to cover the new CSV imports.

Here's the updated README with your three CSV files and the SQL queries included. Copy everything inside the block:

markdown
# 🛠️ IT Service Desk Analytics

An IT service desk analytics project that uses **PostgreSQL**, **SQL**, and **Power BI** to analyze support ticket activity, SLA performance, resolution times, agent workload, and service trends.

---

## 📌 Project Overview

The goal of this project is to analyze an IT service desk dataset and turn raw ticket data into useful operational insights.

The project follows an end-to-end analytics workflow:

```
CSV Data → PostgreSQL → SQL Analysis → Power BI → Business Insights
```

The analysis focuses on questions such as:

- How many tickets are being created?
- Which priorities generate the most support requests?
- Which categories have the highest ticket volume?
- How long does it take to resolve tickets?
- How often are resolution SLAs breached?
- How are tickets distributed across support agents?
- Which merchants generate the most support requests?

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **PostgreSQL** | Data storage and querying |
| **pgAdmin 4** | Database management and CSV import |
| **SQL** | Data analysis and transformation |
| **Power BI** | Data visualization and dashboard development |
| **Power Query** | Data preparation |
| **DAX** | KPI and dashboard calculations |
| **Git/GitHub** | Project version control |

---

## 🗂️ Dataset

The dataset consists of three CSV files, included in the `data/` folder:

| File | Description |
|------|-------------|
| `tickets.csv` | Support ticket records |
| `agents.csv` | Support agent details |
| `merchants.csv` | Merchant/customer details |

### Tables

**Tickets** (`tickets.csv`)
- Ticket ID
- Merchant ID
- Category
- Sub-category
- Priority
- Created date
- First response time
- Resolution time
- Response SLA status
- Resolution SLA status
- Reopened status
- CSAT score

**Agents** (`agents.csv`)
- Agent ID
- Agent name
- Support tier
- Primary category
- Shift region
- Efficiency multiplier

**Merchants** (`merchants.csv`)
- Merchant ID
- Merchant name
- Sector
- Merchant tier
- Region

---

## 🔍 SQL Analysis

The CSV files were imported into PostgreSQL using pgAdmin 4. The SQL queries are organized into practical questions that become progressively more advanced, and are available in the `sql/` folder.

### Analysis Covered

- Ticket volume by priority
- Ticket volume by category
- Average resolution time by priority
- Resolution SLA breach analysis
- Tickets handled by each agent
- Average resolution time by category
- Monthly ticket volume
- Top merchants by ticket volume
- Ranking categories within each priority
- Tickets requiring further investigation

### SQL Features Used

- `GROUP BY`
- Aggregate functions
- `JOIN`
- `WHERE`
- `FILTER`
- `DATE_TRUNC`
- CTEs
- Window functions

---

## 📊 Power BI Dashboard

The Power BI dashboard provides an overview of service desk performance and lets users investigate operational trends.

### Dashboard Pages

#### 1. Executive Overview
- Total tickets
- Open tickets
- SLA performance
- Average resolution time
- Ticket trends
- Priority distribution
- Category distribution

#### 2. SLA & Resolution
- Response SLA performance
- Resolution SLA performance
- SLA breaches by priority
- Resolution time by category
- Monthly SLA trends

#### 3. Agent Performance
- Tickets handled by agent
- Average resolution time
- Average response time
- SLA performance
- Reopened tickets

#### 4. Merchant Analysis
- Tickets by merchant
- Tickets by sector
- Tickets by region
- Top support categories
- High-volume merchants
- Reopened tickets

---

## 💡 Key Business Questions

The analysis is intended to help answer operational questions such as:

- Where is the service desk experiencing the most demand?
- Which ticket priorities take the longest to resolve?
- Which categories contribute most to SLA breaches?
- Are some agents handling significantly more tickets than others?
- Which merchants generate the highest support volume?
- Are there recurring areas that may require process improvements?

---
