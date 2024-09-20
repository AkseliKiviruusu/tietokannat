# kysymys 1

select country.name
from country
where iso_country in(
select iso_country
from airport
where airport.name like "Satsuma%"
);

![image](https://github.com/user-attachments/assets/8f9e77ed-880e-4d87-9fe3-2f5012ba6f1a)

# kysymys 2

select airport.name
from airport
where iso_country in(
select iso_country
from country
where country.name = "Monaco"
);

![image](https://github.com/user-attachments/assets/6803ddb1-eebd-41c1-90d6-dd15eb2a858b)

# kysymys 3

select screen_name
from game
where id in(
select game_id
from goal_reached
where goal_id in(
select id
from goal
where name = "clouds"
)
);

![image](https://github.com/user-attachments/assets/1cdc5258-1c97-4faa-a048-6767333057fd)

# kysymys 4

select name
from country
where iso_country not in(
select iso_country
from airport
);

![image](https://github.com/user-attachments/assets/e6e8715a-c572-4c57-aa19-3e6a641086c6)

# kysymys 5

select name
from goal
where id not in(
select goal_id
from goal_reached
where game_id not in(
select screen_name
from game
where screen_name = "Heini"
)
);

![image](https://github.com/user-attachments/assets/ff39d26b-550c-4289-b130-2bfadb7f9540)
