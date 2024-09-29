# Join harjoitukset
___

### Tehtävä 1
SELECT country.name AS "country name", airport.name AS "airport name" FROM country INNER JOIN airport ON country.iso_country = airport.iso_country WHERE country.name = "Finland" AND scheduled_service = "yes";
![Tehtävä-01.png](Teht%C3%A4v%C3%A4-01.png)

### Tehtävä 2
SELECT game.screen_name, airport.name FROM game INNER JOIN airport ON game.location = airport.ident;
![Tehtävä-02.png](Teht%C3%A4v%C3%A4-02.png)

### Tehtävä 3
SELECT game.screen_name, country.name FROM game INNER JOIN airport ON game.location = airport.ident INNER JOIN country ON airport.iso_country = country.iso_country;
![Tehtävä-03.png](Teht%C3%A4v%C3%A4-03.png)

### Tehtävä 4
SELECT airport.name, game.screen_name FROM airport LEFT JOIN game ON airport.ident = game.location WHERE airport.name LIKE "%Hels%";
![Tehtävä-04.png](Teht%C3%A4v%C3%A4-04.png)

### Tehtävä 5
SELECT goal.name, game.screen_name FROM goal LEFT JOIN goal_reached ON goal.id = goal_reached.goal_id LEFT JOIN game ON goal_reached.game_id = game.id;
![Tehtävä-05.png](Teht%C3%A4v%C3%A4-05.png)