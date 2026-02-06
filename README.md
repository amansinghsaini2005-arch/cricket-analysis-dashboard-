# cricket-analysis-dashboard-

A comprehensive Power BI dashboard analyzing the international cricket career of Virat Kohli. This project visualizes key performance metrics including runs, centuries, and match statistics across different formats and opponents, utilizing data from his debut in 2008 through 2022.
📋 Project Overview
This dashboard transforms raw match-by-match data into an interactive visual story. It allows users to explore Kohli's batting performance through dynamic filtering and custom visualizations. The design focuses on a modern "Glassmorphism" aesthetic with a custom AI-generated background.
✨ Key Features
• Dynamic KPI Cards: Utilizes the "New Card" visual in Power BI to display high-level metrics:
    ◦ Total Matches Played
    ◦ Total Runs Scored
    ◦ Total Centuries (100s)
    ◦ Total Half-Centuries (50s)
    ◦ 30+ Scores
• Time-Series Analysis: A Waterfall Chart visualizes year-on-year performance trends.
• Opponent & Format Analysis:
    ◦ Donut Chart: Break down of matches played against different opponents.
    ◦ Column Chart: Analysis of runs scored against specific teams.
    ◦ Note: Charts are optimized to show "Top 5" categories to maintain a clean design.
• Interactive Filtering: A dedicated Year Slicer allows users to filter the entire dashboard to specific career periods.
• Dynamic Titles: Custom DAX measures generate dynamic titles and text based on user selection (e.g., Debut Date).
📂 Data Source
The project uses a raw CSV file (Source.csv) containing detailed match data:
• Columns: index, runs, opponent, ground, date, match (Format: ODI, Test, T20), Match_No, total.
• Date Range: Covers matches from his debut (Aug 2008) to July 2022.
🛠️ Technical Implementation
Data Transformation
• Data Import: Loaded via "Get Data > Text/CSV" in Power BI.
• Calendar Table: A dedicated date table was created and linked to the main data table to manage time-intelligence functions.
• Calculated Columns: Custom logic added to flag specific milestones:
    ◦ Century (Runs >= 100)
    ◦ Fifty (Runs >= 50 and < 100)
    ◦ 30s (Runs >= 30 and < 50).
DAX Measures
A separate table was created to organize all measures. Key calculations include:
• Debut Date: Calculated dynamically using the MIN() function on the date column.
• Format Specifics: Logic to filter stats based on ODI, T20, or Test formats.
Design Elements
• Background: Custom background image generated via AI and edited for a "glass layer" effect to enhance visual depth.
• Visual Cleaning: Axes and labels were cleaned or removed to create a minimalist look focused on data trends.
