🎬 Strategic Film Performance Analytics

Operational BI System | Power BI | DAX | Star Schema

🧠 Problem Context

Studios rarely struggle due to a single unsuccessful film. Performance risk accumulates when budget allocation, audience reception, ROI, and awards impact interact over time.

Traditional film dashboards report revenue and ratings in isolation. They fail to explain:

Why certain high-grossing films underperform in profitability

How ratings correlate with financial returns

Where long-term franchise efficiency declines

Whether awards recognition aligns with financial success

This project treats each film as an operational investment event and analyzes performance behavior across decades.

The objective is to move beyond volume metrics and surface structural performance drivers.

🎯 Objectives

This system converts historical film performance data into strategic insights.

Key goals:

Model film data using a star-schema optimized for analysis

Calculate ROI and profitability rather than reporting revenue alone

Track long-term financial efficiency trends

Compare critic vs public reception impact

Enable executive-level slicing without duplicating data

Support investment-style decision evaluation

The focus is on understanding performance mechanics, not just outcomes.

📐 Architecture
Layered BI Architecture

Data Sources → Data Modeling → DAX Metrics → Interactive Dashboard → Executive Insight

This architecture separates responsibilities:

Raw film data (source tables)

Structured analytical model (fact & dimensions)

Business logic (DAX measures)

Insight delivery (dashboard)

Each layer is modular and version-controlled.

📁 Repository Structure
strategic-film-performance-analytics/
│
├── powerbi-project/
│   ├── PixarDashboard.pbip
│   ├── PixarDashboard.Report/
│   └── PixarDashboard.SemanticModel/
│
├── dax-measures/
│   └── key_dax_calculations.md
│
├── screenshots/
│   └── executive_overview.png
│
├── data-dictionary/
│   └── schema_description.md
│
├── Architecture.png
├── .gitignore
└── README.md


Each component is isolated by responsibility, enabling clean version control and extensibility.

🛠 Tech Stack

Power BI Desktop

DAX (Advanced Calculations)

Power Query

Star Schema Data Modeling

Git & GitHub (Project-based version control)

The system is built for analytical clarity, not visual overload.

🔄 Data Model Design

The model implements a clean Star Schema.

📌 Fact Table

Film Performance

Revenue

Budget

ROI

Profit Margin

Ratings

Awards Count

📌 Dimension Tables

Film

Genre

Year

Rating Source

The model avoids snowflaking to maintain filter clarity and DAX simplicity.

⚙️ Analytical Logic
Core Business Calculations

ROI = (Revenue – Budget) / Budget

Profit Margin %

Rolling ROI Trend

Weighted Audience Score

Awards Impact Correlation

Top N Film Ranking

All calculations are centralized within a Measure Table for maintainability.

📊 Executive Dashboard Design

The dashboard is built for decision support, not exploratory clutter.

It answers:

Which films generated high revenue but weak profitability?

Does critical acclaim correlate with ROI?

How has financial efficiency evolved over 30 years?

Which genres sustain strong ROI over time?

Are award-winning films financially superior investments?

The design prioritizes:

Clear KPI cards

Controlled slicers

Navigation buttons

Multi-page executive flow

Minimal but powerful visuals

📈 Insights Delivered

The system reveals:

Revenue alone does not predict ROI

High public ratings do not always correlate with profitability

Certain genres sustain stronger financial consistency

Awards recognition moderately aligns with financial performance

Rolling ROI exposes long-term investment volatility

The analysis reframes performance from “Which film made the most?” to “Which investments were structurally efficient?”

💡 Engineering Discipline

Clean star schema

Centralized business logic

Version-controlled project format (.pbip)

Reproducible analytical structure

No duplicated calculated columns

The system is designed for scalability and clarity.
