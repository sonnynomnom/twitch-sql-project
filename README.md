# Codecademy SQL Writing Sample

[Twitch](https://www.twitch.tv) is the world’s leading video platform and community for gamers, with more than 15+ million unique daily visitors. In this project, you will be working with two fictional tables that contain Twitch's streaming data and chat room data and answering questions about them:

- Streaming data is in the `stream` table
- Chat usage data is in the `chat` table

Each question can be answered using one (or more) SQL queries. The answer to the first question is given. The rest is for you to figure out. Let's get started!

---

1. `SELECT` all columns from the first 20 rows of `stream` table.

```sql
SELECT *
FROM stream
LIMIT 20;
```

2. `SELECT` all columns from the first 20 rows of `chat` table.

3. There is something wrong with the `chat` table. Its 1st row is actually the column names. Delete the first row of the `chat` table.

4. What are the `DISTINCT` `channels` in the `stream` table?

5. What are the most popular games in `stream`? Create a list of games and their number of viewers. `ORDER BY` from most popular to least popular.

6. Using a `CASE` statement, create a new column named `genre` for each of the games in `stream`. Group the games into their genres: Multiplayer Online Battle Arena (MOBA), First Person Shooter (FPS), and Others. Your logic should be: *If it is `League of Leagues` or `Dota 2` or `Heroes of the Storm` → then it is `MOBA`. If it is `Counter-Strike: Global Offensive` → then it is `FPS`. Else, it is `Others`.* (Hint: Use `GROUP BY` and `ORDER BY` to showcase only the unique game titles.)

7. The `stream` table and the `chat` table share a column: `device_id`. Do a `JOIN` of the two tables on that column.

8. Try find some other interesting insights using SQL!
