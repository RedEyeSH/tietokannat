# Where-osan liitosehto harjoitukset
___

### Tehtävä 1
SELECT country.name AS "country name", airport.name AS "airport name" FROM country INNER JOIN airport ON country.iso_country = airport.iso_country WHERE country.name = "Iceland";
![Tehtävä-01.png](Teht%C3%A4v%C3%A4-01.png)

### Tehtävä 2
SELECT name AS "airport name" FROM airport WHERE iso_country = "FR" AND type = "large_airport";
![Tehtävä-02.png](Teht%C3%A4v%C3%A4-02.png)

### Tehtävä 3
SELECT country.name AS "country_name", airport.name AS "airport_name" FROM country INNER JOIN airport ON country.iso_country = airport.iso_country WHERE country.continent = "AN";
![Tehtävä-03.png](Teht%C3%A4v%C3%A4-03.png)

### Tehtävä 4
SELECT elevation_ft FROM airport, game WHERE location = ident AND screen_name = "Heini";
![Tehtävä-04.png](Teht%C3%A4v%C3%A4-04.png)

### Tehtävä 5
SELECT elevation_ft * 0.3048 AS "elevation_m" FROM airport, game WHERE location = ident AND screen_name = "Heini";
![Tehtävä-05.png](Teht%C3%A4v%C3%A4-05.png)

### Tehtävä 6
SELECT name FROM airport, game WHERE location = ident AND screen_name = "Ilkka";
![Tehtävä-06.png](Teht%C3%A4v%C3%A4-06.png)

### Tehtävä 7
SELECT country.name FROM airport, country, game WHERE game.location = airport.ident AND airport.iso_country = country.iso_country AND screen_name = "Ilkka";
![Tehtävä-07.png](Teht%C3%A4v%C3%A4-07.png)

### Tehtävä 8
SELECT goal.name FROM goal, goal_reached, game WHERE goal.id = goal_reached.goal_id AND goal_reached.game_id = game.id AND game.screen_name = "Heini";
![Tehtävä-08.png](Teht%C3%A4v%C3%A4-08.png)

### Tehtävä 9
SELECT airport.name FROM goal, goal_reached, game, airport WHERE goal.id = goal_reached.goal_id AND goal_reached.game_id = game.id AND game.location = airport.ident AND game.screen_name = "Ilkka" AND goal.name = "CLOUDS";
![Tehtävä-09.png](Teht%C3%A4v%C3%A4-09.png)

### Tehtävä 10
SELECT country.name FROM goal, goal_reached, game, airport, country WHERE goal.id = goal_reached.goal_id AND goal_reached.game_id = game.id AND game.location = airport.ident AND airport.iso_country = country.iso_country AND game.screen_name = "Ilkka" AND goal.name = "CLOUDS";
![Tehtävä-10.png](Teht%C3%A4v%C3%A4-10.png)
