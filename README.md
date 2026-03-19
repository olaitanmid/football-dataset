CREATE TABLE premier_league_table (
    position INT PRIMARY KEY,
    team VARCHAR(100) NOT NULL,
    played INT,
    won INT,
    draw INT,
    lost INT,
    goals_for INT,
    goals_against INT,
    goal_diff INT,
    points INT
);
INSERT INTO premier_league_table VALUES
(1, 'Manchester City', 38, 28, 6, 4, 94, 33, 61, 90),
(2, 'Arsenal', 38, 27, 5, 6, 88, 43, 45, 86),
(3, 'Liverpool', 38, 24, 8, 6, 85, 41, 44, 80),
(4, 'Aston Villa', 38, 21, 8, 9, 76, 61, 15, 71),
(5, 'Tottenham Hotspur', 38, 20, 6, 12, 74, 61, 13, 66),
(6, 'Chelsea', 38, 18, 9, 11, 70, 63, 7, 63),
(7, 'Newcastle United', 38, 18, 6, 14, 68, 62, 6, 60),
(8, 'Manchester United', 38, 17, 6, 15, 57, 58, -1, 57),
(9, 'West Ham United', 38, 14, 10, 14, 60, 74, -14, 52),
(10, 'Crystal Palace', 38, 13, 10, 15, 49, 55, -6, 49),
(11, 'Brighton & Hove Albion', 38, 12, 12, 14, 55, 59, -4, 48),
(12, 'Bournemouth', 38, 12, 10, 16, 54, 67, -13, 46),
(13, 'Fulham', 38, 11, 11, 16, 50, 65, -15, 44),
(14, 'Wolverhampton Wanderers', 38, 11, 8, 19, 46, 61, -15, 41),
(15, 'Everton', 38, 10, 9, 19, 42, 60, -18, 39),
(16, 'Brentford', 38, 9, 11, 18, 49, 65, -16, 38),
(17, 'Nottingham Forest', 38, 9, 9, 20, 44, 68, -24, 36),
(18, 'Luton Town', 38, 7, 8, 23, 40, 75, -35, 29),
(19, 'Burnley', 38, 5, 9, 24, 38, 78, -40, 24),
(20, 'Sheffield United', 38, 3, 7, 28, 35, 90, -55, 16);

| position | team                    | played | won | draw | lost | goals_for | goals_against | goal_diff | points |
| -------- | ----------------------- | ------ | --- | ---- | ---- | --------- | ------------- | --------- | ------ |
| 1        | Manchester City         | 38     | 28  | 6    | 4    | 94        | 33            | +61       | 90     |
| 2        | Arsenal                 | 38     | 27  | 5    | 6    | 88        | 43            | +45       | 86     |
| 3        | Liverpool               | 38     | 24  | 8    | 6    | 85        | 41            | +44       | 80     |
| 4        | Aston Villa             | 38     | 21  | 8    | 9    | 76        | 61            | +15       | 71     |
| 5        | Tottenham Hotspur       | 38     | 20  | 6    | 12   | 74        | 61            | +13       | 66     |
| 6        | Chelsea                 | 38     | 18  | 9    | 11   | 70        | 63            | +7        | 63     |
| 7        | Newcastle United        | 38     | 18  | 6    | 14   | 68        | 62            | +6        | 60     |
| 8        | Manchester United       | 38     | 17  | 6    | 15   | 57        | 58            | -1        | 57     |
| 9        | West Ham United         | 38     | 14  | 10   | 14   | 60        | 74            | -14       | 52     |
| 10       | Crystal Palace          | 38     | 13  | 10   | 15   | 49        | 55            | -6        | 49     |
| 11       | Brighton & Hove Albion  | 38     | 12  | 12   | 14   | 55        | 59            | -4        | 48     |
| 12       | Bournemouth             | 38     | 12  | 10   | 16   | 54        | 67            | -13       | 46     |
| 13       | Fulham                  | 38     | 11  | 11   | 16   | 50        | 65            | -15       | 44     |
| 14       | Wolverhampton Wanderers | 38     | 11  | 8    | 19   | 46        | 61            | -15       | 41     |
| 15       | Everton                 | 38     | 10  | 9    | 19   | 42        | 60            | -18       | 39     |
| 16       | Brentford               | 38     | 9   | 11   | 18   | 49        | 65            | -16       | 38     |
| 17       | Nottingham Forest       | 38     | 9   | 9    | 20   | 44        | 68            | -24       | 36     |
| 18       | Luton Town              | 38     | 7   | 8    | 23   | 40        | 75            | -35       | 29     |
| 19       | Burnley                 | 38     | 5   | 9    | 24   | 38        |  78           | -40       | 24     | 
  20         Sheffield United        | 38     | 3    |  7  |  28  | 35        | 90            | -55       | 16     |

QUERIES;
View the full table
Query Result;
SELECT * FROM premier_league_table ORDER BY position;

| position | team                    | played | won | draw | lost | goals_for | goals_against | goal_diff | points |
| -------- | ----------------------- | ------ | --- | ---- | ---- | --------- | ------------- | --------- | ------ |
| 1        | Manchester City         | 38     | 28  | 6    | 4    | 94        | 33            | 61        | 90     |
| 2        | Arsenal                 | 38     | 27  | 5    | 6    | 88        | 43            | 45        | 86     |
| 3        | Liverpool               | 38     | 24  | 8    | 6    | 85        | 41            | 44        | 80     |
| 4        | Aston Villa             | 38     | 21  | 8    | 9    | 76        | 61            | 15        | 71     |
| 5        | Tottenham Hotspur       | 38     | 20  | 6    | 12   | 74        | 61            | 13        | 66     |
| 6        | Chelsea                 | 38     | 18  | 9    | 11   | 70        | 63            | 7         | 63     |
| 7        | Newcastle United        | 38     | 18  | 6    | 14   | 68        | 62            | 6         | 60     |
| 8        | Manchester United       | 38     | 17  | 6    | 15   | 57        | 58            | -1        | 57     |
| 9        | West Ham United         | 38     | 14  | 10   | 14   | 60        | 74            | -14       | 52     |
| 10       | Crystal Palace          | 38     | 13  | 10   | 15   | 49        | 55            | -6        | 49     |
| 11       | Brighton & Hove Albion  | 38     | 12  | 12   | 14   | 55        | 59            | -4        | 48     |
| 12       | Bournemouth             | 38     | 12  | 10   | 16   | 54        | 67            | -13       | 46     |
| 13       | Fulham                  | 38     | 11  | 11   | 16   | 50        | 65            | -15       | 44     |
| 14       | Wolverhampton Wanderers | 38     | 11  | 8    | 19   | 46        | 61            | -15       | 41     |
| 15       | Everton                 | 38     | 10  | 9    | 19   | 42        | 60            | -18       | 39     |
| 16       | Brentford               | 38     | 9   | 11   | 18   | 49        | 65            | -16       | 38     |
| 17       | Nottingham Forest       | 38     | 9   | 9    | 20   | 44        | 68            | -24       | 36     |
| 18       | Luton Town              | 38     | 7   | 8    | 23   | 40        | 75            | -35       | 29     |
| 19       | Burnley                 | 38     | 5   | 9    | 24   | 38        | 78            | -40       | 24     |
| 20       | Sheffield United        | 38     | 3   | 7    | 28   | 35        | 90            | -55       | 16     |

QUERY;
Top 4 Teams (Champions League spots)
Query Result;
SELECT * FROM premier_league_table WHERE position <= 4;
| position | team            | played | won | draw | lost | goals_for | goals_against | goal_diff | points |
| -------- | --------------- | ------ | --- | ---- | ---- | --------- | ------------- | --------- | ------ |
| 1        | Manchester City | 38     | 28  | 6    | 4    | 94        | 33            | 61        | 90     |
| 2        | Arsenal         | 38     | 27  | 5    | 6    | 88        | 43            | 45        | 86     |
| 3        | Liverpool       | 38     | 24  | 8    | 6    | 85        | 41            | 44        | 80     |
| 4        | Aston Villa     | 38     | 21  | 8    | 9    | 76        | 61            | 15        | 71     |

QUERY;
Find the Relegated Teams (Bottom 4)
Query Result;
SELECT team_name, points
FROM teams
ORDER BY points ASC
LIMIT 4;
| team              | points |
| ----------------- | ------ |
| Sheffield United  | 16     |
| Burnley           | 24     |
| Luton Town        | 29     |
| Nottingham Forest | 36     |

QUERY;
Team with Most Goals Scored
Query Result;
SELECT team, goals_for
FROM premier_league_table
ORDER BY goals_for DESC
LIMIT 1;

| team            | goals_for |
| --------------- | --------- |
| Manchester City | 94        |


QUERY;
Best Defense (Least Goals Conceded)
Query Result;
SELECT team, goals_against
FROM premier_league_table
ORDER BY goals_against ASC
LIMIT 1;
| team            | goals_against |
| --------------- | ------------- |
| Manchester City | 33            |


QUERY;
Best Goal Difference
Query Result;
SELECT team, goal_diff
FROM premier_league_table
ORDER BY goal_diff DESC
LIMIT 5;

| team              | goal_diff |
| ----------------- | --------- |
| Manchester City   | 61        |
| Arsenal           | 45        |
| Liverpool         | 44        |
| Aston Villa       | 15        |
| Tottenham Hotspur | 13        |

QUERY;
 Teams with More Than 70 Points
 Query Result;
 SELECT team, points
FROM premier_league_table
WHERE points > 70
ORDER BY points DESC;

| team            | points |
| --------------- | ------ |
| Manchester City | 90     |
| Arsenal         | 86     |
| Liverpool       | 80     |
| Aston Villa     | 71     |

QUERY;
Compare Two Teams
Query Result;
SELECT team, points, goal_diff
FROM premier_league_table
WHERE team IN ('Arsenal', 'Liverpool');

| team      | points | goal_diff |
| --------- | ------ | --------- |
| Arsenal   | 86     | 45        |
| Liverpool | 80     | 44        |

QUERY;
Average Points in the League
Query Result;
SELECT AVG(points) AS avg_points
FROM premier_league_table;

| avg_points |
| ---------- |
| 55.3       |

QUERY;
 Find the Win Percentage
Query Result;
SELECT 
    team,
    played,
    won,
    ROUND((won * 100.0 / played), 2) AS win_percentage
FROM premier_league_table
ORDER BY win_percentage DESC;

| team                    | played | won | win_percentage |
| ----------------------- | ------ | --- | -------------- |
| Manchester City         | 38     | 28  | 73.68          |
| Arsenal                 | 38     | 27  | 71.05          |
| Liverpool               | 38     | 24  | 63.16          |
| Aston Villa             | 38     | 21  | 55.26          |
| Tottenham Hotspur       | 38     | 20  | 52.63          |
| Chelsea                 | 38     | 18  | 47.37          |
| Newcastle United        | 38     | 18  | 47.37          |
| Manchester United       | 38     | 17  | 44.74          |
| West Ham United         | 38     | 14  | 36.84          |
| Crystal Palace          | 38     | 13  | 34.21          |
| Brighton & Hove Albion  | 38     | 12  | 31.58          |
| Bournemouth             | 38     | 12  | 31.58          |
| Fulham                  | 38     | 11  | 28.95          |
| Wolverhampton Wanderers | 38     | 11  | 28.95          |
| Everton                 | 38     | 10  | 26.32          |
| Nottingham Forest       | 38     | 9   | 23.68          |
| Brentford               | 38     | 9   | 23.68          |
| Sheffield United        | 38     | 3   | 7.89           |
| Burnley                 | 38     | 5   | 13.16          |
| Luton Town              | 38     | 7   | 18.42          |

  
| 19       | Burnley                 | 38     | 5   | 9    | 24   | 38        | 78            | -40       | 24     |
| 20       | Sheffield United        | 38     | 3   |  7    | 28   | 35        | 90            | -55       | 16     |
 
