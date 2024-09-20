# where_osan liitosehto harjoitukset

# kysymys 1
select country.name as "country name", airport.name as "airport name"
from country, airport
where airport.iso_country = country.iso_country
and country.name = "Iceland";

![Näyttökuva 2024-09-06 144737](https://github.com/user-attachments/assets/9edcd437-cd0c-42e6-987d-9708443c7f96)

# kysymys 2
select airport.name as "airport name"
from country, airport
where airport.type = "large_airport"
and airport.iso_country = country.iso_country
and country.name = "France";

![image](https://github.com/user-attachments/assets/53ac8d9c-6dca-4890-914c-d4f001e3cfd4)

# kysymys 3
select country.name as "country_name", airport.name as "airport_name"
from country, airport
where airport.iso_country = country.iso_country
and country.continent = "AN";

![image](https://github.com/user-attachments/assets/e0a069ae-6ad6-4a40-b3a1-0390714c21c8)

# kysymys 4
select elevation_ft
from airport, game
where game.screen_name = "Heini"
and airport.ident = game.location;


![image](https://github.com/user-attachments/assets/e9854513-980a-430b-97e6-085517ea251a)

# kysymys 5
select (elevation_ft * 0.3048) as "elevation_m"
from airport, game
where game.screen_name = "Heini"
and airport.ident = game.location;

![image](https://github.com/user-attachments/assets/d7e441b6-df7b-4bbe-bc2a-3814296594cc)

# kysymys 6
select airport.name
from airport, game
where airport.ident = game.location
and game.screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/5588b515-74c3-4cbe-834e-ff32d167687b)

# kysymys 7
select country.name
from country, airport, game
where game.location = airport.ident
and airport.iso_country = country.iso_country
and game.screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/0bb0f0d6-2bd6-44b5-9415-80e2c38c85a6)

# kysymys 8
select name
from goal, goal_reached, game
where game.id = game_id
and goal.id = goal_id
and screen_name = "Heini";

![image](https://github.com/user-attachments/assets/2c0fa8ab-3bbd-418b-8f87-4a7899647782)

# kysymys 9
select airport.name
from airport, game, goal_reached, goal
where airport.ident = game.location
and game.id = game_id
and goal.id = goal_id
and screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/2715262d-1cbd-4bee-b3d9-d4277b8e51b9)

# kysymys 10
select country.name
from airport, game, goal_reached, goal, country
where airport.ident = game.location
and game.id = game_id
and goal.id = goal_id
and country.iso_country = airport.iso_country
and screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/253b4886-1ef3-40e3-b0d9-6e44dfec8cbc)
