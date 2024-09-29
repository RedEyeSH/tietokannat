# Koostetieto kyselyt harjoitukset
___

# Tehtävä 1
SELECT max(elevation_ft) FROM airport;
![Tehtävä-01.png](Teht%C3%A4v%C3%A4-01.png)

# Tehtävä 2
SELECT continent, count(*) FROM country GROUP BY continent;
![Tehtävä-02.png](Teht%C3%A4v%C3%A4-02.png)

# Tehtävä 3
SELECT screen_name, count(*) FROM game INNER JOIN goal_reached ON game.id = goal_reached.game_id INNER JOIN goal ON goal_reached.goal_id = goal.id GROUP BY screen_name;
![Tehtävä-03.png](Teht%C3%A4v%C3%A4-03.png)

# Tehtävä 4
SELECT screen_name FROM game WHERE co2_consumed IN (SELECT min(co2_consumed) FROM game);
![Tehtävä-04.png](Teht%C3%A4v%C3%A4-04.png)

# Tehtävä 5
SELECT country.name, count(*) FROM airport, country 

WHERE airport.iso_country = country.iso_country 

GROUP BY country.iso_country ORDER BY count(*) DESC LIMIT 50;
![Tehtävä-05.png](Teht%C3%A4v%C3%A4-05.png)

# Tehtävä 6
SELECT country.name FROM country INNER JOIN airport ON country.iso_country = airport.iso_country GROUP BY country.name HAVING count(airport.name) >= 1000 ORDER BY country.iso_country;
![Tehtävä-06.png](Teht%C3%A4v%C3%A4-06.png)

# Tehtävä 7
SELECT airport.name FROM airport WHERE elevation_ft IN(SELECT max(elevation_ft) FROM airport);
![Tehtävä-07.png](Teht%C3%A4v%C3%A4-07.png)

# Tehtävä 8
SELECT country.name FROM country INNER JOIN airport ON country.iso_country = airport.iso_country WHERE airport.elevation_ft IN(SELECT max(elevation_ft) FROM airport);
![Tehtävä-08.png](Teht%C3%A4v%C3%A4-08.png)

# Tehtävä 9
SELECT count(*) FROM game INNER JOIN goal_reached ON game.id = goal_reached.game_id INNER JOIN goal ON goal_reached.goal_id = goal.id WHERE game.screen_name = "Vesa";
![Tehtävä-09.png](Teht%C3%A4v%C3%A4-09.png)

# Tehtävä 10
SELECT name FROM airport WHERE latitude_deg IN(SELECT min(latitude_deg) FROM airport);
![Tehtävä-10.png](Teht%C3%A4v%C3%A4-10.png)
