# Soccer End-to-End Database Design Project
## Narrative
The soccer league administrator wants to create a database to track teams, players, coaches, matches, fields, vendors, referees, and sponsors. 
Reports include: match scores and results, player stats, referee assignments, team rosters, field and team sponsors, vendor types and field assignments, and coach assignments. 

The soccer league consists of teams. Teams have one or more sponsors whose names appear on the team uniforms. Sponsors can support more than one team, and a team may have more than one sponsor at a time. Sponsorships are tracked by season. 

Each team consists of players. No player belongs to more than one team during a single season. Each player is assigned a unique Player ID when they join the league.  The league records each player’s name and address, parent contact name, player phone number and parent phone number, and parent email. In order to verify players ages, the league also records each player’s date of birth. Each team has a designated captain from among the players. Players are registered for the league followed by a draft to receive their team assignments. Players can play for one team one season and then play for a different team the next season. 

Teams play in matches. Each match is given a unique Match ID number and is scheduled for a specific date. The league records the goals scored by each team and the win or loss result.  

Player performance in each match is recorded for minutes played, goals scored, and penalties assessed.  It is possible for a player to not participate in a match.

The league assigns three referees to each match, based on position (one head (H) and two linesmen (L)).  Referees are assigned a unique Referee ID number when they first register with the league.  The league records each referee’s name (first name and last name), address and phone number, and contact email.  Each new referee is assigned to one experienced referee as a mentor.  Not all of the experienced referees serve as mentors, but those that do can mentor more than one new referee.

Matches take place at soccer fields. Sponsors can support fields by placing banners. Sponsors can support more than one field, and fields can have more than one banner. The league records the name and address (street, city, state, and zip) of all the fields where it stages matches. Each match, occurs at a single field at a time. The fields host multiple matches throughout the season. Some fields are closed when undergoing renovations with no matches scheduled during that period.

Vendors sell items at specific fields. Each field has several vendors. The league tracks the vendor assignments by season. In addition to the vendor’s name, the league records the vendor phone number and the vendor type. Some vendors offer multiple types of services, for example: food, beverage, clothing, soccer suppliers, and other items.

The league also tracks coaches. A coach can be assigned to more than one team, but only as one role per assignment. Coaching roles are head (HC), assistant (AC), volunteer (VC). Each team can have multiple coaches, but only one role at a time may be assigned to a single coach. Coach assignments are based upon season. 

**Reports**
League administrator wants to run the following reports:
1.	Team Rosters – player full name and age calculated from DOB.
2.	Game Report – teams, goals scored, win/loss, head coach, head ref, date, match number.
3.	Player Performance – play full name, total minutes played, penalties, goals, games.
4.	Team Report – team name, games played, goals for and goals against, differential, win/loss record. 

**Rosters**
The league wants to be able to track rosters for each season. You need to figure out how to design the relationship between players and teams to support the tracking of player/team assignments based on season. 

## Skills Learned
- Developed an end-to-end SQL project utilizing ERD (Entities, Attributes, Cardinality, Optionality, dependent entities, associative entity), EERD, and Relational Schema
- Utilized Microsoft Visio and Dictionary for database design and organization
- Built a database with derived attributes (such as calculating age from DoB), and set primary keys, foreign keys, recursive foreign keys, composite keys, and unique keys
- Implemented different types of indexes including clustered, non-clustered, and filtered index, as well as composite indexes
- Created user-defined data types, set default values, and applied Check Constraints and triggers (including delete trigger, update trigger, instead of trigger, and history table)
- Inserted values into the table using generatedata.com, and created views and indexed views
Developed stored procedures (SPROC) with and without parameters
- Utilized advanced SQL techniques such as JOIN (INNER, LEFT/RIGHT, FULL, CROSS, SELF), Nested Queries, CTE, HAVING, GROUP BY, Joining a view to a table, PARTITION BY, and DATEADD.

Additionally, created a comprehensive diagram to illustrate the project.


