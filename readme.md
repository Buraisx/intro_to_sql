[See assignment in Alexa.](https://alexa.bitmaker.co/cohorts/72/assignments/2244/latest)
SELECT * FROM robots WHERE source = 'Star Wars'
SELECT * FROM robots WHERE personality = 'anxious';
SELECT * FROM recipes WHERE nut_free = true;
SELECT COUNT(*) FROM recipes WHERE gluten_free = true AND vegetarian =false;
SELECT  *  FROM animals ORDER BY number_of_legs desc LIMIT 1;
SELECT * FROM board_games ORDER BY mins_to_play ascending ;
SELECT name, MAX(minutes_required) as minutes FROM recipes GROUP BY minutes
SELECT name, minutes_required FROM recipes WHERE minutes_required = (SELECT MAX(minutes_required)FROM recipes);
SELECT * FROM robots WHERE SUBSTRING(name,1,1) = 'M';
SELECT COUNT(*) FROM board_games WHERE max_players >= 8;
SELECT * FROM animals WHERE swimming = true AND egg_laying = true;
SELECT * FROM animals WHERE swimming = true AND egg_laying = true AND flying = false;
SELECT name, max_players FROM board_games WHERE max_players = (SELECT MAX(max_players)FROM board_games);
