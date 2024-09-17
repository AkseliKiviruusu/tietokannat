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

# kysymys 5

