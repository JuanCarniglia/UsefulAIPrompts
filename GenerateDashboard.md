Act as a Senior Business Intelligence Consultant, not just a Data Analyst. Your goal is not merely to visualize data, but to identify opportunities, risks, anomalies, operational bottlenecks, and actionable recommendations that a business stakeholder might otherwise miss. Challenge assumptions when the data suggests a different conclusion.

The primary audience is Operations Managers with limited technical knowledge. Prioritize business insights over technical details.[Business context explanation]

Create a Dashboard with KPIs on a given data set, on a single HTML page, containing all CSS and JavaScript.

Identify the most relevant KPIs based on the dataset and business context. Do not limit yourself to generic metrics. If a useful KPI cannot be computed from the available data, explicitly explain why.

Separate KPIs into Executive KPIs, Operational KPIs, and Diagnostic KPIs. Place Executive KPIs at the top of the dashboard.

The data source is this csv file : [path to csv file]

This is the data structure:

- [field 1]: [what it means] - [how it needs to be interpreted] - [what are the boundaries] - [how important it is for the analysis]
- …

You need to create a Python script that can be run as many times as possible to update the HTML code.

The generated solution should be easily extensible, allowing new KPIs, filters, charts, and sections to be added with minimal code changes.

The information needs to be displayed in individual KPI cards and sections, arrangeable, resizable.

Add a resizable/collapsible sidebar with the list of KPIs where individual KPIs can be shown/hidden.

Clearly distinguish between measured metrics and AI-generated observations.

Name each KPI with a suitable code (i.e. A1, A2, …. ) for cross referencing

For each KPI include (in a popup section):
* Formula
* Business meaning
* Interpretation
* Desired direction (Higher is Better / Lower is Better)
* Thresholds
* Limitations

Add a small explanatory (collapsible) section on each KPI card to explain briefly what that KPI means.

If data tables are used, add sorting and column resizing.

Add three collapsible sections on top:

- Filtering
    - Multi-select filters on most relevant data points.
    - Add a special filter to exclude data from the overall analysis

- Insights (Findings, Issues, Improvement Areas) (Cross reference with KPIs using the codes)

- Individual cases to highlight (if applies) (Cross reference with KPIs using the codes)Highlight the top 5 cases.Rank findings by business impact (Critical, High, Medium, Low).For every issue detected, explain why it is important and its potential business impact.For each finding, suggest one or more concrete actions.If dates are available, compare with previous periods and highlight increases, decreases, and anomalies.If data enables it, identify outliers using statistical methods and explain why they are unusual.Allow tables to be exported to CSV and charts to PNG.
Where appropriate, set thresholds based on the data domain, and highlight cases where that threshold is crossedClearly indicate missing, inconsistent, or invalid records instead of silently ignoring them.


Must work well on desktop, tablet, and mobile devices.

Include a theme switcher.

Never invent metrics or conclusions. If the data is insufficient, explicitly state that.

Every observation must reference the KPIs or records that support it. Never state conclusions without evidence.

Report duplicate records, missing values, invalid formats, unexpected categories, and suspicious values.

Use LocalStorage to store user preferences
