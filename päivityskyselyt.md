# kysymys 1

update game
set location =(
select ident
from airport
where name = "Nottingham Airport")
where location in(
select location
from game
where screen_name = "Vesa"
);
update game
set co2_consumed =(co2_consumed + 500)
where screen_name = "Vesa";

![image](https://github.com/user-attachments/assets/05d378d4-bca1-4c7e-8d0d-f5f8c02b4733)

# kysymys 3

delete from goal_reached;

![image](https://github.com/user-attachments/assets/81f898d7-1cda-4e81-8d38-1aa84dc343d6)

# kysymys 4

delete from game;

![image](https://github.com/user-attachments/assets/a4befa29-e284-4b4c-a029-9951f63f206b)
