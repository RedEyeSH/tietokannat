# Yhteen tauluun kohdistuvien kyselyiden harjoitukset
___
### Tehtävä 1
SELECT * FROM goal;
![Tehtävä-01.png](Teht%C3%A4v%C3%A4-01.png)

### Tehtävä 2
SELECT name, type FROM airport WHERE iso_country = "FI";
![Tehtävä-02.png](Teht%C3%A4v%C3%A4-02.png)

### Tehtävä 3
SELECT name FROM airport WHERE iso_country = "FI" ORDER BY name;
![Tehtävä-03.png](Teht%C3%A4v%C3%A4-03.png)

### Tehtävä 4
SELECT name, type FROM airport WHERE iso_country = "FI" ORDER BY type, name;
![Tehtävä-04.png](Teht%C3%A4v%C3%A4-04.png)

### Tehtävä 5
SELECT name FROM country WHERE name LIKE "f%";
![Tehtävä-05.png](Teht%C3%A4v%C3%A4-05.png)

### Tehtävä 6
SELECT name FROM country WHERE name LIKE "%F%";
![Tehtävä-06.png](Teht%C3%A4v%C3%A4-06.png)

### Tehtävä 7
SELECT location FROM game WHERE screen_name = "Vesa";
![Tehtävä-07.png](Teht%C3%A4v%C3%A4-07.png)

### Tehtävä 8
SELECT co2_consumed FROM game WHERE screen_name = "Ilkka";
![Tehtävä-08.png](Teht%C3%A4v%C3%A4-08.png)

### Tehtävä 9
SELECT DISTINCT co2_budget FROM game;
![Tehtävä-09.png](Teht%C3%A4v%C3%A4-09.png)
