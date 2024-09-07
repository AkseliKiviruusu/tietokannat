# kysymys 1
select country.name as "country name", airport.name as "airport name"
from airport
inner join country on airport.iso_country = country.iso_country
and country.name = "Finland"
and scheduled_service = "yes";

![image](https://github.com/user-attachments/assets/7b23be52-9172-4787-9c5c-3d3f4d1da2c5)

# kysymys 2
select screen_name, airport.name
from game
inner join airport on airport.ident = game.location;

![image](https://github.com/user-attachments/assets/3a22c21b-01b3-4b11-adae-a8e7425f762e)

# kysymys 3
select screen_name, country.name
from game
inner join airport on airport.ident = game.location
inner join country on country.iso_country = airport.iso_country;

![image](https://github.com/user-attachments/assets/3300b723-0bcd-48a2-832d-a1ca877a42b8)

# kysymys 4
select airport.name, screen_name
from airport
left join game on location = ident
where airport.name like "%hels%";

![image](https://github.com/user-attachments/assets/b4ab566a-da9d-469f-a938-b7dc7c4d9f80)

# kysymys 5
select goal.name, screen_name
from goal
left join goal_reached on goal.id = goal_id
left join game on game.id = game_id;

![image](https://github.com/user-attachments/assets/6352be9c-3b94-4d37-a9fe-982048b08050)


