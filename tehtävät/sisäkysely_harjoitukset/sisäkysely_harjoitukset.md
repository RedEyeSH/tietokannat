# Sisäkysely harjoitukset
___

# Tehtävä 1
SELECT name FROM country WHERE iso_country IN(SELECT iso_country FROM airport WHERE name LIKE "%Satsuma%");
![Tehtävä-01.png](Teht%C3%A4v%C3%A4-01.png)

# Tehtävä 2
SELECT name FROM airport WHERE iso_country IN(SELECT iso_country FROM country WHERE name = "Monaco");
![Tehtävä-02.png](Teht%C3%A4v%C3%A4-02.png)

# Tehtävä 3
SELECT screen_name FROM game WHERE id IN(SELECT game_id FROM goal_reached WHERE goal_id IN(SELECT goal.id FROM goal WHERE goal.name = "CLOUDS"));
![Tehtävä-03.png](Teht%C3%A4v%C3%A4-03.png)

# Tehtävä 4
SELECT country.name FROM country WHERE country.iso_country NOT IN(SELECT airport.iso_country FROM airport);
![Tehtävä-04.png](Teht%C3%A4v%C3%A4-04.png)

# Tehtävä 5
SELECT goal.name FROM goal WHERE goal.id NOT IN(SELECT goal_id FROM goal_reached WHERE game_id NOT IN(SELECT game.id FROM game WHERE game.screen_name = "Heini"));
![Tehtävä-05.png](Teht%C3%A4v%C3%A4-05.png)
