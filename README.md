An IT service desk analytics project that uses PostgreSQL, SQL, and Power BI to analyze support ticket activity, SLA performance, resolution times, agent workload, and service trends.

Project Overview

The goal of this project is to analyze an IT service desk dataset and turn raw ticket data into useful operational insights.

The project follows an end-to-end analytics workflow:

CSV Data → PostgreSQL → SQL Analysis → Power BI → Business Insights

The analysis focuses on questions such as:

How many tickets are being created?
Which priorities generate the most support requests?
Which categories have the highest ticket volume?
How long does it take to resolve tickets?
How often are resolution SLAs breached?
How are tickets distributed across support agents?
Which merchants generate the most support requests?
Tools & Technologies
PostgreSQL – Data storage and querying
pgAdmin 4 – Database management
SQL – Data analysis and transformation
Power BI – Data visualization and dashboard development
Power Query – Data preparation
DAX – KPI and dashboard calculations
Git/GitHub – Project version control
Dataset

The dataset contains IT service/support ticket information along with agent and merchant information.

Main Tables

Tickets

Ticket ID
Merchant ID
Category
Sub-category
Priority
Created date
First response time
Resolution time
Response SLA status
Resolution SLA status
Reopened status
CSAT score

Agents

Agent ID
Agent name
Support tier
Primary category
Shift region
Efficiency multiplier

Merchants

Merchant ID
Merchant name
Sector
Merchant tier
Region
SQL Analysis

The SQL analysis is organized into practical questions that become progressively more advanced.

Some of the analysis includes:

Ticket volume by priority
Ticket volume by category
Average resolution time by priority
Resolution SLA breach analysis
Tickets handled by each agent
Average resolution time by category
Monthly ticket volume
Top merchants by ticket volume
Ranking categories within each priority
Tickets requiring further investigation

The project uses SQL features including:

GROUP BY
Aggregate functions
JOIN
WHERE
FILTER
DATE_TRUNC
CTE
Window functions
Power BI Dashboard

The Power BI dashboard is designed to provide an overview of service desk performance and allow users to investigate operational trends.

Dashboard Pages

1. Executive Overview

Total tickets
Open tickets
SLA performance
Average resolution time
Ticket trends
Priority distribution
Category distribution

2. SLA & Resolution

Response SLA performance
Resolution SLA performance
SLA breaches by priority
Resolution time by category
Monthly SLA trends

3. Agent Performance

Tickets handled by agent
Average resolution time
Average response time
SLA performance
Reopened tickets

4. Merchant Analysis

Tickets by merchant
Tickets by sector
Tickets by region
Top support categories
High-volume merchants
Reopened tickets
Key Business Questions

The analysis is intended to help answer operational questions such as:

Where is the service desk experiencing the most demand?
Which ticket priorities take the longest to resolve?
Which categories contribute most to SLA breaches?
Are some agents handling significantly more tickets than others?
Which merchants generate the highest support volume?
Are there recurring areas that may require process improvements?
