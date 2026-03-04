
# NBA Statistics System

The goal of this project is to build a robust system that allows users to interact with professional basketball data through structured queries. It focuses on database schema design, data integrity, and cloud integration.

### Key Features
Based on the `final.py` implementation, the system supports:
* **Seasonal Aggregates**: Querying team performance metrics like Points (PTS), Field Goal Percentage (FG_PCT), and Rebounds (REB).
* **Advanced Game Filters**: Finding specific games based on scoring thresholds (e.g., games with 120+ points) or victory margins.
* **Matchup Analysis**: Identifying a team's most frequent opponents and their historical head-to-head records.
* **User Tracking**: A built-in system to log query history with timestamps, ensuring a record of user interactions.

---

## Technical Stack
* **Database Management**: PostgreSQL
* **Cloud Platform**: Hosted on **AWS RDS** (Amazon Relational Database Service)
* **Database Adapter**: `psycopg2`

---

## Database Design
The system utilizes a relational model with multiple interconnected tables:
1. **`games`**: The core table containing game results and box scores.
2. **`NBA_Team_IDs`**: A mapping table for team names, abbreviations, and unique identifiers.
3. **`Query_History`**: A system table created to store the log of all executed queries.

---
