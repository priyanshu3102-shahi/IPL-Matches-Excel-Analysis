# IPL-Matches-Excel-Analysis
## 📂 Dataset Overview
Matches.csv

Rows: 577

Columns: 19

Key Columns:

Match_Id → Unique match identifier

Match_Date → Match date

Season_Id → Season index

Team_Name_Id, Opponent_Team_Id → Team IDs

Toss_Winner_Id, Toss_Decision

Is_Superover, Is_Result, Is_DuckWorthLewis

Win_Type, Won_By, Match_Winner_Id

Man_Of_The_Match_Id

Venue_Name, City_Name, Host_Country

First_Umpire_Id, Second_Umpire_Id

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Teams.csv<br>
Rows: 13<br>
Columns: 3<br>
Key Columns:<br>
Team_Id → Primary Key<br>
Team_Name → Full team name<br>
Team_Short_Code → Abbreviation<br>

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## ⚙️ Tasks Performed

🔹 Data Cleaning & Preprocessing:
- Applied PROPER() and TRIM() to clean venue, city, and host country names.
- Standardized dates and derived Year and Month.
- Created team lookups using VLOOKUP/XLOOKUP:
- Team_Name_Id → Team_Name & Team_Short_Code
- Opponent_Team_Id → Opponent_Team_Name
- Toss_Winner_Id → Toss_Winner_Name
- Match_Winner_Id → Match_Winner_Name
- Flagged non-standard outcomes (No Result, Tie).
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

 🔹Data Analysis & Calculations
- Win Mode Split → % of wins by chasing vs defending.
- Toss Impact → Toss-to-match win conversion rate per team.
- Identified Top 10 largest win margins (runs & wickets).
- Found Top 10 venues & cities by number of matches and their win distribution.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

🔹 Advanced Excel Concepts
- Conditional formatting to highlight D/L matches.
- Emphasized big wins (≥ 50 runs or ≥ 8 wickets).
- Flagged alerts (no result / missing winner).
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

🔹 Visualization & Dashboard
- Bar Chart → Top 10 teams by total wins.
- Stacked Column → Season-wise win distribution (runs vs wickets).
- Line Chart → Toss decision (field vs bat) trends over seasons.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

📊 Tools Used
- Microsoft Excel
- Functions: PROPER(), TRIM(), VLOOKUP(), XLOOKUP()
- Pivot Tables & Charts
- Conditional Formatting
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

IPL-Excel-Analysis/<br>
│── data/<br>
│   ├── Matches.csv<br>
│   ├── Teams.csv<br>
|<br>
│── analysis/<br>
│   ├── cleaned_dataset.xlsx                       # Preprocessed data<br>
│   ├── Calculations.xlsx                          # pivot tables analysis<br>
│   ├── Advanced_Excel_Concepts.xlsx               # conditional formatting<br>
│   ├── Dashboard.xlsx                             # Final dashboard<br>
│<br>
│── README.md<br>
