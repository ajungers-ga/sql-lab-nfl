# NFL SQL Lab 🏈

## Overview

This project is **Lab 4** of 5 in the Unit 4 SQL series from my General Assembly software engineering program. 

While Lab 1 ([Carmen Sandiego SQL Lab](https://github.com/ajungers-ga/sql-lab-carmen)) focused on solving clues through data exploration, and Lab 2 ([Computers & Televisions](https://github.com/ajungers-ga/sql-lab-computers-televisions)) was about building and modifying schema structures, **this lab challenged me to query a prebuilt relational database of NFL teams and players**. 

THIS HAS BEEN MY FAVORITE LAB OF THE SERIES! As a NFL stats nerd, this was so much fun revisiting memories of great players from over a decade ago! 

Crazy stat: Tom Brady had a cap hit of $950k in the 2014 NFL season. Furthermore, at the time, Drew Brees ($15,760,000) and Peyton Manning($18,000,000) were taking monster hits to the SALARY CAP against their team.

What happens when the best player in the world takes a pay cut so the team can add MORE talent around him?

9 SB appearances and 6 SB wins with the Patriots.

I had to call in a lifeline for number 9.... thanks for the help, Dad!

The objective: extract structured insights through aggregate functions, filters, sorting, and multi-table joins.

---

### View the SQL Lab series:

- Lab 1 – Find Carmen: https://github.com/ajungers-ga/sql-lab-carmen  
- Lab 2 – Computers & Televisions: https://github.com/ajungers-ga/sql-lab-computers-televisions  
- Lab 3 – Realty: https://github.com/ajungers-ga/sql-lab-realty  
- Lab 4 – NFL: https://github.com/ajungers-ga/sql-lab-nfl  
- Lab 5 – Flights: https://github.com/ajungers-ga/sql-lab-flights  

---

## What I Practiced

- Executing a provided schema and loading seed data with `psql`
- Performing basic and compound `SELECT` queries
- Using `JOIN` to link related data across multiple tables
- Filtering results with `WHERE`, `IS NULL`, and comparative conditions (`>`, `<`, `=`)
- Aggregating data with `AVG`, `SUM`, `COUNT`, and `MAX`
- Sorting and slicing data with `ORDER BY` and `LIMIT`
- Running `.sql` scripts in the CLI using `psql dbname -f file.sql`

---

##  File Breakdown

### `schema.sql`
- Defines two related tables: `teams` and `players`
- Teams have fields like `name`, `division`, `conference`, `head_coach`, and `stadium`
- Players include `name`, `position`, `salary`, and `team_id` (for relational joins)

### `players.sql` & `teams.sql`
- Seeded with full rosters and organizational data
- Loaded via the Postgres CLI

### `nfl.sql`
- Contains 14 completed SQL queries, broken into 4 logical sections:
  - **Queries 1–4**: Basic data exploration (team names, total players)
  - **Queries 5–8**: Multi-condition filtering and salary-based logic
  - **Queries 9–11**: Sorting and aggregating player data
  - **HFM Queries 12–14**: Advanced joins across `players` and `teams` using `JOIN` and `WHERE`

---

## Final Reflections

This lab offered a great blend of real-world SQL logic and sports data. I especially appreciated how the **Hungry For More** section pushed me to join tables and isolate key relationships between players and teams.

It helped reinforce syntax fluency and the need to think through compound logic, like combining `JOIN`, `ORDER BY`, and `LIMIT` in one command. I also got better at debugging (see nfl.sql Lines 62-68), checking schema assumptions, and reviewing logical flow across multiple queries in a single `.sql` file.

---

## Tech Used

- PostgreSQL 16
- CLI with `psql`
- SQL syntax: `SELECT`, `JOIN`, `COUNT`, `AVG`, `SUM`, `MAX`, `ORDER BY`, `LIMIT`, `WHERE`, and `GROUP BY`
