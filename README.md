<!-- ========================= -->
<!-- TikTok Engagement Analytics -->
<!-- ========================= -->

<h1 align="center">TikTok Engagement Analytics</h1>

<p align="center">
  Data analysis project focused on modelling engagement behaviour and informing content strategy using TikTok analytics data.
</p>

<hr>

<h2>Overview</h2>

<p>
This project analyses TikTok performance data to understand how users interact with content and how engagement translates into growth.
The goal is to convert raw platform metrics into a structured, interpretable model that supports data-driven decision making.
</p>

<ul>
  <li>Defines a normalised engagement metric</li>
  <li>Identifies high-performing content patterns</li>
  <li>Establishes realistic engagement benchmarks</li>
  <li>Supports strategic planning using data analysis techniques</li>
</ul>

<hr>
<!-- Tableau Dashboard Link Section -->

<h2>Interactive Tableau Dashboard</h2>

<p>
An interactive version of this analysis is available via Tableau Public.  
This dashboard explores audience demographics, including gender and location distributions, and supports deeper investigation of engagement patterns.
</p>

<p>
<a href="https://public.tableau.com/app/profile/alexander.sainsbury/viz/TikTokAnalysis_17641303502480/AudienceGenderandLocationDistributions" target="_blank">
<strong>View the Tableau Dashboard</strong>
</a>
</p>

<hr>

<h2>Objectives</h2>

<ul>
  <li>Develop a standardised engagement score (range 0 to 1)</li>
  <li>Analyse engagement distribution and variability</li>
  <li>Identify characteristics of high-performing content</li>
  <li>Provide actionable recommendations for growth</li>
</ul>

<hr>

<h2>Dataset</h2>

<p>The dataset consists of daily TikTok analytics with the following variables:</p>

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Date</td><td>Recording date</td></tr>
    <tr><td>Video Views</td><td>Total number of views</td></tr>
    <tr><td>Profile Views</td><td>Number of profile visits</td></tr>
    <tr><td>Likes</td><td>Total likes</td></tr>
    <tr><td>Comments</td><td>Total comments</td></tr>
    <tr><td>Shares</td><td>Total shares</td></tr>
    <tr><td>Daily Performance Score</td><td>Calculated engagement metric</td></tr>
  </tbody>
</table>

<hr>

<h2>Methodology</h2>

<h3>Engagement Metric</h3>

<p>
The engagement score is defined as the average proportion of viewers performing key actions:
</p>

<p>
$$
E = \frac{\frac{L}{V} + \frac{C}{V} + \frac{S}{V} + \frac{P}{V}}{4}
$$
</p>

<p>Where:</p>

<ul>
  <li><strong>V</strong> = Views</li>
  <li><strong>L</strong> = Likes</li>
  <li><strong>C</strong> = Comments</li>
  <li><strong>S</strong> = Shares</li>
  <li><strong>P</strong> = Profile Views</li>
</ul>

<h3>Interpretation</h3>

<table>
  <thead>
    <tr>
      <th>Score Range</th>
      <th>Interpretation</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>0</td><td>No engagement</td></tr>
    <tr><td>0.01 – 0.03</td><td>Low engagement</td></tr>
    <tr><td>0.03 – 0.07</td><td>Average engagement</td></tr>
    <tr><td>0.07 – 0.15</td><td>Strong engagement</td></tr>
    <tr><td>&gt; 0.15</td><td>High-performing content</td></tr>
  </tbody>
</table>

<h3>Data Processing</h3>

<ul>
  <li>Handled division-by-zero cases where views = 0</li>
  <li>Standardised date formats across regions</li>
  <li>Cleaned and structured raw exported data</li>
  <li>Prepared data for aggregation and pivot analysis</li>
</ul>

<hr>

<h2>Key Findings</h2>

<ul>
  <li>Engagement distribution is highly skewed, with most days showing near-zero interaction</li>
  <li>High-performing content occurs infrequently but is measurable</li>
  <li>Likes account for the majority of engagement</li>
  <li>Comments and shares occur at significantly lower rates</li>
  <li>Profile views are rare but represent higher intent user behaviour</li>
</ul>

<hr>

<h2>Benchmark Context</h2>

<p>Typical engagement rates observed across TikTok content:</p>

<ul>
  <li>Likes: approximately 2% – 10% of views</li>
  <li>Comments: approximately 0.1% – 1% of views</li>
  <li>Shares: approximately 0.05% – 0.5% of views</li>
</ul>

<p>
These benchmarks indicate that most viewers do not actively engage with content.
</p>

<hr>

<h2>Strategic Insights</h2>

<h3>Effective Content Characteristics</h3>

<ul>
  <li>Strong initial hook within the first few seconds</li>
  <li>Recognisable characters and visual identity</li>
  <li>Community-driven or interactive content</li>
</ul>

<h3>Observed Limitations</h3>

<ul>
  <li>High view counts do not guarantee engagement</li>
  <li>Passive content results in minimal interaction</li>
</ul>

<hr>

<h2>Account Recommendations</h2>

<h3>Content Strategy</h3>

<ul>
  <li>Replicate formats from high-performing posts</li>
  <li>Incorporate prompts for engagement (questions, calls to action)</li>
  <li>Utilise event-based participation (e.g. art challenges)</li>
</ul>

<h3>Engagement Strategy</h3>

<ul>
  <li>Encourage comments and shares explicitly</li>
  <li>Optimise profile presentation to convert views into profile visits</li>
</ul>

<h3>Data Strategy</h3>

<ul>
  <li>Track rolling averages (e.g. 7-day performance)</li>
  <li>Segment analysis by content type</li>
  <li>Refine thresholds using statistical distribution methods</li>
</ul>

<h3>Strategy Framework (VMOST)</h3>
<ul>
  This project includes a structured VMOST analysis outlining the strategic direction for content growth:

- Vision: Long-term community goal
- Mission: Purpose of content creation
- Objectives: Measurable growth targets
- Strategy: High-level approach
- Tactics: Execution plan

[View VMOST Analysis](reports/TikTok_Engagement_Strategy_VMOST_Analysis.pdf)
</ul>

<hr>

<h2>Tools and Technologies</h2>

<p align="left">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge\&logo=git\&logoColor=white" alt="Git"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge\&logo=github\&logoColor=white" alt="GitHub"/>
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge\&logo=power-bi\&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/Tableau-E97627?style=for-the-badge\&logo=tableau\&logoColor=white" alt="Tableau"/>
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge\&logo=microsoft-excel\&logoColor=white" alt="Excel"/>
  <img src="https://img.shields.io/badge/Excel-Data%20Cleaning-217346?style=for-the-badge\&logo=microsoft-excel\&logoColor=white" alt="Excel Data Cleaning"/>
  <img src="https://img.shields.io/badge/Excel-Data%20Analysis-217346?style=for-the-badge\&logo=microsoft-excel\&logoColor=white" alt="Excel Data Analysis"/>
  <img src="https://img.shields.io/badge/Excel-Pivot%20Tables-217346?style=for-the-badge\&logo=microsoft-excel\&logoColor=white" alt="Excel Pivot Tables"/>
</p>

<hr>

<h2>Project Structure</h2>

<pre>
project/
│
├── data/
│   ├── Content_data/
│   └── Followers_data/
│   └── Overviews_data/
│   └── Viewers_data/
│
├── analysis/
│   └── Analysis.xlsx
│
├── dashboards/
│   └── powerbi/
│       └── TikTok Analytics Report.pbix
│
├── reports/
│   └── TikTok_Engagement_Insights.pdf
│   └── TikTok_Engagement_Strategy_VMOST_Analysis.pdf
│
├── images/
│   └── Tableau_dashboard_preview.png
│
└── README.md
</pre>

<hr>

<h2>Future Work</h2>

<ul>
  <li>Incorporate additional metrics such as watch time and completion rate</li>
  <li>Automate data ingestion and processing</li>
  <li>Explore predictive modelling approaches</li>
</ul>

<hr>

<h2>Author</h2>

<p>
Alex Sainsbury<br>
Aspiring Data Analyst
</p>

<hr>

<h2>Conclusion</h2>

<p>
This project demonstrates how structured analysis and quantitative modelling can transform raw social media data into actionable insights for growth and optimisation.
</p>
