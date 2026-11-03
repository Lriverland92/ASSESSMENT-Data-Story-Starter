Data Story Documentation

Project Title

How Many College Students Actually Graduate?

1. Data Source

Organization: National Center for Education Statistics (NCES)

Dataset: Integrated Postsecondary Education Data System (IPEDS), Graduation Rates

Source: https://nces.ed.gov/ipeds/SummaryTables/report/817

Data period: Reporting years 2015–2024

The project examines six-year bachelor's degree graduation rates at U.S. four-year institutions. The data focuses on first-time, full-time students completing their degrees at their starting institution.

2. Figures and Asset Credits

Figure 1 — Graduation Trends, 2015–2024

File: graduation-trend.svg

Type: Line chart

Data source: NCES IPEDS

Created for this project with AI assistance.

Figure 2 — Graduation Rates, 2015 vs. 2024

File: graduation-comparison.svg

Type: Bar chart

Data source: NCES IPEDS

Created for this project with AI assistance.

Figure 3 — Responsive SVG Comparison

Location: Inline SVG in index.html

Type: Horizontal bar comparison

Data source: NCES IPEDS

Created for this project with AI assistance.

No third-party photographs or illustrations were used.

3. Data Transformations

The graduation rates were taken from the NCES IPEDS summary table.

The original rates were retained to one decimal place.

Two additional columns were calculated for the HTML table:

Change from Previous Year = Current Year's Rate − Previous Year's Rate

Change Since 2015 = Current Year's Rate − 2015 Rate

Changes are expressed in percentage points (pp), not percentage increases.

The graduation rate increased from 59.4% in 2015 to 64.8% in 2024.

64.8 − 59.4 = 5.4 percentage points.

The charts use the reported percentages. The SVG bar lengths were scaled proportionally to the graduation rates.

4. Accessibility and Responsive Design

The webpage includes:

Descriptive alternative text for both external SVG charts.

Visible figure captions and source credits.

A data table with a caption and row and column headers.

A horizontally scrollable table region with keyboard focus.

An inline SVG with an accessible title and description.

Responsive layouts using CSS Grid.

CSS custom properties for consistent colors and spacing.



5. Testing Record

| Test                            | Result         | Evidence                            |
|---------------------------------|----------------|-------------------------------------|
| HTML validation                 | Passed         | W3C: 0 errors                       |
| CSS validation                  | Passed         | W3C: 0 errors                       |
| 320px viewport                  | Passed         | Layout and table scrolling checked  |
| 768px viewport                  | Partial        | Header and introduction checked     |
| 1280px viewport                 | Partial        | Header and figures checked          |
| 200% browser zoom               | Passed         | Text, charts, and table fit         |
| Keyboard table scrolling        | Passed         | Tab and arrow key scrolling         |
| Accessibility tree              | Passed         | Figures, table, and SVG checked     |
| Images disabled                 | Passed         | Alt text and captions visible       |
| Three NCES data values          | Passed         | 2015, 2020, 2024 verified           |

6. AI Assistance Disclosure

I used ChatGPT to help me with the HTML, CSS, SVG graphics, and data table. It also helped me organize the documentation and make the webpage responsive and accessible. I checked the graduation rates using the NCES spreadsheet and tested my webpage with Chrome DevTools and the W3C validators.


Repository URL: https://github.com/Lriverland92/ASSESSMENT-Data-Story-Starter
Github pages: https://lriverland92.github.io/ASSESSMENT-Data-Story-Starter/