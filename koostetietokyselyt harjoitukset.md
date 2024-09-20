# kysymys 1

select max(elevation_ft)
from airport;

![image](https://github.com/user-attachments/assets/7108ee6f-fe58-496d-9542-166da5000dc0)

# kysymys 2

select continent, count(*)
from country
group by continent;

![image](https://github.com/user-attachments/assets/9b124b3a-98b0-4bbf-8f19-ce1b69a06021)

# kysymys 3

select screen_name, count(*)
from game
inner join goal_reached on game.id = goal_reached.game_id
group by screen_name;

![image](https://github.com/user-attachments/assets/b6f43803-6b57-4855-bdeb-25ae46ca3059)

# kysymys 4

select screen_name
from game
where co2_consumed in(
select min(co2_consumed)
from game
);

![image](https://github.com/user-attachments/assets/1f71d4b7-d82b-459c-859f-3162d5c87198)

# kysymys 5 (moodle ei tykännyt vastauksestani, vaikka "odotettu" ja "saatu" olivat identtiset)

select country.name, count(*)
from country
inner join airport on country.iso_country = airport.iso_country
group by country.name
order by count(*) desc
limit 50;

![image](https://github.com/user-attachments/assets/1b7c5f17-85a8-4eae-ab14-e7a800d853ed)

# kysymys 6

select country.name
from country
inner join airport on country.iso_country = airport.iso_country
group by country.iso_country
having count(*) >= 1000;

![image](https://github.com/user-attachments/assets/ddf69319-cceb-42ae-a003-1542f5f9c2d7)

# kysymys 7

select name
from airport
where elevation_ft in(
select max(elevation_ft)
from airport
);

![image](https://github.com/user-attachments/assets/f91f2c39-a139-47e7-8fc7-336c0a29638b)

# kysymys 8

select name
from country
where iso_country in(
select iso_country
from airport
where elevation_ft in(
select max(elevation_ft)
from airport
)
);

![image](https://github.com/user-attachments/assets/2c3cab2e-d0b5-487f-9aac-014fd9ac28ac)

# kysymys 9

select count(*)
from goal_reached
where game_id in(
select id
from game
where screen_name = "Vesa"
);

![image](https://github.com/user-attachments/assets/98c04318-1c3a-4e16-85e3-d742a1f23de4)

# kysymys 10

select name 
from airport
where latitude_deg in(
select min(latitude_deg)
from airport
);

![image](https://github.com/user-attachments/assets/c869c326-844c-4c6f-9f6b-f33d534d9568)

